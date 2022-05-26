# Lending Pools

#### Introduction

Lending pools in Cora are single asset pools of **stablecoins**, where users or **Liquidity Providers** deposit any of the supported stablecoin **** tokens in exchange of a Cora LP token that represents the share of the pool.

Lending Pools serve as a source of liquidity for loans. Borrowers will lock their collateral in exchange for a stablecoin token that will be taken from the lending pool reserves.

![](<../.gitbook/assets/Artboard 1@2x.png>)

**Borrowing Fees**

The Cora protocol is an interest free lending platform, however every time a borrower takes a loan, it is required to pay a one time [Borrowing Fee](borrowing-fees.md). The borrowing fees go to the liquidity providers and are distributed proportionally to the liquidity provider's share of the lending pool.

Lending pools have associated a Borrowing Fee Calculator smart contract that can be changed via governance. The Borrowing fee calculator is based on [Option Pricing Models](pricing-models/) and has the goal of calculating what is the right amount that a liquidity provider should charge for the risk of providing a loan.&#x20;

For more information about how borrowing fees are calculated, see the [Borrowing Fees](borrowing-fees.md) section.

![Borrowing Fee Calculator](<../.gitbook/assets/Architecture Simple - Copy of Pool.jpg>)

#### &#x20;Multiple Liquidity Pools

The [Cora Protocol design](../developer/contract-architecture.md) supports the creation of multiple Pools**,** each Pool has associated a  collateral and a stablecoin.

Liquidity Pools have the following naming convention:

> **\[Stablecoin]-\[Collateral]**

For example a Liquidity Pool called:

> **USDC-ETH**

means, the Liquidity Pool accepts USDC deposits, and borrowers can get USDC loans using ETH as collateral.

The initial release of the protocol will only support ETH as a collateral and USDC stablecoins for liquidity provision.

**Pool Strategy**

All Liquidity Pools have a borrowing strategy associated. The strategy will define what is the maximum amount of Stablecoins that the borrowers can borrow based in the different types of collateral.

The strategy uses quantitative finance analysis methods and incorporates in its analysis external market conditions and variables like implied volatility to define a general pool collateralization ratio.

The main goal of the strategy is define a set of parameters that have the goal of maximising the risk-reward relationship based on quantitative financial theory, that is backtested and adaptable.&#x20;

![](<../.gitbook/assets/Architecture Simple - Copy of Pool (1).jpg>)

For more information about the Risk Management, please check the [Risk Management](risk-management.md) section.

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

Each Liquidity Pool can have a different Borrowing Fee Calculator, this Borrowing Fee calculated is mostly known in the traditional Options world as a Price Model, this price model can be changed and upgraded via governance (see the [Pricing Models](pricing-models/) section for more details).

#### **Risks**

As in any other system where users provide liquidity, there are risks inherent of the nature of a decentralized system, like hacks or black swan events that could make the markets crash.

However, we have worked in trying to minimise them, by auditing our code (see [Audits](../security/audits.md) section), defining procedures for contingency and unexpected situations and by having a Risk Management framework that has been backtested and simulated (see the [Risk Management ](risk-management.md)section for more details).&#x20;

****

****
