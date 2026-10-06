# gate io futures fees: The 0.02%/0.05% Base Rate, the VIP Ladder Behind It, and the Costs Most Traders Miss

Search for Gate futures fees and you get three numbers that don't agree: 0.02%, 0.05%, and 0.075%. All three are real, and none of them is your total cost. They describe different things — resting orders, crossing orders, and one specific way of paying — and a fee comparison table will never show you the rest of the bill.

Here's what a Gate USDT-margined perpetual actually charges, how the 17-tier ladder works, and where the money goes after the trading fee.

## What one futures trade costs on a fresh account

At VIP 0, Gate charges **0.020% for maker orders and 0.0500% for taker orders** on standard USDT perpetual contracts. Taker is the rate most people pay, because a market order crosses the spread by definition.

The fee is charged on position value, not on the margin you put up:

> Trading fee = position value × maker/taker rate

A $10,000 notional trade costs roughly $5 at 0.05% to open and $5 to close — $10 for the round trip. Two things worth knowing before you compare that figure with another exchange:

- **Leverage doesn't move the rate.** It only changes how large the fee looks next to your margin. At 10x on $1,000 of margin, a $10 round trip is 1% of the money you actually posted. For a small account, that ratio matters more than a one-basis-point difference in the published rate.
- **Unfilled and cancelled orders cost nothing.** Fees are deducted from position margin and only appear on open, close, or partial close.

