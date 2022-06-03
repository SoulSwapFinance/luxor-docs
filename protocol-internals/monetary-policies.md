# Monetary Policies

**​**[**Luxor**](https://app.luxor.money) features policy constants that allow us to optimize the system.

## Bonds <a href="#bonds" id="bonds"></a>

Every time a user Mints LUX on Luxor, they are actually purchasing a **bond**.

These "Bonds" have different parameters, including the **BCV,** which allows us to scale the rate at which bond premiums increase. A higher BCV means a lower discount for bonders and more protocol profit. A lower BCV means a higher discount for bonders and less protocol profit.

The **vesting term** determines how long it takes for bonds to become fully redeemable. A longer term means lower inflation and lower bond demand.

## Sales <a href="#sales" id="sales"></a>

The **DCV** allows us to scale protocol buy pressure up or down. A higher DCV means more buy pressure and higher deflation. A lower DCV means less buy pressure and a weaker floor.

## Treasury <a href="#treasury" id="treasury"></a>

Profit allocations are the only treasury variable. This allows us to choose who receives profits from the protocol.

## Staking <a href="#staking" id="staking"></a>

There are no variables in the staking contract. **LUX** and **LUMens** are always redeemable 1:1, and profits are always distributed equally through rebase.

## Buy-Back Policy <a href="#staking" id="staking"></a>

In the interest of maintaining our backing (floor) price, we are instituting a policy that enables the treasury to buyback LUX off the market.\
\
This policy will take place any time the market price falls within a non-specific threshold. This threshold is intentionally unannounced in an attempt to prevent bad actors from manipulating the process to their benefit.\
\
Additionally, the exact division of the policy allocation of LUX buybacks are reflected in the resources section, under [Buyback Allocation](../resources/buyback-allocation.md) and updated on occasion. ~~As is the case with the Bond Limits~~, all updates will be immediately documented. \
\
**Please Note**: we are no longer limiting bonds, but instead enforcing a new rule (**Minimum Price Requirement**) as explained below.

### Minimum Price Requirement

All bonds are now subject to a lower bond, such that the discount of any given bond f**ollows closely with the backing price of LUX**. \
\
The motivation for this decision is due to the impact of steep-discounts that were provided on Luxor Bonds, in the past. **Long gone are the days of 50%+ discounts, thanks to this new policy**.

