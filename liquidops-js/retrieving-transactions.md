# Retrieving transactions

Get transactions for a specific token and action

```typescript
const getTransactions = await client.getTransactions({
  token: "QAR",
  action: "lend", // "lend" | "unLend" | "borrow" | "repay";
  walletAddress: "psh5nUh3VF22Pr8LeoV1K2blRNOOnoVH0BbZ85yRick",
});
```
