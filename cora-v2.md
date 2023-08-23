---
description: Learn about the latest Cora protocol features
---

# 🆕 Cora V2

Cora v2 is an enhanced version of Cora v1. Same benefits, more possibilities and a more scalable and robust architecture. You can check our initial announcement [here](https://medium.com/coraprotocol/the-future-of-cora-introducing-cora-v2-4aa7f4d0c1f).

TLDR;

* In Cora v2, lenders can create and customise their own lending pools, this means lenders can select what collaterals they want to accept, the LTV per collateral, max loan duration and how much lenders want to charge for their stablecoins.
* For borrowers, Cora v2 offers more flexible loan durations, no liquidations, fixed terms, fixed rates, no bullshit.

Let's deep dive into Cora v2 and why we believe is a game changer.

### V2 Features

#### Custom Pools

Cora v2 introduces a new base layer where anybody can create their own lending pools. We see Cora v2 as a new Defi primitive for fixed terms, fixed rates money markets.

These new pools are fully customisable. Lenders can create their own lending pools and choose:

* What collaterals they want to accept (maximum 10 collaterals per pools)
* Maximum LTV and loan duration (customised per collateral)
* What pricing model they want to use to price their loans

#### **Flexible loan durations**

The version 2 of Cora maintains the same benefits as Cora v1. Users can borrow stablecoins for a fixed period of time and only pay a one-time borrowing fee **without the risk of being liquidated.**

However, the duration of the loans now is more flexible. In Cora v1 users were able to borrow up to a maximum of 30 days if they were able to borrow in the first day of the round.

In Cora v2 loans have flexible loan durations up to 1 year. Although the current testnet supports only a maximum of 90 days. The capability to borrow for 1 year is possible.

<figure><img src=".gitbook/assets/Screenshot 2023-08-23 at 09.18.03.png" alt="" width="375"><figcaption><p>Improved borrower experience</p></figcaption></figure>

#### **Simplified UI**&#x20;

Cora V2 introduces a new borrowing experience with a UI style similar to Uniswap. Borrowers simply define the collateral they want to lock, the amount to borrow, the loan duration and you are set !

This new user experience is thanks to our new modular architecture that includes a router engine that helps borrowers find the best rates across all the lending pools in the Cora universe.

#### Router Engine

The router engine is a modular architectural element of the new Cora protocol. The routing engine outsources liquidity from all the lending pools in the Cora universe and is flexible enough to also find liquidity across other sources like connecting off chain market makers who are willing to lend in the Cora protocol.

