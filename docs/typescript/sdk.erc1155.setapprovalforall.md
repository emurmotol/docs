---
slug: /sdk.erc1155.setapprovalforall
title: Erc1155.setApprovalForAll property
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# Erc1155.setApprovalForAll property

Set approval for all NFTs

## Example

```javascript
const operator = "{{wallet_address}}";
await contract.erc1155.setApprovalForAll(operator, true);
```

**Signature:**

```typescript
setApprovalForAll: {
        (operator: string, approved: boolean): Promise<Omit<{
            receipt: ethers.providers.TransactionReceipt;
            data: () => Promise<unknown>;
        }, "data">>;
        prepare: (operator: string, approved: boolean) => Promise<Transaction<Omit<{
            receipt: ethers.providers.TransactionReceipt;
            data: () => Promise<unknown>;
        }, "data">>>;
    };
```

## Remarks

Approve or remove operator as an operator for the caller. Operators can call transferFrom or safeTransferFrom for any token owned by the caller.