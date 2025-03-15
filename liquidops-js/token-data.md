# Token data

Access supported token data

```typescript
import { tokenData, tokens, oTokens, controllers } from "liquidops";
```

Get token details

```typescript
const qarData = tokenData.QAR;
/* {
    name: "Quantum Arweave",
    ticker: "QAR", 
    address: "XJYGT9...",
    oTicker: "oQAR",
    oAddress: "CbT2b...",
    controllerAddress: "vYlv6...",
    // ...other metadata
} */
```

Get base token addresses

```typescript
const tokenAddress = tokens.QAR; // "XJYGT9..."
```

Get oToken addresses

```typescript
const oTokenAddress = oTokens.oQAR; // "CbT2b..."
```

Get controller addresses

```typescript
const controllerAddress = controllers.QAR; // "vYlv6..."
```

Helper function to resolve token addresses and related data

```typescript
import { tokenInput, type TokenInput } from "liquidops";
```

Can use either ticker or address

```typescript
const resolved = tokenInput("QAR");
```

Or

```typescript
const resolved = tokenInput("XJYGT9ZrVdzQ5d7FzptIsKrJtEF4jWPbgC91bXuBAwU");

/* Returns:
{
  tokenAddress: "XJYGT9...",    // Base token address
  oTokenAddress: "CbT2b...",    // oToken address
  controllerAddress: "vYlv6..." // Controller contract address
}
*/
```

Currently supported tokens: QAR (Test Quantum Arweave), STETH (Test Staked Ethereum), USDC (Test USD Circle)
