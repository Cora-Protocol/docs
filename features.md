---
description: Here we describe the main features of the Cora Protocol
---

# Features

**Capital Efficient**

One of the main features of the Cora protocol is its capital efficiency. \
\
Liquidity providers simply deposit stablecoins in the Lending pools. Version 1 of the protocol has unique Lending pools per pair of assets. For instance, the pool **stETH-USDC** would accept stETH as collateral and offer loans in USDC.&#x20;

Version 2 of the protocol allows **multi-collateral Lending pools**, where a single Lending pool will be able to accept a whole family of collateral types, for instance, stETH, cbETH, RETH, ETH, WETH, ERC-4626s and offer loans in USDC or any other selected stablecoins.

One single pool of liquidity is used to offer loans of multiple durations and multiple LTVs. This has great benefits since there is **NOT** liquidity fragmentation.

**Community-owned**

The Cora protocol is fully community-owned. Our goal is to design native economic mechanisms that will incentivise multiple participants to support and benefit from the protocol's success.

**Immutable**

The Cora protocol smart contracts are **NON-upgradeable**, which means the protocol rules are fully written in code.&#x20;

**Permissionless**&#x20;

In the first version of the Cora protocol, the Cora DAO is the only entity that can create Lending pools. However, we expect the community to remove this restriction and allow any party to create Liquidity pools in a permissionless fashion according to their risk appetite since they will be able to configure different parameters like:

* LTV
* Collateral type
* Stablecoin type
* Price model&#x20;

**Modular Pricing models**

Lending pools can have associated any of the whitelisted price models. This modularity feature will allow the creation of new types of products on top of Cora.&#x20;

We predict that once the DAO enables permissionless pool creation, this will allow anybody to create their own Lending pools with custom price models.

**Decentralized Pricing models**&#x20;

The Cora Protocol will allow any external participant to propose new pricing models in the protocol. Proposed pricing models will be voted on via governance and will be awarded **1% of the total protocol fees** for the lifetime of their pricing model if the performance of the Lending pool is positive.

We expect quantitative finance analysts, financial engineers, and any other participant to propose different pricing models that can help the overall health of the system and benefit Borrowers, Liquidity Providers, and the Cora Protocol.&#x20;



