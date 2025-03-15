# oToken data functions

Get APR for a token

```typescript
const getAPR = await client.getAPR({
  token: "QAR",
});
```

Get balances

```typescript
const getBalances = await client.getBalances({
  token: "QAR",
});
```

Get token info

```typescript
const getInfo = await client.getInfo({
  token: "QAR",
});
```

Get position for a address

```typescript
const getPosition = await client.getPosition({
  token: "QAR",
  recipient: "psh5nUh3VF22Pr8LeoV1K2blRNOOnoVH0BbZ85yRick",
});
```

Get price for quantity

```typescript
const getPrice = await client.getPrice({
  token: "QAR",
  quantity: 1n,
});
```

Get reserves

```typescript
const getReserves = await client.getReserves({
  token: "QAR",
});
```
