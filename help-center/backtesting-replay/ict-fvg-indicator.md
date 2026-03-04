---
title: Utilizing the ICT Fair Value Gap (FVG) Indicator in TradeZella Backtesting
description: How to use the ICT Fair Value Gap indicator for ICT methodology traders
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/10396341-utilizing-the-ict-fair-value-gap-fvg-indicator-in-tradezella-backtesting
  md: https://www.tradezella.com/help-center/backtesting-replay/ict-fvg-indicator.md
---

# Utilizing the ICT Fair Value Gap (FVG) Indicator in TradeZella Backtesting

The ICT Fair Value Gap (FVG) indicator is an advanced tool designed specifically for traders following Inner Circle Trading (ICT) methodology. This tool automatically identifies and highlights fair value gaps on your charts for precise entry and exit planning.

## Understanding Fair Value Gaps (FVGs)

### What is a Fair Value Gap?

A fair value gap is a price range that the market "skipped over" due to a gap move:

**Example Scenario:**
- Candle 1 high: 4550
- Candle 2 low: 4560
- Gap exists: 4550-4560 (untested price zone)
- This zone is the "fair value gap"

### Why FVGs Matter in Trading

Fair value gaps represent:
- **Imbalance zones**: Market inefficiency that needs correction
- **Liquidity vacuums**: Areas traders skipped when entering/exiting
- **Return opportunities**: Market likely to return to fill the gap
- **Entry signals**: Potential reversal or continuation points
- **ICT core concept**: Fundamental to many ICT trading strategies

### Two Types of FVGs

**Bullish FVG (Upward Gap)**
- Market gaps upward overnight or intraday
- Creates unfilled zone below current price
- Often acts as support level
- Signals bullish bias

**Bearish FVG (Downward Gap)**
- Market gaps downward overnight or intraday
- Creates unfilled zone above current price
- Often acts as resistance level
- Signals bearish bias

## Accessing the FVG Indicator

### Enabling the Indicator

1. **Open your backtesting session**
2. **Click the Indicators button** in the chart toolbar
3. **Search for "Fair Value Gap"** or "FVG"
4. **Click to add** the indicator to your chart
5. FVG zones appear as highlighted zones on your chart

### Indicator Customization

Once enabled, customize the appearance:

**Visual Settings:**
- **Zone color**: Change FVG display color
- **Opacity**: Adjust transparency (0-100%)
- **Border style**: Solid, dashed, or dotted lines
- **Background fill**: Highlight entire zone or just lines
- **Legend**: Show/hide on chart

**Configuration Options:**
- **Minimum gap size**: Filter gaps below certain size
- **Lookback period**: How many candles to scan for gaps
- **Timeframe sync**: Apply across multiple timeframes
- **Alert notifications**: Get alerts when price approaches FVG

## Identifying FVGs on Your Charts

### Visual Recognition

FVGs appear as clearly marked zones on your chart:

**Bullish FVG Display:**
- Green highlighted zone
- Below current price level
- Indicates gap to the upside
- Area price skipped over

**Bearish FVG Display:**
- Red highlighted zone
- Above current price level
- Indicates gap to the downside
- Area price skipped over

### Size Categories

The indicator classifies gaps by magnitude:

**Small FVGs**: 10-20 pips
- Minor imbalances
- Frequent occurrences
- Quick fills often

**Medium FVGs**: 20-50 pips
- Moderate imbalances
- Normal market activity
- Common trading opportunities

**Large FVGs**: 50+ pips
- Significant imbalances
- Major news or events
- Strong fill probability

## Using FVGs in Backtesting Strategy

### FVG Fill Strategy

One of the most popular ICT strategies:

1. **Identify FVG**: Use indicator to spot gaps
2. **Confirm age**: How old is the gap? (hours, days)
3. **Watch for pullback**: Price retraces toward FVG zone
4. **Enter at FVG**: Trade the fill of the gap
5. **Target beyond**: Exit past the FVG zone

**Example:**
- Bullish FVG identified: 4500-4505
- Price pulls back to 4510
- Place buy limit at 4503
- Target: 4495 or lower (fill the gap)

### Combining FVGs with Other Confirmations

Don't trade FVG fills alone. Combine with:

**Price Action Confirmation:**
- Candle patterns (pins, engulfings)
- Support/resistance levels
- Trend direction
- Volume analysis

**ICT Tools:**
- Order blocks
- Breaker blocks
- Liquidity sweeps
- Internal structure (4-hour levels)

**Technical Indicators:**
- Moving averages for trend
- RSI for overbought/oversold
- MACD for momentum
- Volume for conviction

### Multi-Timeframe FVG Analysis

Use FVGs across multiple timeframes:

1. **Daily chart**: Identify major FVGs
2. **4-hour chart**: Find smaller FVGs
3. **1-hour chart**: Trade the fill of 4-hour FVGs
4. **5-minute chart**: Fine-tune entry within hourly FVG

