---
title: How to Take Partials in Backtesting
description: Scaling out of positions partially during backtesting sessions
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/9828709-how-to-take-partials-in-backtesting
  md: https://www.tradezella.com/help-center/backtesting-replay/take-partials-backtesting.md
---

# How to Take Partials in Backtesting

Taking partials (also called scaling out) is a professional trade management technique where you close part of your position at target prices while letting the rest run. TradeZella backtesting fully supports partial exits to help you refine this critical skill.

## What is a Partial Exit?

### Understanding Partials

A partial exit means:
- **Close part of position**: Exit 50% at first target, 25% at second target
- **Keep position open**: Remaining 25% continues running
- **Multiple exit points**: Exit at multiple price levels
- **Maximize winners**: Lock in profit while preserving upside
- **Risk management**: Secure gains while protecting remaining capital

### Example Scenario

**Initial Trade Setup:**
- Entry: 100 contracts at 4500
- Initial risk: $10,000

**Partial Exit Strategy:**
- Exit 40 contracts at 4550 (first target) - Lock in $2,000 profit
- Exit 35 contracts at 4600 (second target) - Lock in additional profit
- Exit 25 contracts at breakeven if price reverses - Protect capital
- Keeps structure and reduces risk as trade progresses

## Benefits of Taking Partials

### Risk Management
- **Lock in profits**: Secure gains at predetermined levels
- **Reduce risk**: Lower position size reduces drawdown
- **Breakeven protection**: Move stop to breakeven after first target
- **Preserve capital**: Avoid giving back large gains

### Performance Optimization
- **Improve win rate**: More trades hit partial targets
- **Increase profit factor**: Lock wins while managing losses
- **Better risk/reward**: Achieve higher R-multiples on winners
- **Psychological benefit**: Confidence from hitting targets

### Trade Refinement
- **Test different scales**: Experiment with partial strategies
- **Optimize timing**: Find best exit points through backtesting
- **Develop discipline**: Practice systematic exit strategies
- **Build playbook**: Document your best partial techniques

## How to Take Partials in Backtesting

### Method 1: Click-Based Partial Exits

**During a Live Trade:**
1. **Right-click on your position** in the chart or positions panel
2. **Select "Take Partial Profit"** or "Scale Out"
3. **Enter the quantity** to exit (e.g., 50 contracts of 100)
4. **Choose exit type**: Market order, limit order, or at specific price
5. **Confirm execution**
6. **Remaining position stays open** at original entry

### Method 2: Drag to Scale Out

**Direct Chart Interaction:**
1. **Locate your entry point** on the chart
2. **Drag from entry point downward** (long position) or upward (short)
3. **Drag to your target price level**
4. **Release at target**: Automatically sets partial exit order
5. **Chart shows scaled position**
6. **Continue trading with remaining position**

### Method 3: Using the Positions Panel

**From the Positions Panel:**
1. **Right-click your active trade** in positions list
2. **Select "Close Partial"** option
3. **Use slider to select % to close**: 25%, 50%, 75%
4. **Or enter specific quantity**: Close 50 of 200 contracts
5. **Confirm action**
6. **Remaining position updates** in positions panel

### Method 4: Hotkey Scaling

**Quick Keyboard Scaling:**
1. **Select your position** (click on it)
2. **Press Ctrl+1** for 25% scale out
3. **Press Ctrl+2** for 50% scale out
4. **Press Ctrl+3** for 75% scale out
5. **Custom hotkeys**: Configure your preferred percentages

## Setting Up Partial Targets Before Entry

### Pre-Planned Scaling Strategy

Professional traders often plan partials before entering:

1. **Before placing entry order:**
   - Define your 1st target (take 25%)
   - Define your 2nd target (take 25%)
   - Define your 3rd target (take 25%)
   - Define your stop level (close final 25%)

2. **Enter the trade** with all targets pre-set
3. **TradeZella automatically executes** at each target
4. **No manual intervention needed**
5. **Disciplined execution**

### Example Pre-Planned Setup

| Level | Action | Quantity | Price |
|-------|--------|----------|-------|
| Entry | Buy | 100 | 4500 |
| Target 1 | Sell 25% | 25 | 4525 |
| Target 2 | Sell 25% | 25 | 4550 |
| Target 3 | Sell 25% | 25 | 4600 |
| Stop | Sell 25% | 25 | 4490 |

