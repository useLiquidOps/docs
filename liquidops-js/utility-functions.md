# Utility functions

Get balance

```typescript
const getBalance = await client.getBalance({
  tokenAddress: "XJYGT9ZrVdzQ5d7FzptIsKrJtEF4jWPbgC91bXuBAwU",
  walletAddress: "psh5nUh3VF22Pr8LeoV1K2blRNOOnoVH0BbZ85yRick",
});
```

Get result

```typescript
const getResult = await client.getResult({
  transferID: "0RY-eSVV156qxyuHBs3GPO2pwsIvmA-yI1oKS1ABSyI",
  tokenAddress: "XJYGT9ZrVdzQ5d7FzptIsKrJtEF4jWPbgC91bXuBAwU",
  action: "lend", // "lend" | "unLend" | "borrow" | "repay";
});
```

Transfer tokens

```typescript
const transfer = await client.transfer({
  token: "QAR",
  recipient: "psh5nUh3VF22Pr8LeoV1K2blRNOOnoVH0BbZ85yRick",
  quantity: 1n,
});
```