To see the number that applies to your own account rather than a table on the internet, 👉 [open a Gate account and check your live fee tier](https://bit.ly/GateVIP) — the rate displayed inside your account is the one that bills you.

## Maker vs taker: your limit order isn't automatically cheaper

Maker orders sit in the book and wait. Taker orders match against existing orders immediately. The rate you get depends on what happened at the moment of execution, not on which button you clicked.

A limit order can still be a taker trade: if you place a limit price that's already resting on the other side, it fills instantly and bills at the taker rate. Only the portion that waits in the order book earns the maker rate. The practical version of this is that "I use limit orders" is not the same as "I pay maker fees," and the difference between the two rates on the base tier is 2.5x.

## The complete VIP 0 to VIP 16 futures fee table

Gate publishes 17 tiers. The table below is the standard USDT perpetual ladder — the one that applies to BTC_USDT, ETH_USDT and the rest of the standard crypto perpetuals.

| VIP tier | 30-day weighted volume to qualify (USD) | Maker | Taker | Open an account |
| --- | --- | --- | --- | --- |
| VIP 0 | Below 60,000 | 0.0200% | 0.0500% | [Open account](https://bit.ly/GateVIP) |
| VIP 1 | ≥ 60,000 | 0.0200% | 0.0500% | [Open account](https://bit.ly/GateVIP) |
| VIP 2 | ≥ 120,000 | 0.0200% | 0.0500% | [Open account](https://bit.ly/GateVIP) |
| VIP 3 | ≥ 240,000 | 0.0200% | 0.0480% | [Open account](https://bit.ly/GateVIP) |
| VIP 4 | ≥ 500,000 | 0.0200% | 0.0480% | [Open account](https://bit.ly/GateVIP) |
| VIP 5 | ≥ 1,000,000 | 0.0200% | 0.0450% | [Open account](https://bit.ly/GateVIP) |
| VIP 6 | ≥ 3,000,000 | 0.0180% | 0.0420% | [Open account](https://bit.ly/GateVIP) |
| VIP 7 | ≥ 8,000,000 | 0.0160% | 0.0375% | [Open account](https://bit.ly/GateVIP) |
| VIP 8 | ≥ 20,000,000 | 0.0140% | 0.0350% | [Open account](https://bit.ly/GateVIP) |
| VIP 9 | ≥ 50,000,000 | 0.0120% | 0.0320% | [Open account](https://bit.ly/GateVIP) |
| VIP 10 | ≥ 100,000,000 | 0.0100% | 0.0300% | [Open account](https://bit.ly/GateVIP) |
| VIP 11 | ≥ 120,000,000 | 0.0080% | 0.0280% | [Open account](https://bit.ly/GateVIP) |
| VIP 12 | ≥ 240,000,000 | 0.0060% | 0.0260% | [Open account](https://bit.ly/GateVIP) |
| VIP 13 | ≥ 440,000,000 | 0.0050% | 0.0240% | [Open account](https://bit.ly/GateVIP) |
| VIP 14 | ≥ 800,000,000 | 0.0020% | 0.0220% | [Open account](https://bit.ly/GateVIP) |
| VIP 15 | ≥ 1,600,000,000 | 0.0000% | 0.0180% | [Open account](https://bit.ly/GateVIP) |
| VIP 16 | ≥ 3,000,000,000 | 0.0000% | 0.0160% | [Open account](https://bit.ly/GateVIP) |

Two things jump out of that column of makers.

**The maker rate doesn't budge until VIP 6.** From VIP 0 through VIP 5 it's 0.0200% on every row. If you mostly rest orders and your 30-day volume is, say, $400,000, you pay exactly what a brand-new account pays. This is the single most common surprise in threads about Gate futures fees, and it's not a bug — the ladder is built to reward size, not order type.

**Zero maker arrives at VIP 15.** Fifteen tiers above a new account, versus venues that publish 0% maker as their standard rate.

One caveat on precision: Gate's own documents don't line up perfectly at the edges. An older fee announcement lists marginally different maker rates at VIP 3 through VIP 5 than the current help-centre table does. When two official pages disagree, the fee page inside your logged-in account is the one that matters.

## How Gate decides which tier you're in

Two tracks, and you get whichever is better:

- **30-day trading volume**, calculated with product weightings. Spot volume (including Convert) and stock trading count at 100%, USDT perpetuals, BTC perpetuals and USDT delivery futures at 40%, options and USD1 contracts at 20%, CFD contracts at 10%. Copy-trading volume is included.
- **14-day average GT holdings**, including GT2. VIP 1 starts at 100 GT, VIP 6 at 12,000 GT, VIP 8 at 50,000 GT.

Tiers are reassessed monthly. The 40% weighting on futures is worth pausing on: a pure futures desk has to turn over roughly 2.5x the notional of a spot trader to land on the same tier. If you trade both, the spot side is doing more for your tier than the futures side.

## The 0.075% number you keep seeing

This is where most fee articles get muddy. Gate's help centre documents a Points deduction for futures taker fees: the deduction is applied at a fixed **0.075%** nominal rate, with the final effective rate dropping as low as **0.0225%** depending on the conditions of your account.

Three details decide whether that helps you:

- It applies to **taker fees only**. Maker fees can't be offset with Points.
- If your Points balance runs dry, billing falls back to your VIP tier rate.
- It's a pricing path, not an automatic discount. You opt into it, and whether it beats your tier rate depends on your account.

Separately, GT deduction reduces **spot** trading fees by about a tenth at the base tier (0.1% to 0.09%), and the GT discount column stops helping entirely from VIP 10 upward, where the standard and GT rates converge. Nothing about GT deduction changes your futures rate.

There are also fee rebate vouchers, which cover part of the trading fees you generate. They need manual activation, only one can be active at a time, and the refund lands in your spot account on the next trading day.

## Funding rate: the cost that isn't a fee

Funding is not a Gate charge. It's a transfer between longs and shorts, and the platform takes none of it. If the funding rate is positive, longs pay shorts; if negative, shorts pay longs.

The mechanics worth knowing:

- Funding = position notional value × funding rate. Like the trading fee, it's based on position value, not margin, so leverage doesn't change the rate.
- Most contracts settle every 8 hours, at 00:00, 08:00 and 16:00 UTC. Some pairs use a 4-hour cycle, which means six settlements a day.
- If you close before the settlement timestamp, you don't pay or receive it.
- The rate is recalculated every 60 seconds and the cycle's weighted average becomes the final rate. Gate's baseline interest is 0.03% per day, which works out to 0.01% per 8-hour cycle before the premium index is applied. Caps vary by contract and are published on the contract info page.

Why this matters when you're comparing fees: hold a $10,000 long for a week at 0.01% per settlement and you pay roughly $21 in funding across 21 settlements. A round trip in taker fees on the same position is $10. Funding is often double the trading cost, and it never shows up in a maker/taker table.

## What changed on 1 September 2026

Gate split its fee structure in two, and this is the newest thing to know if you're pricing a trade.

**TradFi perpetuals got their own schedule.** Contracts on stocks, metals, indices, FX and commodities no longer share the standard USDT perpetual ladder. The dedicated TradFi ladder starts at the same 0.0200%/0.0500% at VIP 0, but descends faster — it reaches 0% maker at VIP 14 rather than VIP 15, and the VIP requirements for each tier didn't change.

**A taker discount programme opened.** Discount level depends on your share of platform-wide USDT perpetual taker volume in a calculation period:

| Monthly share of platform taker volume | Taker fee discount |
| --- | --- |
| 0.02% ≤ X < 0.2% | 9% |
| 0.2% ≤ X < 1% | 16% |
| X ≥ 1% | 20% |

You have to register through your account manager — it isn't switched on by default. Managed sub-accounts don't qualify, and if you miss the entry threshold in one month's assessment, you revert to the standard rate the following month.

For anyone below those volume bands, the practical takeaway is straightforward: the standard ladder in the table above is your pricing.

## How Gate futures fees compare

Traders Union's fee survey, updated in April 2026, puts the industry average for futures at 0.024% maker and 0.053% taker. Gate's base rate of 0.02%/0.05% sits just under that, and level with Binance's and Kraken's standard rates in the same table.

At $15 million of 30-day volume, the same survey shows Gate at 0.016% maker / 0.0375% taker, Binance at 0.016% / 0.04%, and Kraken at 0.01% / 0.035%. The same comparison shows MEXC listing 0% maker and 0.02% taker with no tier or token requirement.

That last line is the honest framing of the whole trade-off. Gate's ladder rewards genuinely large turnover, and it publishes all 17 tiers to logged-out visitors, which is more transparency than most venues offer. But below VIP 6 the maker rate is flat, so if your strategy is limit-order heavy and your volume is moderate, a flat schedule can cost you less for structural reasons rather than promotional ones.

## Six ways to pay less, and one that usually backfires

1. **Rest orders when you can.** The gap between 0.02% and 0.05% is the largest single lever on the base tier, and it's free.
2. **Check your tier each month.** Reassessment is monthly, and volume weightings mean your spot activity contributes more than you may assume.
3. **Run the Points maths on your taker flow.** It's a real pricing path down to 0.0225%, but it only touches taker fees.
4. **Activate a fee rebate voucher** if you have one sitting in your card centre. They expire.
5. **Watch funding on multi-day holds.** Fewer, larger positions are cheaper on funding than many small ones held through settlements.
6. **Look at the GT track** if you already hold GT for other reasons. Don't buy it solely to chase a tier.

The one that backfires: pushing your 30-day volume higher to reach the next tier. The extra notional you have to trade will almost always cost more than the basis points you save, and it puts on risk you didn't want. On the standard ladder, the first meaningful maker break is three million dollars of weighted volume away.

If you're starting from zero and want to see the actual numbers against your own account, 👉 [sign up on Gate and check which tier you land in](https://bit.ly/GateVIP). Tier assignment happens automatically, so you'll know your rate before your first trade rather than after.

## Gate futures fees: quick answers

**What are Gate's futures fees?** On standard USDT perpetuals, 0.020% for maker orders and 0.0500% for taker orders at VIP 0, charged on position value and deducted from position margin.

**Does leverage affect the fee?** No. The rate applies to position value regardless of leverage. Higher leverage only makes the fee larger relative to the margin you posted.

**Can I pay futures fees with GT?** GT deduction reduces spot trading fees. Futures taker fees can be offset with Points, at a fixed 0.075% nominal rate with an effective floor around 0.0225%. Futures maker fees can't be offset with either.

**Do I pay a fee if my order doesn't fill?** No. Cancelled and unfilled orders are free.

**When is funding charged?** Every 8 hours at 00:00, 08:00 and 16:00 UTC for most contracts, and every 4 hours for pairs on the shorter cycle. Close before the settlement timestamp and you skip it.

**Is Gate cheaper than Binance for futures?** On base rates they're level at 0.02%/0.05%. Beyond that it depends on your volume, which tier weighting your activity falls into, and whether you're willing to hold GT — 👉 [compare your own numbers on the tier table](https://bit.ly/GateVIP) rather than trusting a single headline figure from any comparison site.
