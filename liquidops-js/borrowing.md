# Borrowing

Borrow tokens

```typescript
const borrow = await client.borrow({
  token: "QAR",
  quantity: 1n,
});
```

Repay borrowed tokens

```typescript
const repay = await client.repay({
  token: "QAR",
  quantity: 1n,
});
```
