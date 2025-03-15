# Protocol data functions

Get all positions

```typescript
const getAllPositions = await client.getAllPositions({
  token: "QAR",
});
```

Get historical APR

```typescript
const getHistoricalAPR = await client.getHistoricalAPR({
  token: "QAR",
});
```

Get liquidations

```typescript
const getLiquidations = client.getLiquidations({
  token: "QAR",
});
```
