# FAQ

## Why do we need Luxor in the first place?

Dollar-pegged stable coins have become an essential part of crypto due to their lack of volatility as compared to tokens such as Bitcoin and Ether. Users are comfortable with transacting using stable coins knowing that they hold the same amount of purchasing power today vs. tomorrow. But this is a fallacy. The dollar is controlled by the US government and the Federal Reserve. _This means a depreciation of dollar also means a depreciation of these stable coins._

Luxor aims to solve this by creating a non-pegged stable coin called **LUX**. By focusing on supply growth rather than price appreciation, Luxor hopes that **LUX** can function as a currency that is able to hold its purchasing power regardless of market volatility.

## Is LUX a stablecoin? <a href="#is-time-a-stable-coin" id="is-time-a-stable-coin"></a>

**No, LUX is not a stable coin**. Rather, **LUX** aspires to become an algorithmic reserve currency backed by other decentralized assets. Similar to the idea of the gold standard, **LUX** provides free-floating value its users can always fall back on, simply because of the fractional treasury reserves **LUX** draws its intrinsic value from.



## **LUX** is backed, not pegged. <a href="#time-is-backed-not-pegged-1" id="time-is-backed-not-pegged-1"></a>

Each **LUX** is backed by 1 **DAI**, not pegged to it. Because the treasury backs every **LUX** with at least 1 **DAI**, the protocol would buy back and burn **LUX** when it trades below 1 **DAI**. This has the effect of pushing **LUX** price back up to 1 **DAI**. **LUX** could always trade above 1 **DAI** because there is no upper limit imposed by the protocol. Think pegged == 1, while backed >= 1.

You might say that the **LUX** floor price or intrinsic value is 1 **DAI**. We believe that the actual price will always be 1 **DAI** + premium, but in the end that is up to the market to decide.

## How does it work? <a href="#how-does-it-work" id="how-does-it-work"></a>

At a high level, Luxor consists of its protocol managed treasury, protocol owned liquidity, bond mechanism (minting), and high staking rewards that are designed to control supply expansion.

Bonding in the "Mint" page generates profit for the protocol, and the treasury uses the profit to mint **LUX** and distribute them to stakers. With LP bond, the protocol is able to accumulate liquidity to ensure the system stability.

## What is the deal with (⭐, ⭐) and (🏦, 🏦)? <a href="#what-is-the-deal-with-hat-hat" id="what-is-the-deal-with-hat-hat"></a>

