[@tauri-apps/api](../README.md) / process

# Module: process

Perform operations on the current process.

This package is also accessible with `window.__TAURI__.process` when `tauri.conf.json > build > withGlobalTauri` is set to true.

## Functions

### exit

▸ **exit**(`exitCode?`): `Promise`<`void`\>

Exits immediately with the given `exitCode`.

**`example`**
```typescript
import { exit } from '@tauri-apps/api/process';
await exit(1);
```

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `exitCode` | `number` | `0` | The exit code to use. |

#### Returns

`Promise`<`void`\>

A promise indicating the success or failure of the operation.

#### Defined in

[process.ts:25](https://github.com/tauri-apps/tauri/blob/dc432ef/tooling/api/src/process.ts#L25)

___

### relaunch

▸ **relaunch**(): `Promise`<`void`\>

Exits the current instance of the app then relaunches it.

**`example`**
```typescript
import { relaunch } from '@tauri-apps/api/process';
await relaunch();
```

#### Returns

`Promise`<`void`\>

A promise indicating the success or failure of the operation.

#### Defined in

[process.ts:45](https://github.com/tauri-apps/tauri/blob/dc432ef/tooling/api/src/process.ts#L45)
