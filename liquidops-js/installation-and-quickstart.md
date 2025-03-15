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
@permaweb/aoconnect <= 0.0.77
```

&#x20;Required peer dependencies for LiquidOps JS
{% endhint %}

Here's a simple lending example to get you started:

```typescript
import LiquidOps from "liquidops";
import { createDataItemSigner } from "@permaweb/aoconnect";

const signer = createDataItemSigner(window.arweaveWallet);

const client = new LiquidOps(signer);

const lend = await client.lend({
  token: "QAR",
  quantity: 1n,
});

console.log(lend)
```
