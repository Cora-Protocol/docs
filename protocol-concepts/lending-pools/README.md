---
description: Learn more about Lending Pools in the Cora Protocol
---

# Lending Pools

#### Introduction

**Lending pools** in Cora are single asset pools of **stablecoins**, where users or **liquidity providers** deposit any of the supported stablecoin tokens in exchange of a Cora LP token that represents the share of the pool.

Lending pools serve as a source of liquidity for loans. Borrowers will lock their collateral in exchange for a stablecoin token that will be taken from the lending pool reserves.

<figure><img src="../../.gitbook/assets/lending-pools-white@2x.png" alt=""><figcaption></figcaption></figure>

**Borrowing Fees**

Every time a borrower takes a loan, it is required to pay a one time **borrowing fee.**

The borrowing fees go to the liquidity providers and are distributed proportionally to the liquidity provider's share of the lending pool.

Lending pools have associated a [Price model](../pricing-models.md) smart contract that can be changed via governance.&#x20;

These models are based on Option's pricing models and calculate what is the right amount that a liquidity provider should charge to the borrower for the risk of providing a non liquidatable loan.&#x20;

For more information about how borrowing fees are calculated, see the [Borrowing Fees](../borrowing-fees.md) section.

<figure><img src="../../.gitbook/assets/multiple-price-models-white@2x (1).png" alt=""><figcaption><p>Lending pool and price models</p></figcaption></figure>

**Lending Pool Strategy**

All lending pools have a borrowing strategy associated. The strategy will define what is the maximum amount of stablecoins that the borrowers can borrow based in the different types of collateral.

The strategy uses quantitative finance analysis methods and incorporates in its analysis external market conditions and variables like implied volatility to define risk parameters in the Lending pool.

Strategies are fully backtested and are adaptable based on external factors. Their main goal is to maximise the risk-reward relationship based on quantitative financial theory and help LPs to manage their risk.

<figure><img src="../../.gitbook/assets/lending-pool-strategy@2x (1).png" alt=""><figcaption><p>Decentralized Risk Management Engine</p></figcaption></figure>

For more information about the Risk Management, please check the [Risk Management](../risk-management.md) section.

#### **Pool Parameters**

_**Collateral token**_

The collateral that the Lending pool will accept in order to provide a loan.

_**Stablecoin token**_

The stablecoin that the Lending pool will accept as liquidity and to offer a loan.

_**Max LTV**_

The Lending pool strategy will define what is the maximum amount of stablecoins that the borrowers can borrow based in the different types of collateral, we call this process maximum LTV selection.

For example:

Using ETH as collateral, the strategy can define a maximum LTV of 80%.

Then a user can borrow up to 80% of their ETH spot price at borrowing time.

_**Price model**_

Each Lending pool can have a different price model. This price model can be changed and upgraded via governance (see the [Pricing Models](../pricing-models.md) section for more details).

_**Price feed**_

At borrowing time, the Lending pool will verify the current collateral value in order to validate that the amount requested is lower than the maximum LTV. The price feed address is a Chainlink data feed for the particular collateral.

_**Minimum amount to borrow**_

Minimum amount that users should be able to borrow.&#x20;

_**Minimum amount to deposit**_

Minimum amount that liquidity providers should deposit.

_**Maximum cap**_

Maximum capacity of the Lending pool. In other words, this is the maximum amount of stablecoins that lending pools will accept as deposit. After this threshold is crossed, new deposits will be reverted.

This ensures the levels of utilization of the Lending pool stay at a level that ensures that liquidity providers keep earning competitive yields.&#x20;

_**Round duration**_

This is the duration of the round in seconds.

Rounds are a fundamental part of the life cycle of a Lending pool. We have dedicated [a section ](rounds.md)where you can learn more about its purpose and how they work.

_**Genesis round duration**_

This is the duration of the genesis round in seconds.

The genesis round is the first round in the life cycle of any Lending pool. This round automatically starts after the creation of the Lending pool.&#x20;

The goal of the genesis round is to enable the Lending pool to "load" stablecoins in its reserves. You can imagine this as the gasoline needed for a car to start.&#x20;

During the genesis round there are not restrictions of withdrawals and deposits, however once the genesis round finishes, the normal rounds will start.&#x20;

You can learn more about the life cycle of a Lending pool in [this section.](rounds.md)







