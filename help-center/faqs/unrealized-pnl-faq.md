---
title: Unrealized P&L FAQ
description: FAQ about unrealized (open) P&L vs realized P&L, how TradeZella calculates and displays them
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/12572470-unrealized-p-l-faq
  md: https://www.tradezella.com/help-center/faqs/unrealized-pnl-faq.md
---

# Unrealized P&L FAQ

Understanding the difference between unrealized P&L (profit and loss on open positions) and realized P&L (profit and loss on closed positions) is fundamental to trading and evaluating performance. TradeZella displays both metrics separately because they tell different stories about your trading. Realized P&L represents actual money made or lost on trades you've completed, while unrealized P&L shows the current paper profit or loss on positions you still hold. Together, these metrics provide a complete picture of your account equity and trading performance.

Many traders focus only on realized P&L and ignore unrealized P&L, but this can be misleading. A trader might have strong realized P&L but massive unrealized losses on open positions, meaning their actual account is underwater. Conversely, a trader with poor realized P&L might have large unrealized gains that could improve overall performance if those positions are closed profitably. TradeZella makes it easy to track both metrics to understand your true position and account status.

## Basic Definitions

### Unrealized P&L
- Profit or loss on positions you currently hold but haven't closed yet
- Also called "paper profit/loss" or "open P&L"
- Changes in real-time as market price moves
- Not locked in until you close the position
- Can swing dramatically between sessions

**Example:** You bought 100 shares of Apple at $150. The stock is now at $165. Your unrealized profit is: (165 - 150) × 100 = $1,500. This is a paper profit. If you sell right now, you'll realize this $1,500 gain (minus commissions).

### Realized P&L
- Profit or loss on positions you've closed
- Also called "actual P&L" or "locked-in P&L"
- Final, unchanging figure once trade closes
- Real money earned or lost
- Your account has actual cash from realized P&L

**Example:** Same Apple trade—you bought 100 shares at $150 and sold at $165. Your realized profit is: (165 - 150) × 100 = $1,500. This is now confirmed; the money is in your account.

### Total P&L
- Realized P&L + Unrealized P&L
- Represents your total profit or loss if you closed all positions right now
- Changes as markets move and trades close
- Most important number for understanding overall account health

**Example:**
- Realized P&L: +$5,000 (from closed trades)
- Unrealized P&L: -$2,000 (from open positions)
- Total P&L: +$3,000

## Calculating Unrealized P&L

### Formula by Asset Type

**Equities/Stocks:**
- Unrealized P&L = (Current Price - Entry Price) × Quantity
- Example: Bought 100 shares at $50, current price $52 = ($52 - $50) × 100 = $200

**Options:**
- Unrealized P&L = (Current Option Price - Entry Price) × Contracts × 100
- Example: Bought 1 call at $2.00, current price $3.50 = ($3.50 - $2.00) × 1 × 100 = $150

**Forex:**
- Unrealized P&L = (Current Price - Entry Price) × Pip Value × Quantity
- Example: Long EUR/USD at 1.1000, current 1.1050 = 50 pips × $10 per pip = $500

**Futures:**
- Unrealized P&L = (Current Price - Entry Price) × Contract Multiplier × Quantity
- Example: Long ES at 4800, current 4820 = 20 points × $50 × 1 = $1,000

**Cryptocurrency:**
- Unrealized P&L = (Current Price - Entry Price) × Quantity in Coins
- Example: Bought 0.5 BTC at $40,000, current $45,000 = ($45,000 - $40,000) × 0.5 = $2,500

### Accounting for Commissions

Some traders include commissions in unrealized P&L calculations; others don't:

**Including Commissions:** More realistic because commissions reduce profit
- Unrealized P&L (with commissions) = [(Current Price - Entry Price) × Quantity] - Commissions

**Excluding Commissions:** Shows pure price movement P&L
- Unrealized P&L (excluding commissions) = (Current Price - Entry Price) × Quantity

TradeZella typically displays both, allowing you to see pure price P&L and commissions separately.

## How TradeZella Calculates & Displays P&L

### Dashboard Display

**Account Summary Widget:**
- Shows Total P&L prominently
- Breaks down into Realized P&L + Unrealized P&L
- Updates in real-time as prices change
- Color coding: Green for gains, Red for losses

**Open Positions Panel:**
- Lists all open trades
- Shows unrealized P&L for each position
- Shows percentage gain/loss
- Shows quantity and current price

**Closed Trades Journal:**
- Lists completed trades
- Shows realized P&L for each trade
- Shows entry price, exit price, profit
- Shows percentage gain/loss

### Real-Time Updates

**Unrealized P&L Updates:** Constantly refresh as market prices change
- During market hours: Updates multiple times per second
- Outside market hours: Updates based on last known price
- Can change dramatically during volatile market conditions

**Realized P&L:** Static once trade is closed
- Never changes after closing
- Only updates when you close a new trade
- Historical record remains permanent

### Filtering & Analysis

