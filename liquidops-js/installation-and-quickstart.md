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
ao-tokens >= 0.0.6
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

You can also add optional custom configurations to the SDK:

```typescript
const client = new LiquidOps(signer, {
    GATEWAY_URL: "",
    GRAPHQL_URL: "",
    GRAPHQL_MAX_RETRIES: "",
    GRAPHQL_RETRY_BACKOFF: "",
    MU_URL: "",
    CU_URL: ""
});
```

Declare LiquidOps class in node environments:

```typescript
import { createDataItemSigner } from "@permaweb/aoconnect/dist/client/node/wallet";
import LiquidOps from "liquidops";

const signer = createDataItemSigner(window.arweaveWallet);

const client = new LiquidOps(signer);
```

Here's a simple lending example to get you started:

```typescript
import { createDataItemSigner } from "@permaweb/aoconnect/dist/client/node/wallet";
import LiquidOps from "liquidops";

const signer = createDataItemSigner(window.arweaveWallet);

const client = new LiquidOps(signer);

const lend = await client.lend({
  token: "QAR",
  quantity: 1n,
});

console.log(lend)
```
