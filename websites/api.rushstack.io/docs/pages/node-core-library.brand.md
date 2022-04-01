---
hide_title: true
custom_edit_url: null
pagination_prev: null
pagination_next: null
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@rushstack/node-core-library](./node-core-library.md) &gt; [Brand](./node-core-library.brand.md)

## Brand type

A "branded type" is a primitive type with a compile-type key that makes it incompatible with other aliases for the primitive type.

<b>Signature:</b>

```typescript
export declare type Brand<T, BrandTag extends string> = T & {
  __brand: BrandTag;
};
```

## Remarks

Example usage:

```ts
// PhoneNumber is a branded type based on the "string" primitive.
type PhoneNumber = Brand<string, 'PhoneNumber'>;

function createPhoneNumber(input: string): PhoneNumber {
  if (!/\d+(\-\d+)+/.test(input)) {
    throw new Error('Invalid phone number: ' + JSON.stringify(input));
  }
  return input as PhoneNumber;
}

const p1: PhoneNumber = createPhoneNumber('123-456-7890');

// PhoneNumber is a string and can be used as one:
const p2: string = p1;

// But an arbitrary string cannot be implicitly type cast as PhoneNumber.
// ERROR: Type 'string' is not assignable to type 'PhoneNumber'
const p3: PhoneNumber = '123-456-7890';
```

For more information about this pattern, see [this comment](https://github.com/Microsoft/TypeScript/blob/7b48a182c05ea4dea81bab73ecbbe9e013a79e99/src/compiler/types.ts#L693-L698) explaining the TypeScript compiler's introduction of this pattern, and [this article](https://spin.atomicobject.com/2018/01/15/typescript-flexible-nominal-typing/) explaining the technique in depth.