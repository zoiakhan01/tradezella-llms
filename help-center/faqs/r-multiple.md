---
title: Understanding R-Multiple
description: R-Multiple measures trade returns relative to initial risk amount
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/7190710-understanding-r-multiple
  md: https://www.tradezella.com/help-center/faqs/r-multiple.md
---

# Understanding R-Multiple

R-Multiple, often referred to as "R" in trading terminology, is a critical metric that measures your profit or loss relative to the amount of capital you risked on a trade. Rather than looking at absolute dollar amounts, R-Multiple normalizes returns to your initial risk, making it easier to compare trades of different sizes and understand your risk-reward relationship. The formula is simple: **R = (Profit or Loss) / Initial Risk**.

For example, if you risked $100 on a trade and made $300 profit, your R-Multiple would be 3R (or 3:1 risk-to-reward). If you risked $100 and lost $200, your R-Multiple would be -2R. Using R-Multiple helps traders evaluate their risk management, compare performance across different trading instruments, and determine whether they're following their trading plan's risk-reward targets.

In TradeZella, R-Multiple calculations are automatically performed for every trade you import. The platform uses your entry price and stop loss level to determine initial risk, then calculates how many multiples of that risk you gained or lost on each trade. This metric becomes even more powerful when analyzed across your entire trading history, showing patterns in your ability to capture risk-reward ratios that match your trading plan.

## How R-Multiple Is Calculated

### The Basic Formula
**R-Multiple = Trade Profit (or Loss) / Initial Risk per Share (or Contract)**

### Example Calculations

**Stock Trade Example:**
- Entry: $50.00 per share
- Stop Loss: $48.00 per share
- Initial Risk per Share: $2.00 (your R)
- Exit: $56.00 per share
- Profit per Share: $6.00
- R-Multiple: $6.00 / $2.00 = **3R** (3 times your risk)

**Options Trade Example:**
- Entry: Buy 1 call option for $2.00 per contract ($200 total)
- Stop Loss: $0.50 per contract
- Initial Risk: $1.50 per contract ($150 total)
- Exit: Sell for $5.00 per contract ($500 total)
- Profit: $3.00 per contract ($300 total)
- R-Multiple: $3.00 / $1.50 = **2R**

**Futures Trade Example:**
- Entry: Long ES contract at 4800
- Stop Loss: 4790 (10 points × $50 multiplier = $500 risk)
- Exit: 4830 (30 points × $50 multiplier = $1,500 profit)
- R-Multiple: $1,500 / $500 = **3R**

## Why R-Multiple Matters

### Risk-Reward Ratio Alignment
Traders often set targets like "I need 2R reward for 1R risk" or "minimum 3R trades." R-Multiple helps you see if you're actually hitting these targets across your trades.

### Comparing Different Trades
A $5,000 profit on one trade and a $500 profit on another sound different, but if the first trade risked $10,000 and the second risked $100, both were 0.5R trades. R-Multiple eliminates the noise of position size.

### Edge Discovery
Analyzing your R-Multiple distribution helps identify edges in your strategy. If your average winning trade is 2.5R and your average losing trade is -1R with a 60% win rate, you have positive expectancy.

### Position Sizing Evaluation
R-Multiple analysis can reveal if you're sizing positions appropriately relative to your stop loss. Consistently taking much larger or smaller R values than intended suggests your position sizing logic needs adjustment.

## R-Multiple Categories in TradeZella

### Positive R
Trades where profit exceeded initial risk. A +2R trade means you made twice your risk amount.

### Negative R
Trades where you took a loss. A -1.5R trade means you lost 1.5 times your risk amount.

### Breakeven
Trades that resulted in approximately zero profit or loss (typically within transaction costs).

## Analyzing Your R-Multiple Distribution

TradeZella's analytics dashboard shows:
- **Average R per Trade:** Your mean R across all trades in the selected period/strategy
- **Best R Trade:** Highest R-Multiple achieved
- **Worst R Trade:** Lowest R-Multiple (biggest loss relative to risk)
- **R Distribution Chart:** Visual representation of all your trades plotted by R-Multiple

This distribution helps you understand your typical outcomes and identify outliers that may represent violations of your trading plan.

## Setting R-Multiple Targets

Smart traders use expected R-Multiple targets as part of their trading plan:
- Require minimum 2:1 risk-to-reward ratio (willing to take -1R trades if reward target is +2R)
- Average winning trade must be at least 1.5R
- Stop losses are set to establish initial risk, then profit targets are set based on R goals

---

## See also
- [What Is Trade Expectancy, and How Does It Help?](/help-center/faqs/trade-expectancy.md)
- [How to Edit Trades in TradeZella](/help-center/faqs/how-to-edit-trades.md)
- [How to Filter Your Trades in TradeZella](/help-center/faqs/how-to-filter-trades.md)
