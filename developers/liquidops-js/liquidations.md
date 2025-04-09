# Liquidations

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

<pre class="language-typescript"><code class="lang-typescript"><strong>const liquidate = client.getLiquidations();
</strong></code></pre>

Get discounted quantity

```typescript
const getDiscountedQuantity = client.getDiscountedQuantity({
  liquidated,
  rewardToken,
  qualifyingPosition,
  priceData,
  validateMax: false // Optionally validate the liqidated token quantity and the discounted quantity. This will throw an error if any of these quantities are more than what the user holds.
});
```
