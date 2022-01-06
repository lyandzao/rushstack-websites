---
hide_title: true
custom_edit_url: null
pagination_prev: null
pagination_next: null
---
<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@microsoft/rush-lib](./rush-lib.md) &gt; [VersionPolicy](./rush-lib.versionpolicy.md) &gt; [setDependenciesBeforePublish](./rush-lib.versionpolicy.setdependenciesbeforepublish.md)

## VersionPolicy.setDependenciesBeforePublish() method

> This API is provided as a preview for developers and may change based on feedback that we receive. Do not use this API in a production environment.
> 

Tells the version policy to modify any dependencies in the target package to values used for publishing.

<b>Signature:</b>

```typescript
setDependenciesBeforePublish(packageName: string, configuration: RushConfiguration): void;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  packageName | string |  |
|  configuration | [RushConfiguration](./rush-lib.rushconfiguration.md) |  |

<b>Returns:</b>

void
