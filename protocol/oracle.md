# Oracle

LiquidOps uses a instance of the [Redstone](https://www.redstone.finance/) pull oracle on AO.&#x20;

Oracle process ID: R5rRjBFS90qIGaohtzd1IoyPwZD0qJZ25QXkP7\_p5a0

You can via Oracle messages via ao.link [here](https://www.ao.link/#/entity/R5rRjBFS90qIGaohtzd1IoyPwZD0qJZ25QXkP7_p5a0?tab=incoming)

```json
// Example oracle message to the controller

{
  "AR": {
    "verifiedPackage": {
      "v": 5.10010259,
      "t": 1744749890000
    }
  },
  "qAR": {
    "verifiedPackage": {
      "v": 5.10010259,
      "t": 1744749890000
    }
  },
  "USDC": {
    "verifiedPackage": {
      "v": 1.00000612,
      "t": 1744749890000
    }
  },
  "wUSDC": {
    "verifiedPackage": {
      "v": 1.00000612,
      "t": 1744749890000
    }
  }
}
```
