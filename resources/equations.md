---
description: It's not as tough as it looks, give it a try and understand how we operate.
---

# Equations

## Staking // Rebasing

$$
deposit = withdrawal
$$

Swaps between **LUX** and **LUM** during deposits and withdrawals are always honored 1:1. The amount of **LUX** deposited will always result in the same amount of **LUM**. The amount of **LUM** withdrawn from the staking contract will always result in the same amount of **LUX**.

$$
rebase = 1 - ( LUX_D / LUM _O)
$$

The treasury deposits **LUX** into the distributor. The distributor then deposits **LUX** into the staking contract, creating an imbalance between **LUX** and **LUM**.

**LUM** is rebased to correct this imbalance between **LUX** deposited (_**d**_) and **LUM** outstanding (_**o**_). The rebase brings **LUM** outstanding back up to parity so that 1 **LUM** equals 1 staked **LUX**.

## Circulating Supply

**Circulating Supply** is equal to total **LUX** minted, minus the total balance of Luxor stored as collateral for **SOR** (**s**), our stable coin.

$$
circulating = total - backing_s
$$

## Minting and Bond Price

Minting enables users to purchase bonds. This bond price is the mint price.

$$
bond Price = 1 + Premium
$$

**LUX** has an intrinsic value of **1 USD** (not to be confused by **backing** as defined below), which is roughly equivalent to $1. In order to make a profit from minting, **Luxor** charges a premium for each minting action.

$$
Premium = debt Ratio * BCV
$$

The **premium** is derived from the debt ratio of the system and a scaling variable called **BCV**.

**BCV** allows us to control the rate at which bond prices increase.

The **premium** determines profit due to the protocol and in turn, stakers. This is because new **LUX** is minted from the profit and subsequently distributed among all stakers.

$$
debt Ratio = bondsOutstanding/LUXSupply
$$

The debt ratio is the total of all **LUX** promised to bonders divided by the total supply of **LUX**. This allows us to measure the debt of the system.

$$
bondPayout_{reserveBond} = marketValue_{asset}\ /\ bondPrice
$$

Bond payout determines the number of **LUX** sold to a minter.

For reserve mints, the market value of the assets supplied by the minter is used to determine the bond payout.

For example, if a user supplies **1000 DAI** and the mint price is **250 DAI**, the user will be entitled 4 **LUX**.

$$
bondPayout_{lpBond} = marketValue_{lpToken}\ /\ bondPrice
$$

For liquidity mints, the market value of the LP tokens supplied by the minter is used to determine the bond payout. For example, if a user supplies **0.001 LUX-FTM LP token** which is valued at **1000 DAI** at the time of bonding, and the bond price is **250 DAI**, the user will be entitled 4 **LUX**.

## **Luxor** Supply

$$
LUX_{supplyGrowth} = LUX_{stakers} + LUX_{bonders} + LUX_ {DAO}
$$

**LUX** supply does not have a hard cap. Its supply increases when:

* **LUX** is minted and distributed to **LUM** holders (those staking LUX).
* **LUX** is minted for the bonder. This happens whenever a bond is purchased.
* **LUX** is minted for the DAO.&#x20;
  * This happens whenever someone purchases a bond with a tax fee.

$$
LUX_{stakers} = LUX_{totalSupply} * rewardRate
$$

At the end of each epoch, the treasury mints **LUX** at a set reward rate. These **LUX** will be distributed to those staking in the protocol.

$$
LUX_{bonders} = bondPayout
$$

Whenever someone purchases a bond, a set number of **LUX** is minted.

These **LUX** will not be released to the minter all at once - they are vested to the bonder linearly over time.

The bond payout uses a different formula for different types of bonds.

Check the Minting section above to see how it is calculated.

$$
LUX_{DAO} = LUX_{bonders}
$$

The DAO receives the same amount of **LUX** as the minter. This represents the **DAO profit**.

## **Backing Price (Price Floor)**

$$
Price Floor = Reserves / Supply_c
$$

Treasury assets may be divided into two categories: **reserves and liquidity.**&#x20;

Unlike other reserve currencies, **Luxor DAO guarantees a defendable price floor**, which is determined by the equation above, where the floor equals the value of the protocol's reserves divided by the circulating (_**c**_) supply.

The intuition here is for each dollar value in our reserves, we are able to cover the circulating supply at a floating price floor.&#x20;

_Reserves_ are stated in the Dashboard and equal to the following:

$$
Reserves = DAI_b + (FTM_b * FTM_p)
$$

Where _b_ is the balance held in the Treasury and _p_ is the asset price.