**By Position:** See unrealized P&L on individual open trades
**By Account:** See total unrealized P&L across all accounts
**By Symbol:** Filter to see unrealized P&L on specific symbols
**By Strategy:** Group unrealized P&L by trading strategy
**By Date:** See how unrealized P&L has changed over time

## Common Questions About P&L

### Why Is My Unrealized P&L Negative?
Your position moved against you. If you bought at $100 and price is now $95, you have a $5 unrealized loss per share. This is temporary until you close the trade.

### Should I Close Trades with Unrealized Losses?
Depends on your trading plan. If the setup is broken and you should exit per your rules, yes. If you're within your stop loss and plan to hold, keep it. Don't let unrealized losses force emotional decisions.

### How Do I Know If I'm Really Profitable?
Look at Realized P&L, not Total P&L. Your realized P&L shows actual profits from closed trades. Unrealized P&L is temporary and can reverse.

### What If I Have Large Unrealized Losses?
Unrealized losses are concerning because:
1. Your account equity is reduced
2. You've lost capital that could be deployed elsewhere
3. Risk management may suggest closing losing positions
4. You're exposed to further losses if price moves more against you

However, unrealized losses can also reverse if price moves back in your favor. Review your trading plan to decide if you should hold or exit.

### Can Unrealized Gains Disappear?
Yes. Until you close a position, unrealized gains are only "on paper." If you have an unrealized gain of $1,000 but don't close the trade, and price moves back to your entry, the gain disappears. Paper profits aren't real until you lock them in.

## Using P&L Data for Trading Improvement

### Analyzing Realized P&L
1. Filter closed trades by time period (monthly, quarterly)
2. Calculate win rate: (Number of wins / Total closed trades) × 100
3. Calculate average win and average loss
4. Calculate expectancy: (Win rate × Avg win) - (Loss rate × Avg loss)
5. Identify which strategies/symbols are most profitable

**Question:** Are some of your strategies more profitable than others? Focus on the winners.

### Analyzing Unrealized P&L
1. Review current open positions
2. Calculate: How much of your account equity is at risk in open positions?
3. Identify: Do your unrealized losses exceed your risk tolerance?
4. Ask: Are these positions aligned with your trading plan?
5. Decide: Should any positions be closed to reduce risk?

**Question:** Is your account equity too concentrated in positions moving against you?

### Total P&L Perspective
1. Track Total P&L weekly or monthly
2. Identify: Is total equity growing or shrinking over time?
3. Compare: Is your account making money after all trades and positions?
4. Evaluate: Are you outperforming if you held it in the S&P 500?

**Question:** Is your trading strategy worth the time and risk, or would passive index investing be better?

## Scenarios & Examples

### Scenario 1: Mixed Performance
**Open Positions:**
- Long 100 AAPL at $150, current $155 = +$500 unrealized
- Short 50 TSLA at $200, current $195 = -$250 unrealized (oops)
- Total Unrealized P&L: +$250

**Closed Trades This Month:**
- MSFT: Bought $300, sold $310 = +$1,000 realized
- GOOGL: Bought $2,500, sold $2,480 = -$2,000 realized
- Total Realized P&L: -$1,000

**Total P&L: -$750** (You're actually down overall, despite unrealized gains)

**Interpretation:** Your position sizing on GOOGL was too large. Reduce position size or review why you took that losing GOOGL trade.

### Scenario 2: Strong Realized, Weak Unrealized
**Closed Trades:**
- 10 winning trades at average $500 each = +$5,000
- 5 losing trades at average -$300 each = -$1,500
- Realized P&L: +$3,500

**Open Positions:**
- Multiple positions with unrealized losses totaling -$4,000

**Total P&L: -$500** (Disappointing, even with good realized performance)

**Interpretation:** You're closing winners but holding losers. Review exit strategy. Consider using stop losses to close losers earlier.

### Scenario 3: Strong Total Performance
**Realized P&L:** +$8,000 from closed trades
**Unrealized P&L:** +$3,000 from open positions
**Total P&L:** +$11,000

**Interpretation:** Trading well overall. Both closed and open trades performing. Continue current approach while managing open positions.

## Best Practices

**Monitor Both Metrics:** Don't focus only on realized P&L and ignore unrealized. Your account needs both to be healthy.

**Realize Winners:** Consider taking profits on large unrealized gains rather than letting them disappear if price reverses.

**Address Large Unrealized Losses:** If unrealized losses exceed your risk tolerance or account rules, consider closing positions.

**Track Trend:** Monitor if total P&L is growing or shrinking over weeks/months. Growing account = good process.

**Review Open Positions:** Regularly review what you're holding. Is each open position aligned with your trading plan?

**Don't Emotionalize:** Unrealized losses are temporary. Stick to your trading plan rather than making emotional decisions based on current P&L.

---

## See also
- [What Is Trade Expectancy, and How Does It Help?](/help-center/faqs/trade-expectancy.md)
- [Understanding R-Multiple](/help-center/faqs/r-multiple.md)
- [How to Edit Trades in TradeZella](/help-center/faqs/how-to-edit-trades.md)
