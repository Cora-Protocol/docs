---
description: Learn how rounds work in the Cora Protocol
---

# Rounds

Lending pools run perpetually, they are unstoppable and immutable.

A good analogy for a Lending pool is a bus, a bus needs gasoline or maybe electricity but it requires a source of energy in order to be able to work.&#x20;

In the same way, Lending pools require liquidity to be able to provide loans to borrowers.

Once the bus starts its journey, it has to stop in multiple stations and people leave the bus, while others join. One thing to keep in mind is that people in the bus will always signal that they want to stop in the next station and people who want to take the bus, will signal they want to take the bus.

\<todo Image of lending pool>&#x20;

In the same way, Lending pools in Cora allow users to signal their deposits and withdrawals but they are only able to enter in the next round. While this has impact in the user experience, it has some benefits from the implementation point of view. Since in Cora, rewards and defaulted loans are calculated properly at the end of each round.&#x20;

This mechanism prevents also liquidity providers who want to exit if the pool is underperforming, which can create dynamics where the faster liquidity providers will exit faster than the others.

The version 1 of the Cora protocol defines rounds of 28 days. This means liquidity providers have to commit their liquidity till the end of the round, in other words for at least 28 days.

The life cycle of a Lending pool is as follows:

\<todo Image of lending pool>&#x20;









