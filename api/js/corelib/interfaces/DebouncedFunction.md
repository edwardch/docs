[@serenity-is/corelib](../README.md) / DebouncedFunction

# Interface: DebouncedFunction\<T\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends (...`args`: `any`[]) => `any` |

## Callable

### DebouncedFunction

▸ **DebouncedFunction**(`...args`): `ReturnType`\<`T`\>

Call the original function, but applying the debounce rules.

If the debounced function can be run immediately, this calls it and returns its return
value.

Otherwise, it returns the return value of the last invocation, or undefined if the debounced
function was not invoked yet.

#### Parameters

| Name | Type |
| :------ | :------ |
| `...args` | `Parameters`\<`T`\> |

#### Returns

`ReturnType`\<`T`\>

#### Defined in

[src/base/debounce.ts:11](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/base/debounce.ts#L11)

## Table of contents

### Methods

- [clear](DebouncedFunction.md#clear)
- [flush](DebouncedFunction.md#flush)

## Methods

### clear

▸ **clear**(): `void`

Throw away any pending invocation of the debounced function.

#### Returns

`void`

#### Defined in

[src/base/debounce.ts:16](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/base/debounce.ts#L16)

___

### flush

▸ **flush**(): `ReturnType`\<`T`\>

If there is a pending invocation of the debounced function, invoke it immediately and return
its return value.

Otherwise, return the value from the last invocation, or undefined if the debounced function
was never invoked.

#### Returns

`ReturnType`\<`T`\>

#### Defined in

[src/base/debounce.ts:25](https://github.com/serenity-is/serenity/blob/master/packages/corelib/src/base/debounce.ts#L25)
