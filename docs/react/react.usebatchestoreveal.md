---
slug: /react.usebatchestoreveal
title: useBatchesToReveal() function
hide_title: true
displayed_sidebar: react
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## useBatchesToReveal() function

**Signature:**

```typescript
export declare function useBatchesToReveal<TContract extends NFTContract>(
  contract: RequiredParam<TContract>,
): import("@tanstack/react-query").UseQueryResult<
  import("@thirdweb-dev/sdk/dist/browser").BatchToReveal[],
  unknown
>;
```

## Parameters

| Parameter | Type                                                       | Description                                            |
| --------- | ---------------------------------------------------------- | ------------------------------------------------------ |
| contract  | [RequiredParam](./react.requiredparam.md)&lt;TContract&gt; | an instance of a [NFTContract](./react.nftcontract.md) |

**Returns:**

import("@tanstack/react-query").UseQueryResult&lt;import("@thirdweb-dev/sdk/dist/browser").BatchToReveal\[\], unknown&gt;

a response object that gets the batches to still be revealed