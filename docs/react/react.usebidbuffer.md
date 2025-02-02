---
slug: /react.usebidbuffer
title: useBidBuffer() function
hide_title: true
displayed_sidebar: react
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## useBidBuffer() function

> This API is provided as a preview for developers and may change based on feedback that we receive. Do not use this API in a production environment.

Use this to get the buffer in basis points between offers from your marketplace contract.

## Example

```javascript
const { data: auctionWinner, isLoading, error } = useBidBuffer(<YourMarketplaceContractInstance>);
```

**Signature:**

```typescript
export declare function useBidBuffer(
  contract: RequiredParam<Marketplace>,
): import("@tanstack/react-query").UseQueryResult<BigNumber, unknown>;
```

## Parameters

| Parameter | Type                                                         | Description                           |
| --------- | ------------------------------------------------------------ | ------------------------------------- |
| contract  | [RequiredParam](./react.requiredparam.md)&lt;Marketplace&gt; | an instance of a marketplace contract |

**Returns:**

import("@tanstack/react-query").UseQueryResult&lt;BigNumber, unknown&gt;

a response object that includes an array of listings
