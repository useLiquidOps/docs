# The LiquidOps Auction Model

<figure><img src="../.gitbook/assets/liquidops auction model.png" alt=""><figcaption></figcaption></figure>

### LiquidOps Auction Model

Liquidations possess a key role in DeFi protocols. They are fundamental elements of the protocol’s operation, because they ensure that loans without enough collateral are repaid as quickly as possible.&#x20;

Successful liquidations require competition between liquidators so debts can be settled quickly and efficiently.&#x20;

Let’s see how this process works for LiquidOps!

### Discounted Auction for Liquidations

To make liquidators act fast and handle numerous liquidations, we use an auction model for liquidatable positions.&#x20;

This model works by offering a predetermined percentage discount compared to the market price – in our case, 5% – at the moment the liquidation is detected. This way, liquidators can acquire tokens at a lower price.

### Time-Based Dutch Auction Mechanism

To encourage fast liquidation, the auction model decreases the discount percentage linearly over a set period, until the discount reaches 0%. This ensures that liquidators compete to settle the debt as quickly as possible.&#x20;

It is worth noting that larger protocols typically use a "Dutch auction" model, which starts with a high liquidation bonus that gradually decreases over time until a buyer steps in.