(⭐, ⭐) is the idea that, if everyone cooperated in Luxor, it would generate the greatest gain for everyone (from a [**game theory**](https://en.wikipedia.org/wiki/Game\_theory) standpoint). Currently, there are three actions a user can take:

* _Staking_&#x20;
* _Minting_ (_Bonding_)
* _Selling_&#x20;

Staking and minting are considered beneficiary to the protocol, while selling is considered detrimental. Staking and selling will also cause a price move, while bonding (minting) does not (we consider buying **LUX** from the market as a prerequisite of staking, thus causing a price move). If both actions are beneficiary, the actor who moves price also gets half of the benefit (+🏦). If both actions are contradictory, the bad actor who moves price gets half of the benefit (+🏦), while the good actor who moves price gets half of the downside (Ⅹ). If both actions are detrimental, which implies both actors are selling, they both get the worst possible outcome (❌)!

Thus, given two actors, all scenarios of what they could do and the effect on the protocol are shown here:

* If we both stake  (⭐,⭐), it is the best thing for both of us and the protocol (both users gets the The Mad Hatter's hat).
* If one of us stakes and the other one bonds, it is also great because staking takes **LUX** off the market and put it into the protocol, while bonding provides liquidity and **DAI** for the treasury!&#x20;
* When one of us sells, it diminishes effort of the other one who stakes or bonds.
* When we both sell, it creates the worst outcome for both of us and the protocol (❌, ❌)

## Why is PCV important? <a href="#why-is-pcv-important" id="why-is-pcv-important"></a>

As the protocol controls the funds in its treasury, **LUX** can only be minted or burned by the protocol. This also guarantees that the protocol can always back 1 **LUX** with 1 **DAI**. You can easily define the risk of your investment because you can be confident that the protocol will indefinitely buy **LUX** below 1 **DAI** with the treasury assets until no one is left to sell. You can't trust the FED but you can trust the CODE.

As the protocol accumulates more PCV, more runway is guaranteed for the stakers.&#x20;

This means the stakers can be confident that the current staking APY can be sustained for a longer term because more funds are available in the treasury.

## Why is the market price of **LUX** so volatile? <a href="#why-is-the-market-price-of-time-so-volatile" id="why-is-the-market-price-of-time-so-volatile"></a>

It is extremely important to understand how early in development the Luxor protocol is. A large amount of discussion has centered around the current price and expected a stable value moving forward. The reality is that these characteristics are not yet determined. The network is currently tuned for expansion of **LUX** supply, which when paired with the staking, minting, and yield mechanics of Luxor, result in a fair amount of volatility.

**LUX** could trade at a very high price because the market is ready to pay a hefty premium to capture a percentage of the current market capitalization. However, the price of **LUX** could also drop to a large degree if the market sentiment turns bearish. We would expect significant price volatility during our growth phase so please **do your own research** whether this project suits your goals.

## What is the point of buying it now when **LUX** trades at a very high premium? <a href="#what-is-the-point-of-buying-it-now-when-time-trades-at-a-very-high-premium" id="what-is-the-point-of-buying-it-now-when-time-trades-at-a-very-high-premium"></a>

When you buy and stake **LUX**, you capture a percentage of the supply (market cap) which will remain close to a constant. This is because your staked **LUX** balance also increases along with the circulating supply. The implication is that if you buy **LUX** when the market cap is low, you would be capturing a larger percentage of the market cap.

## What is a rebase? <a href="#what-is-a-rebase" id="what-is-a-rebase"></a>

Rebase is a mechanism by which your staked **LUX** balance increases automatically. When new **LUX** are minted by the protocol, a large portion of it goes to the stakers. Because stakers only see staked **LUX** balance instead of **LUX** the protocol utilizes the rebase mechanism to increase the staked **LUX** balance so that 1 staked **LUX** (**LUMens**) is always redeemable for 1 **LUX**.

## What is reward yield? <a href="#what-is-reward-yield" id="what-is-reward-yield"></a>

Reward yield is the percentage by which your staked **LUX** balance increases on the next epoch. It is also known as _rebase rate_. You can find this number on the Luxor staking page.

## What is APY? <a href="#what-is-apy" id="what-is-apy"></a>

**APY** stands for annual percentage yield. It measures the real rate of return on your principal by taking into account the effect of compounding interest. In the case of Luxor, your staked **LUX** represents your principal, and the compound interest is added periodically on every epoch (8 hours) thanks to the rebase mechanism.

One interesting fact about **APY** is that your balance will grow not linearly but exponentially over time! Assuming a daily compound interest of 2%, if you start with a balance of 1 **LUX** on day 1, after a year, your balance will grow to about 1377.&#x20;

![](https://gblobscdn.gitbook.com/assets%2F-MV4hwONledQK5nEDaUc%2Fsync%2F585854ca21f006875c918ba2aed711730f71284a.png?alt=media)

## How is the APY calculated? <a href="#how-is-the-apy-calculated" id="how-is-the-apy-calculated"></a>

The APY is calculated from the reward yield (a.k.a rebase rate) using the following equation:

$$
APY = ( 1 + rewardYield )^{1095}
$$

It raises to the power of 1,095 because a rebase happens 3 times daily. Consider there are 365 days in a year, this would give a rebase frequency of 365 \* 3 = 1,095.

Reward yield is determined by the following equation:

$$
rewardYield = LUX_{distributed} / LUX
_{totalStaked}
$$

The number of LUX distributed to the staking contract is calculated from LUX total supply using the following equation:

$$
LUX_{distributed} = LUX_
{totalSupply} \times rewardRate
$$

Note that the reward rate is subject to change by the protocol.

## Why does the price of LUX become irrelevant in long term? <a href="#why-does-the-price-of-time-become-irrelevant-in-long-term" id="why-does-the-price-of-time-become-irrelevant-in-long-term"></a>

As illustrated above, your **LUX** balance will grow exponentially over time thanks to the power of compounding. Let's say you buy a **LUX** for $400 now and the market decides that in 1 year time, the intrinsic value of **LUX** will be $2.&#x20;

Assuming a daily compound interest rate of 2%, your balance would grow to about 1377 **LUX** by the end of the year, which is worth around $2754. That is a cool $2354 profit! By now, you should understand that you are paying a premium for **LUX** now in exchange for a long-term benefit. Thus, you should have a long time horizon to allow your **LUX** balance to grow exponentially and make this a worthwhile investment.

## What will be LUX intrinsic value in the future? <a href="#what-will-be-time-intrinsic-value-in-the-future" id="what-will-be-time-intrinsic-value-in-the-future"></a>

There is no clear answer for this, but the intrinsic value can be determined by the treasury performance. For example, if the treasury could guarantee to back every **LUX** with 100 **DAI**, the intrinsic value will be 100 **DAI**. It can also be decided by the future DAO. For example, if the DAO decides to raise the price floor of **LUX**, its intrinsic value will rise accordingly.

## How does the protocol manage to maintain the high staking APY? <a href="#how-does-the-protocol-manage-to-maintain-the-high-staking-apy" id="how-does-the-protocol-manage-to-maintain-the-high-staking-apy"></a>

Let’s say the protocol targets an APY of 100,000%. This would translate to a rebase rate of about 0.6328%, or a daily growth of about 2%. Please refer to the [**equation**](https://wonderland.gitbook.io/wonderland/basics/faq#how-is-the-apy-calculated) above to learn how APY is calculated from the rebase rate.

If there are 100,000 **LUX** tokens staked right now, the protocol would need to mint an additional 2000 **LUX** to achieve this daily growth. This is achievable if the protocol can bring in at least 2000 **DAI** daily from bond sales. If the protocol fails to achieve this, the APY of 100,000% cannot be guaranteed.

## Do I have to unstake and stake LUX on every epoch to get my rebase rewards? <a href="#do-i-have-to-unstake-and-stake-time-on-every-epoch-to-get-my-rebase-rewards" id="do-i-have-to-unstake-and-stake-time-on-every-epoch-to-get-my-rebase-rewards"></a>

No. Once you have staked **LUX** with Luxor, your staked **LUX** (**LUMens**) balance will auto-compound on every epoch. _That increase in balance represents your rebase rewards._

## How do I track my rebase rewards? <a href="#how-do-i-track-my-rebase-rewards" id="how-do-i-track-my-rebase-rewards"></a>

You can track your rebase rewards by calculating the increase in your staked **LUX** balance.

1\. Record down the Current Index value on the staking page when you first stake your **LUX**. Let's call this the Start Index.

2\. After staking for some time, if you want to determine by how much your balance has increased, check the Current Index value again. Let's call this the End Index.

3\. By dividing the End Index by Start Index, you would get the ratio by which your staked **LUX** balance has increased.

$$
ratio = endIndex / startIndex
$$

## Is Luxor Audited?

Luxor is currently unaudited! It is a fork of Olympus DAO on the Fantom Opera Network, audits will occur at a later stage.&#x20;

**Stay cautious!**

## Why is it Minting and not Bonding?

Here at Luxor we believe that minting better describes the action that users are taking, when purchasing **LUX** with different assets. If you go to the "Mint" page of the website, you will be able to mint LUX tokens, effectively selling your assets for discounted **LUX** tokens. Despite the name difference, the process is exactly the same as a Bond Purchase on Olympus DAO!
