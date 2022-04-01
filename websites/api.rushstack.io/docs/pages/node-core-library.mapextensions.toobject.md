---
hide_title: true
custom_edit_url: null
pagination_prev: null
pagination_next: null
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@rushstack/node-core-library](./node-core-library.md) &gt; [MapExtensions](./node-core-library.mapextensions.md) &gt; [toObject](./node-core-library.mapextensions.toobject.md)

## MapExtensions.toObject() method

Converts a string-keyed map to an object.

<b>Signature:</b>

```typescript
static toObject<TValue>(map: Map<string, TValue>): {
        [key: string]: TValue;
    };
```

## Parameters

| Parameter | Type                      | Description                                             |
| --------- | ------------------------- | ------------------------------------------------------- |
| map       | Map&lt;string, TValue&gt; | The map that the object properties will be sourced from |

<b>Returns:</b>

{ \[key: string\]: TValue; }

## Remarks

This function has the same effect as Object.fromEntries(map.entries()) in supported versions of Node ( &gt; = 12.0.0).