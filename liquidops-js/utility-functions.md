# Utility functions

Get balance

```typescript
const getBalance = await client.getBalance({
  token: "XJYGT9ZrVdzQ5d7FzptIsKrJtEF4jWPbgC91bXuBAwU",
  walletAddress: "psh5nUh3VF22Pr8LeoV1K2blRNOOnoVH0BbZ85yRick",
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

Get result

```typescript
const getResult = await client.getResult({
  transferID: "0RY-eSVV156qxyuHBs3GPO2pwsIvmA-yI1oKS1ABSyI",
  tokenAddress: "XJYGT9ZrVdzQ5d7FzptIsKrJtEF4jWPbgC91bXuBAwU",
  action: "lend", // "lend" | "unLend" | "borrow" | "repay";
});
```
