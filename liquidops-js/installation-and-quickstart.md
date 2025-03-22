# Installation & quickstart

You can install the LiquidOps JS using npm:

```
npm i liquidops
```

Or using yarn:

```
yarn add liquidops
```

Or using bun:

```
bun i liquidops
```

{% hint style="warning" %}
```
@permaweb/aoconnect >= 0.0.77
ao-tokens >= 0.0.5
```

Required peer dependencies for LiquidOps JS
{% endhint %}

Declare LiquidOps class in node environments:

```typescript
import { createDataItemSigner } from "@permaweb/aoconnect/dist/client/node/wallet";
import LiquidOps from "liquidops";

const JWK = `{
  "kty": "RSA",
  "e": "AQAB",
  "n": "...",
  "d": "...",
  "p": "...",
  "q": "...",
  "dp": "...",
  "dq": "...",
  "qi": "..."
}`;

const signer = createDataItemSigner(JWK);

const client = new LiquidOps(signer);
```

Declare LiquidOps class in node environments:

```typescript
import { createDataItemSigner } from "@permaweb/aoconnect";
import LiquidOps from "liquidops";

const signer = createDataItemSigner(window.arweaveWallet);

const client = new LiquidOps(signer);
```

Here's a simple lending example to get you started:

```typescript
import { createDataItemSigner } from "@permaweb/aoconnect";
import LiquidOps from "liquidops";

const signer = createDataItemSigner(window.arweaveWallet);

const client = new LiquidOps(signer);

const lend = await client.lend({
  token: "QAR",
  quantity: 1n,
});

console.log(lend)
```
