---
id: UnwrapFormAsyncValidateOrFn
title: UnwrapFormAsyncValidateOrFn
---

<!-- DO NOT EDIT: this page is autogenerated from the type comments -->

# Type Alias: UnwrapFormAsyncValidateOrFn\<TValidateOrFn\>

```ts
type UnwrapFormAsyncValidateOrFn<TValidateOrFn> = [TValidateOrFn] extends [FormValidateAsyncFn<any>] ? Awaited<ReturnType<TValidateOrFn>> : [TValidateOrFn] extends [StandardSchemaV1<any, any>] ? Record<string, StandardSchemaV1Issue[]> : undefined;
```

Defined in: [packages/form-core/src/FormApi.ts:141](https://github.com/TanStack/form/blob/main/packages/form-core/src/FormApi.ts#L141)

## Type Parameters

• **TValidateOrFn** *extends* `undefined` \| `FormAsyncValidateOrFn`\<`any`\>
