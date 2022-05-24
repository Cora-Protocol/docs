---
description: >-
  Learn more about the Risk Management Strategy of each of the Cora Liquidity
  Pools
---

# Risk Management

The Cora protocol divides its risk management overall strategy into 2 parts.

**1) Maximum percentage to borrow / collateral ratio selection**

What is the optimal collateral ratio for a certain asset?

By defining an optimal collateral ratio, the protocol adds a layer of protection to Liquidity Providers. Since it will limit the amounts that borrowers can borrow.

In order to find the optimal value, the Cora protocol performs the following steps.

1.  Every epoch, which last 30 days, the Pool Manager analyses historical data about the behaviour of a particular collateral asset. i.e ETH.

    \<TODO> Include historical data chart of ETH.
2.  Based on the historical data analysis, it will define a maximum percentage that every Liquidity Pool should allow to borrow for a particular asset. This analysis will consider the observed volatility and historical price declines.  &#x20;

    For example, it can define that the USDC-ETH Liquidity Pool can allow loans up to 80% of the collateral value at borrowing time.
3. The Pool Manager will perform a backtesting strategy to analyse the behaviour of the Cora protocol under the conditions specified in the previous step and it will conclude if the strategy is safe to execute.
4. The Pool Manager will publish the results and propose parameters changes if required.
5. The community analyse and vote the proposal.

**2) Pricing Model selection**

Which Pricing Model should the Liquidity Pool use?

Selecting the right Pricing Model for a particular Liquidity Pool is important because it will estimate properly what is the right Borrowing Fee that Liquidity Providers should charge for the risk of providing a loan.

...coming soon