## Advanced Partial Strategies

### Trailing Stop Strategy

After hitting first target:
1. **Close 50% at first target** (4525)
2. **Move stop to breakeven** (4500) on remaining position
3. **Set trailing stop**: 30 points below market
4. **Let winner run** with protected capital

### Multiple Timeframe Partials

Using different timeframes:
1. **1st target**: When 4-hour target hits (exit 25%)
2. **2nd target**: When daily resistance tested (exit 25%)
3. **3rd target**: When weekly target achieved (exit 25%)
4. **Final position**: Run to ultimate goal (exit 25%)

### Volatility-Based Scaling

Adjust partial sizes based on market conditions:
1. **High volatility**: Smaller partials (take 10% each time)
2. **Low volatility**: Larger partials (take 50% at a time)
3. **Adjust targets**: Wider stops in high volatility
4. **Adapt in real-time** as you backtest different conditions

## Managing Multiple Partial Exits

### Tracking Partial Exits

Your journal automatically records:
- **Each partial close**: Separate entry in your journal
- **Cumulative P&L**: Total profit from all partials on that trade
- **Average exit price**: Calculated across partial exits
- **Exit progression**: Timeline of each scale-out

### Position Size After Partials

**Remaining Position Calculation:**
- Initial: 100 contracts
- After 1st partial (25%): 75 contracts remain
- After 2nd partial (25%): 50 contracts remain
- After 3rd partial (25%): 25 contracts remain
- Remaining position continues with original entry price

### Risk After Partials

**Risk Profile Changes:**
- Remaining position has lower absolute risk
- But still exposed to percentage moves
- Stop loss should reflect remaining position size
- Total account risk decreases with each partial

## Analyzing Partial Exit Performance

### Journal Analysis of Partials

After backtesting with partials, analyze:
- **Did partials help or hurt performance?**
- **Were target levels optimal?**
- **Did you give back too much?**
- **Could you have held longer?**
- **What was the impact on R-multiple?**

### Metrics to Track

- **Average profit per partial**: Track each exit level
- **Win rate on partials**: How often you hit targets
- **Missed opportunities**: Times target was hit then reversed
- **Optimal partial percentages**: Which splits work best
- **Best performing targets**: Which target level is most reliable

## Partial Exit Patterns to Test

### Conservative Scaling (Good Risk Management)
- 50% at first target
- 25% at second target
- 25% final stop

**Best for**: Risk-averse traders, capital preservation focus

### Aggressive Scaling (Maximize Winners)
- 25% at first target
- 25% at second target
- 50% final target

**Best for**: Trend traders, high conviction setups

### Balanced Approach
- 33% at first target
- 33% at second target
- 34% final exit

**Best for**: Most traders, balanced risk/reward

## Partial Exit Keyboard Shortcuts

| Action | Shortcut |
|--------|----------|
| Close 25% of position | Ctrl+1 |
| Close 50% of position | Ctrl+2 |
| Close 75% of position | Ctrl+3 |
| Close remaining | Ctrl+4 |
| Undo last partial | Ctrl+Z |
| Scale to breakeven | Ctrl+B |

## Tips for Effective Partial Testing

1. **Start simple**: Test 2-partial strategy before complex scaling
2. **Document targets**: Write down your targets before entry
3. **Stay consistent**: Use same partial strategy across multiple trades
4. **Review results**: Analyze partial effectiveness monthly
5. **Adjust gradually**: Make small refinements based on data
6. **Track in journal**: Note all partial exits in your journal
7. **Compare strategies**: Test different partial approaches in different sessions

## Common Mistakes with Partials

### Mistakes to Avoid

- **Scaling too small**: Tight partials miss upside on winners
- **No scaling plan**: Random partials lack discipline
- **Giving back gains**: Not protecting partial profits with trailing stops
- **Over-complicating**: Too many levels creates confusion
- **No analysis**: Not reviewing partial effectiveness
- **Ignoring context**: Not adjusting for market conditions

---

## See also
- [Understanding Different Order Types in TradeZella Backtesting](./order-types-backtesting.md)
- [How to Create a Backtesting Session](./create-backtesting-session.md)
- [Journaling Backtesting Trades While Backtesting](./journaling-while-backtesting.md)
