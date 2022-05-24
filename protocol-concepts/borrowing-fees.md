---
description: Learn how Borrowing Fees are calculated in the Cora Protocol
---

# Borrowing Fees

Traditionally in an Options Trade, an Option buyer pays a premium for the Option he is acquiring, this premium fee is paid to the Option seller or Option writer in exchange for taking the risk of selling an Option.

Similarly, in **Cora**, a Liquidity Provider is taking a risk by offering his capital to be lent without any interest, therefore he will receive a payment that we call **Borrowing Fee.**

The **Borrowing Fee** is a one time payment made by the borrower in order to get a non-liquidatable loan. The value of the Borrowing Fee is variable and depends on the duration of the loan and the current spot price of the collateral being locked in a particular [Liquidity Pool](liquidity-pools.md).

Long term loans will have a higher borrowing fee, see in the image below how borrowing fees increase as the duration of the loan increases.

![Loan Duration vs Borrowing Fee for ETH-USDC pools](<../.gitbook/assets/Screenshot 2021-10-30 at 12.36.25.png>)

**How Borrowing Fees Are Calculated ?**

The way the Borrowing Fee is calculated depends on the [Pricing Model](pricing-models/) the Liquidity Pool is using. Since each Liquidity Pool has associated an Option Pricing Model and a collateral type, this can be slightly different, however, the shape of the curve will be of the same form.

Option Pricing models are interchangeable and upgradeable, we can have many way to calculate the Borrowing Fee. The first version of the protocol for ETH pools uses a [Black Scholes](https://www.investopedia.com/terms/b/blackscholes.asp) Pricing model.&#x20;

For more details about the pricing models, review the [Pricing Models](pricing-models/) section.
