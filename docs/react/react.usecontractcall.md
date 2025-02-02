---
slug: /react.usecontractcall
title: useContractCall() function
hide_title: true
displayed_sidebar: react
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## useContractCall() function

> This API is provided as a preview for developers and may change based on feedback that we receive. Do not use this API in a production environment.

Use this to get a function to make a write call to your contract

## Example

```javascript
const { contract } = useContract("{{contract_address}}");
const {
  mutate: myFunction,
  isLoading,
  error,
} = useContractCall(contract, "myFunction");

// the function can be called as follows:
// myFunction(...args)
```

**Signature:**

```typescript
export declare function useContractCall(
  contract: RequiredParam<ReturnType<typeof useContract>["contract"]>,
  functionName: RequiredParam<string>,
): import("@tanstack/react-query").UseMutationResult<
  any,
  unknown,
  unknown,
  unknown
>;
```

## Parameters

| Parameter    | Type                                                                                                | Description                                                 |
| ------------ | --------------------------------------------------------------------------------------------------- | ----------------------------------------------------------- |
| contract     | [RequiredParam](./react.requiredparam.md)&lt;ReturnType&lt;typeof useContract&gt;\["contract"\]&gt; | the contract instance of the contract to call a function on |
| functionName | [RequiredParam](./react.requiredparam.md)&lt;string&gt;                                             | the name of the function to call                            |

**Returns:**

import("@tanstack/react-query").UseMutationResult&lt;any, unknown, unknown, unknown&gt;

a response object that includes the write function to call
