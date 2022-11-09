---
description: >-
  This roadmap aims to provide an overview of the future plans and timelines of
  the Cora Protocol
---

# Roadmap

### November 2022: Testnet launch

The Cora Protocol will release an initial version in the Goerli and Moonbase alpha network. The goal of this testnet release is to start battle-testing the protocol in a close to Mainnet environment.

**The details of this release include:**

* Supported Collateral: **cWETH (Cora WETH test token)**
* Supported Stablecoins: **cUSDC (Cora USDC test token)**
* Supported Loan Durations: **1, 7, 14, 28 days**
* Option Pricer Model: **BlackScholes**
* Rounds Duration: **1 day**
* Liquidity Cap: **No limits**

### December 2022: DAO Formation

The Cora Protocol will be a community owned protocol. Together with the community we will define the rules  and guidelines to allow any person to be part of the DAO.

### December 2022: Audit

The Cora Protocol will be audited at the end of Q4 of 2022. We will perform audits with Consensys Diligence and Zellic.

> Note: The following dates are subject to the DAO approval

### January 2023: Mainnet launch

The Cora Protocol is planned to be released to Ethereum Mainnet in January of 2022.

**The details of this release include:**

* Supported Collateral: **WETH**
* Supported Stablecoins: **USDC**
* Supported Loan Durations: **1, 7, 14, 28 days**
* Option Pricer Model: **KellyCriterion**
* Round Duration: **28 days**
* Liquidity Cap: Maximum **2 Million USDC**

### February **2023: Multi collateral lending pools**

We plan to release Lending Pools with multiple collaterals with the goal to increase the capital efficiency of the protocol. Some of the ERC20 tokens that can potentially become accepted are:

* cbETH
* stETH
* RETH

### March 2023: Cora Vaults

We will release a set of products built on top of the Cora Protocol.

* **Liquidity Mining Vault**
* **Leverage Protected Staking Vault**
* **Staking Vault**

### March 2023: Multi chain deployments

Some of the networks where the Cora Protocol is planning to deploy are:

* Moonbeam
* NEAR
* Arbitrum
* Optimism

### Areas of Interest

Some ideas that we would love to explore are:

**Any loan duration**\
****To allow users to get a loan for any duration using any of the supported collateral tokens.&#x20;

**Shared liquidity across chains**\
****Cora version 1 will have multiple instances of the protocol deployed on multiple Blockchains. However, these instances don't share liquidity. What if Cora can share liquidity across chains?

**Instant withdrawals**\
****The current version of the protocol has rounds with duration of 28 days. Which means Liquidity providers can signal to withdraw, but they have to wait for the round to finish to be able to withdraw their capital. We want to remove this barrier and allow LPs to withdraw instantly at any point.

**Permissionless pools**\
****In the first version of the protocol  the Cora DAO is the only entity that can create Lending pools, however we expect this to change via Cora DAO voting and allow any participant to deploy their own Lending pools.
