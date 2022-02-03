# Monetary Policies

**​**[**Luxor**](https://app.luxor.money) features policy constants that allow us to optimize the system.

## Bonds <a href="#bonds" id="bonds"></a>

Every time a user Mints LUX on Luxor, they are actually purchasing a **bond**.&#x20;

These "Bonds" have different parameters, including the **BCV,** which allows us to scale the rate at which bond premiums increase. A higher BCV means a lower discount for bonders and more protocol profit. A lower BCV means a higher discount for bonders and less protocol profit.

The **vesting term** determines how long it takes for bonds to become fully redeemable. A longer term means lower inflation and lower bond demand.

## Sales <a href="#sales" id="sales"></a>

The **DCV** allows us to scale protocol buy pressure up or down. A higher DCV means more buy pressure and higher deflation. A lower DCV means less buy pressure and a weaker floor.

## Treasury <a href="#treasury" id="treasury"></a>

Profit allocations are the only treasury variable. This allows us to choose who receives profits from the protocol.

## Staking <a href="#staking" id="staking"></a>

There are no variables in the staking contract. **LUX** and **LUMens** are always redeemable 1:1, and profits are always distributed equally through rebase.

## Buy-Back Policy <a href="#staking" id="staking"></a>

In the interest of maintaining our backing (floor) price, we are instituting a policy that enables the treasury to buy back LUXOR off the market to store in the DAO and burn (50/50). This policy will take place any time the market price falls within a non-specific threshold. This threshold is intentionally unannounced in an attempt to prevent bad actors from manipulating the process to their benefit.&#x20;
