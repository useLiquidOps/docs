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

Get exchange rate

```typescript
const getExchangeRate = await client.getExchangeRate({
  token: "QAR",
});
```

Get global position

```typescript
const getGlobalPosition = await client.getGlobalPosition({
  walletAddress: "psh5nUh3VF22Pr8LeoV1K2blRNOOnoVH0BbZ85yRick"
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