**Benefit:** Higher probability trades when smaller FVGs align with larger timeframe gaps

## Trading FVG Scenarios

### Scenario 1: Bullish FVG Fill

**Setup:**
- ES gapped up from 4500 to 4520 overnight
- FVG exists: 4500-4520
- Price pulls back to 4515 (testing FVG)
- Signal: Buy the dip toward FVG

**Execution:**
1. Wait for pullback to 4510-4515
2. Place limit buy at 4503 (within FVG)
3. Stop: 4498 (below FVG)
4. Target: 4540 (above gap)
5. Result: Profitable fill trade

### Scenario 2: Bearish FVG Rejection

**Setup:**
- EURUSD gapped down from 1.1000 to 1.0980
- FVG exists: 1.0980-1.1000
- Price bounces to 1.0990 (testing FVG)
- Signal: Short the resistance at FVG

**Execution:**
1. Wait for bounce to 1.0995-1.1000
2. Place limit sell at 1.0997 (within FVG)
3. Stop: 1.1005 (above FVG)
4. Target: 1.0970 (below gap)
5. Result: Mean reversion trade

### Scenario 3: FVG as Support/Resistance

**Dynamic Support:**
- Bullish FVG zone identified
- Price oscillates within the zone
- Acts as repeated bounce point
- Provides multiple entry opportunities

**Dynamic Resistance:**
- Bearish FVG zone identified
- Price tests zone repeatedly
- Acts as repeated rejection point
- Provides multiple short opportunities

## Advanced FVG Techniques

### FVG Mitigation

When FVGs are partially filled:
- **Incomplete fills**: Zone might partially fill then reverse
- **Overshoot**: Price might overshoot then pull back
- **Chop**: Multiple small fills within larger gap
- **Watch for these patterns** in your backtesting

### FVG Chasing

Identify patterns where FVGs tend to fill quickly:
1. **After overnight gaps**: Often fill within hours
2. **After large moves**: Tend to fill next session
3. **In trending markets**: Fill against trend (pullbacks)
4. **In ranging markets**: Fill as zones flip between S/R

### FVG-Block Confluence

Combine with ICT order blocks:
- **FVG + block**: When FVG forms at block, high probability
- **Multiple timeframe**: FVG on multiple timeframes = stronger setup
- **Accumulation zones**: Blocks build near FVGs

## Indicator Settings for Different Strategies

### Day Trading Settings

- **Minimum gap size**: 5 pips (aggressive)
- **Opacity**: 40% (lighter, less cluttered)
- **Timeframes**: 5-min and 15-min
- **Alert**: Yes (notify when price approaches)

### Swing Trading Settings

- **Minimum gap size**: 20 pips (avoid noise)
- **Opacity**: 60% (more visible)
- **Timeframes**: 1-hour and 4-hour
- **Historical**: Show last 30 days of gaps

### Scalping Settings

- **Minimum gap size**: 2 pips (very aggressive)
- **Opacity**: 30% (background only)
- **Timeframes**: 1-min and 5-min
- **Real-time alerts**: Enabled for instant notification

## Backtesting FVG Strategies

### Testing Methodology

1. **Enable FVG indicator**
2. **Scan for gaps** at session start
3. **Document FVGs**: Note zones and sizes
4. **Set execution rules**: Define entry/exit at FVG
5. **Track results**: Log trades and outcomes

### Performance Metrics to Track

- **Fill probability**: What % of FVGs actually fill?
- **Avg time to fill**: How long before FVG fills?
- **Win rate on fills**: % of profitable FVG trades
- **Best timeframes**: Which timeframes have best FVG setups?
- **Best sessions**: Which market sessions have best gaps?

### Documentation Template

For each FVG trade in backtesting:
- **Gap details**: Size, timeframe, type (bullish/bearish)
- **Age**: How old when traded
- **Entry**: Price and order type used
- **Exit**: Price, reason for exit
- **Result**: Profit/loss and R-multiple
- **Notes**: What worked, what didn't

## Common FVG Trading Mistakes to Avoid

1. **Trading every gap**: Not all FVGs are profitable
2. **Ignoring confirmation**: Need additional signals
3. **Wrong timeframe**: Trading FVG on wrong timeframe
4. **No risk management**: Always use stops
5. **Gap-opening trades**: Avoid trading right at gap open
6. **Exhaustion gaps**: Some gaps don't fill for long time
7. **Against strong trend**: FVG fills work better with trend

## FVG Indicator Limitations

Be aware of:
- **Lagging data**: FVGs form after the gap occurs
- **Multiple fills**: Complex gaps with partial fills
- **News gaps**: Economic data can prevent fill
- **Overnight gaps**: May not fill for days
- **Timeframe dependency**: Same gap looks different on different timeframes

---

## See also
- [How to Create a Backtesting Session](./create-backtesting-session.md)
- [Multiple Symbols and Multiple Charts](./multiple-symbols-charts.md)
- [Backtesting Indicators Overview](./backtesting-indicators.md)
