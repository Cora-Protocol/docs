---
description: Learn more about Lending Pools in the Cora Protocol
---

# Lending Pools

#### Introduction

**Lending pools** in Cora are single asset pools of **stablecoins**, where users or **liquidity providers** deposit any of the supported stablecoin **** tokens in exchange of a Cora LP token that represents the share of the pool.

Lending pools serve as a source of liquidity for loans. Borrowers will lock their collateral in exchange for a stablecoin token that will be taken from the lending pool reserves.

<figure><img src="../../.gitbook/assets/lending-pools-white@2x.png" alt=""><figcaption></figcaption></figure>

**Borrowing Fees**

Every time a borrower takes a loan, it is required to pay a one time **borrowing fee.**

The borrowing fees go to the liquidity providers and are distributed proportionally to the liquidity provider's share of the lending pool.

Lending pools have associated a **** [Price model](../pricing-models/) **** smart contract that can be changed via governance.&#x20;

\<TODO> pool con multiple price models

decir que estan basados en options price models pero que puede ser cualquier cosa

These models are based on Option's pricing models and calculates what is the right amount that a liquidity provider should charge to the borrower for the risk of providing a non liquidatable loan.&#x20;

For more information about how borrowing fees are calculated, see the [Borrowing Fees](../borrowing-fees.md) section.

![Borrowing Fee Calculator](<../../.gitbook/assets/borrowingFeeCalculator@2x (1).png>)

**Lending Pool Strategy**

All lending pools have a borrowing strategy associated. The strategy will define what is the maximum amount of stablecoins that the borrowers can borrow based in the different types of collateral.

The strategy uses quantitative finance analysis methods and incorporates in its analysis external market conditions and variables like implied volatility to define a general **loan to value (LTV).**

The main goal of the strategy is define a set of parameters that have the goal of maximising the risk-reward relationship based on quantitative financial theory, that is backtested and adaptable.&#x20;

![](<../../.gitbook/assets/Architecture Simple - Copy of Pool (1).jpg>)

For more information about the Risk Management, please check the [Risk Management](../risk-management.md) section.

#### **Pool Parameters**

_Collateral_

The collateral that the Liquidity Pool will accept in order to provide a loan.

_Stablecoin_

The Stablecoin that the Liquidity Pool will accept as liquidity and to offer a loan.

_Maximum percentage to borrow_

The Pool Strategy will define what is the maximum amount of Stablecoins that the borrowers can borrow based in the different types of collateral.

For example:

Using ETH as collateral, the system can define a maximum percentage to borrow of 80%&#x20;

Then a user can borrow up to 80% of their ETH spot price at borrowing time.

_Borrowing Fee Calculator_

Each Liquidity Pool can have a different Borrowing Fee Calculator, this Borrowing Fee calculated is mostly known in the traditional Options world as a Price Model, this price model can be changed and upgraded via governance (see the [Pricing Models](../pricing-models/) section for more details).

#### **Risks**

As in any other system where users provide liquidity, there are risks inherent of the nature of a decentralized system, like hacks or black swan events that could make the markets crash.

However, we have worked in trying to minimise them, by auditing our code (see [Audits](../../security/audits.md) section), defining procedures for contingency and unexpected situations and by having a Risk Management framework that has been backtested and simulated (see the [Risk Management ](../risk-management.md)section for more details).&#x20;

****

****
