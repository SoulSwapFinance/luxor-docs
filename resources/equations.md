---
description: It's not as tough as it looks, give it a try and understand how we operate.
---

# Equations

## Staking

$$
deposit = withdrawal
$$

Swaps between **LUX** and **LUMens** during staking and unstaking are always honored 1:1. The amount of **LUX** deposited into the staking contract will always result in the same amount of **LUMens**. And the amount of **LUMens** withdrawn from the staking contract will always result in the same amount of **LUX**.

$$
rebase = 1 - ( LUXDeposits / LUMens
Outstanding )
$$

The treasury deposits **LUX** into the distributor. The distributor then deposits **LUX** into the staking contract, creating an imbalance between **LUX** and **LUMens**.&#x20;

**LUMens** are rebased to correct this imbalance between **LUX** deposited and **LUMens** outstanding. The rebase brings **LUMens** outstanding back up to parity so that 1 **LUMens** equals 1 staked **LUX**.

## Minting

Minting happens by allowing users to purchase a bond. This bond price is the Mint price.

$$
bond Price = 1 + Premium
$$

**LUX** has an intrinsic value of **1 DAI**, which is roughly equivalent to $1. In order to make a profit from minting, **Luxor** charges a premium for each minting action.

$$
Premium = debt Ratio * BCV
$$

The premium is derived from the debt ratio of the system and a scaling variable called BCV. BCV allows us to control the rate at which bond prices increase.

The premium determines profit due to the protocol and in turn, stakers. This is because new **LUX** is minted from the profit and subsequently distributed among all stakers.

$$
debt Ratio = bondsOutstanding/LUXSupply
$$

The debt ratio is the total of all **LUX** promised to bonders divided by the total supply of **LUX**. This allows us to measure the debt of the system.

$$
bondPayout_{reserveBond} = marketValue_{asset}\ /\ bondPrice
$$

Bond payout determines the number of **LUX** sold to a minter.&#x20;

For reserve mints, the market value of the assets supplied by the minter is used to determine the bond payout.&#x20;

For example, if a user supplies **1000 DAI** and the mint price is **250 DAI**, the user will be entitled 4 **LUX**.

$$
bondPayout_{lpBond} = marketValue_{lpToken}\ /\ bondPrice
$$

For liquidity mints, the market value of the LP tokens supplied by the minter is used to determine the bond payout. For example, if a user supplies **0.001 LUX-FTM LP token** which is valued at **1000 DAI** at the time of bonding, and the bond price is **250 DAI**, the user will be entitled 4 **LUX**.&#x20;

## **LUX** Supply

$$
LUX_{supplyGrowth} = LUX_{stakers} + LUX_{bonders} + LUX_
{DAO}
$$

**LUX** supply does not have a hard cap. Its supply increases when:

* **LUX** is minted and distributed to the stakers.
* **LUX** is minted for the bonder. This happens whenever someone purchases a bond.
* **LUX** is minted for the DAO. This happens whenever someone purchases a bond. The **DAO** gets the same number of **LUX** as the bonder.

$$
LUX_{stakers} = LUX_{totalSupply} * rewardRate
$$

At the end of each epoch, the treasury mints **LUX** at a set reward rate. These **LUX** will be distributed to all the stakers in the protocol.&#x20;

$$
LUX_{bonders} = bondPayout
$$

Whenever someone purchases a bond, a set number of **LUX** is minted.&#x20;

These **LUX** will not be released to the minter all at once - they are vested to the bonder linearly over time.&#x20;

The bond payout uses a different formula for different types of bonds.&#x20;

Check the Minting section above to see how it is calculated.

$$
LUX_{DAO} = LUX_{bonders}
$$

The DAO receives the same amount of **LUX** as the minter. This represents the **DAO profit**.

## Backing per LUX

$$
LUX_{backing} = treasuryBalance_{stablecoin} + treasuryBalance_{otherAssets}
$$

Every **LUX** in circulation is backed by the **Luxor** treasury.&#x20;

The assets in the treasury can be divided into two categories: stable coin and non-stable coin.

$$
treasuryBalance_{stablecoin} = BackingPerLUX_{reserveBond} + BackingPerLUX_{lpBond}
$$

The stable coin balance in the treasury grows when bonds are sold. Backing per **LUX** is calculated differently for different mints types.

$$
BackingPerLUX_{reserveBond} = assetSupplied
$$

For reserve mints such as **DAI** minting, the Backing per **LUX** simply equals to the amount of the underlying asset supplied by the minter.

$$
BackingPerLUX_{lpBond} = 2sqrt(constantProduct) * (\%\ ownership\ of\ the\ pool)
$$

For LP Mints such as **LUX-FTM Minting**, their backing per **LUX** is calculated differently because the protocol needs to mark down its value.&#x20;

_Why?_ The LP token pair consists of **LUX**, and each **LUX** in circulation will be backed by these LP tokens - there is a cyclical dependency. To safely guarantee all circulating **LUX** are backed, the protocol marks down the value of these LP tokens.
