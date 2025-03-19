# Liquidation

Liquidate a position

```typescript
const liquidate = client.liquidate({
  token: "QAR",
  rewardToken: "USDC",
  targetUserAddress: "psh5nUh3VF22Pr8LeoV1K2blRNOOnoVH0BbZ85yRick",
  quantity: 1n,
});
```

Get available liquidations

```typescript
const liquidate = client.getLiquidations({
  token: "QAR",
});
```
