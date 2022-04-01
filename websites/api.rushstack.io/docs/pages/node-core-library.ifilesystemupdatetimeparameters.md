---
hide_title: true
custom_edit_url: null
pagination_prev: null
pagination_next: null
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@rushstack/node-core-library](./node-core-library.md) &gt; [IFileSystemUpdateTimeParameters](./node-core-library.ifilesystemupdatetimeparameters.md)

## IFileSystemUpdateTimeParameters interface

The options for [FileSystem.updateTimes()](./node-core-library.filesystem.updatetimes.md) Both times must be specified.

<b>Signature:</b>

```typescript
export interface IFileSystemUpdateTimeParameters
```

## Properties

| Property                                                                            | Type           | Description                                               |
| ----------------------------------------------------------------------------------- | -------------- | --------------------------------------------------------- |
| [accessedTime](./node-core-library.ifilesystemupdatetimeparameters.accessedtime.md) | number \| Date | The POSIX epoch time or Date when this was last accessed. |
| [modifiedTime](./node-core-library.ifilesystemupdatetimeparameters.modifiedtime.md) | number \| Date | The POSIX epoch time or Date when this was last modified  |