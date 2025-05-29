# Retrieving transactions

Get transactions for a specific token and action

```typescript
const getTransactions = await client.getTransactions({
  token: "QAR",
  action: "lend", // "lend" | "unLend" | "borrow" | "repay";
  walletAddress: "psh5nUh3VF22Pr8LeoV1K2blRNOOnoVH0BbZ85yRick",
});
```

Get a transactions result after it has been submitted

```typescript
const getResult = await LiquidOpsClient.getResult({
    transferID "", // the id returned from lend/borrow/unLend/repay
    tokenAddress: '', // address of the token
    action: "", // "lend" | "unLend" | "borrow" | "repay";
});
```
