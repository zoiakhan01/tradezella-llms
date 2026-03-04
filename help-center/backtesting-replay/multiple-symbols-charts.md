---
title: How to Backtest Multiple Symbols and Multiple Charts
description: Setting up and using multiple symbols and charts simultaneously in backtesting
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/9641861-how-to-backtest-multiple-symbols-and-multiple-charts
  md: https://www.tradezella.com/help-center/backtesting-replay/multiple-symbols-charts.md
---

# How to Backtest Multiple Symbols and Multiple Charts

TradeZella allows you to backtest multiple symbols simultaneously with multiple chart layouts. This is essential for analyzing correlations, spread trading, and multi-instrument strategies.

## Why Multi-Symbol Backtesting?

Multi-symbol backtesting enables:
- **Correlation analysis**: Compare two related instruments
- **Spread trading**: Backtest calendar spreads, currency crosses, commodity spreads
- **Sector analysis**: Trade related stocks or currency pairs
- **Risk management**: Monitor hedging instruments
- **Portfolio analysis**: Test multiple positions simultaneously
- **Market structure**: Compare primary and secondary timeframes across symbols

## Setting Up Multiple Charts

### Method 1: Creating a New Chart Window

1. **Start in your backtesting session**
2. Look for the **"Add Chart"** or **"+" button** in the chart area
3. Click to create a new chart window
4. Select your new symbol
5. Choose the timeframe for this chart
6. Second chart appears alongside your primary chart

### Method 2: Using the Layout Options

1. Click **Layout** button in the toolbar
2. Select your preferred multi-chart layout:
   - **2-Column layout**: Side-by-side charts
   - **2-Row layout**: Top and bottom charts
   - **Grid layout**: 2x2 arrangement (4 charts)
   - **Custom layout**: Define your own arrangement
3. Confirm layout selection
4. Charts appear in your chosen layout

### Method 3: Chart Management Menu

1. Click **Chart Settings** (gear icon)
2. Select **Manage Charts**
3. Choose **Add New Chart**
4. Enter the symbol and timeframe
5. Adjust chart position in layout

## Selecting Multiple Symbols

### Supported Symbol Combinations

You can combine any symbols in your backtesting session:
- **Forex + Forex**: EURUSD and GBPUSD (correlated pair)
- **Futures + Futures**: ES and NQ (index correlation)
- **Forex + Futures**: EURUSD and 6E (same market, different instruments)
- **Stocks + Stocks**: AAPL and MSFT (sector correlation)
- **Crypto + Crypto**: BTC and ETH (market correlation)
- **Mixed**: ES with VIX, EURUSD with GLD, etc.

### Entering Multiple Symbols

For the primary chart:
1. Enter first symbol (e.g., "ES")
2. Select timeframe (e.g., "1-hour")

For additional charts:
1. Click "Add Chart"
2. Type the second symbol (e.g., "NQ")
3. Select its timeframe
4. Charts load simultaneously

## Multi-Chart Layouts

### 2-Column Layout

**Best for:**
- Comparing correlated pairs
- Spread analysis (ES vs NQ)
- Primary and secondary chart analysis

**Setup:**
- Left chart: Primary symbol
- Right chart: Secondary symbol
- Both visible side-by-side
- Easy comparison

### 2-Row Layout

**Best for:**
- Timeframe analysis
- Volume analysis below price
- Indicator analysis

**Setup:**
- Top chart: Primary symbol
- Bottom chart: Related instrument
- Vertical alignment
- Stacked analysis

### 2x2 Grid Layout

**Best for:**
- Complex correlation analysis
- Multiple timeframe comparison
- Portfolio backtesting

**Setup:**
- Four independent charts
- Each with different symbol/timeframe
- Comprehensive market view
- Track multiple positions

## Synchronizing Charts

### Time Synchronization

Multiple charts stay automatically synchronized:
- All charts show the same date/time period
- When you navigate one chart, all update together
- Jump to date on one chart affects all others
- Playback speed applies to all charts simultaneously

### Manual Synchronization

If charts drift:
1. Click **Sync Charts** button in toolbar
2. Select reference chart
3. All other charts align to that chart's time
4. Continues synchronization automatically

## Trading with Multiple Charts

### Executing Trades Across Symbols

You can trade multiple symbols in one session:

1. **Place trade on first chart**:
   - Click entry point on ES chart
   - Set quantity and order type
   - Confirm trade execution

2. **Place trade on second chart**:
   - Click entry point on NQ chart
   - Set quantity and order type
   - Execute trade on second symbol

3. **Both trades active simultaneously**:
   - Manage both positions
   - Close independently
   - Track correlated performance

### Order Entry on Multiple Charts

Each chart has its own trading controls:
- **Entry tools**: Click on each chart independently
- **Order parameters**: Set separately for each symbol
- **Position sizing**: Control size on each instrument
- **Exit levels**: Define stops/targets per symbol

## Multi-Symbol Trading Strategies

### Spread Trading

Trade the difference between two instruments:
1. Go long ES on primary chart
2. Go short NQ on secondary chart
3. Watch the spread between them
4. Close when target spread is hit

**Advantages:**
- Hedges directional risk
- Profits from correlation breakdown
- Lower overall portfolio drawdown

### Correlation Trading

Trade two correlated instruments:
1. Look for correlation breakdown
2. Long the stronger chart
3. Short the weaker chart
4. Re-entry when correlation recovers

**Example**: EURUSD and GBPUSD often move together; trade when correlation breaks down.

### Sector Trading

Trade multiple stocks in same sector:
1. Monitor sector trends on multiple charts
2. Trade strongest performer
3. Fade weakest performer
4. Capture sector rotation

### Risk Management

Use secondary chart as hedge:
1. Primary position: Long ES
2. Secondary position: Long VIX or TLT hedge
3. Monitor correlation
4. Adjust hedge as needed

## Analyzing Correlations

### Visual Correlation Analysis

Looking at two charts simultaneously:
- Identify when they move together
- Spot divergences from correlation
- Find leading indicators
- Predict likely next move

### Quantitative Analysis

TradeZella can overlay correlation data:
1. Add correlation indicator to second chart
2. Compare directional moves
3. Measure correlation coefficient
4. Document significant changes

### Documentation

Keep notes on correlation patterns:
- Write down correlation observations
- Document divergence patterns
- Track seasonal correlations
- Build strategy playbook

## Advanced Multi-Chart Features

### Chart Linking

Link charts together:
- Move one chart = other charts follow
- Share horizontal axis only
- Share vertical axis only
- Full synchronization

### Overlay Charts

Display one symbol over another:
1. Select overlay mode in chart options
2. Adjust chart opacity for layering
3. Compare price action directly
4. Identify support/resistance similarities

### Independent Analysis Per Chart

Each chart maintains:
- Independent indicators
- Separate notes and annotations
- Individual trade decisions
- Distinct entry/exit prices

## Keyboard Shortcuts for Multiple Charts

| Action | Shortcut |
|--------|----------|
| Switch between charts | Tab or Alt+Number |
| Add new chart | Ctrl+N or Cmd+N |
| Close current chart | Ctrl+W or Cmd+W |
| Sync all charts | Ctrl+S or Cmd+S |
| Maximize chart | F or double-click |

## Performance Analysis with Multiple Symbols

Your trading journal captures:
- Trades on each symbol independently
- Correlation between positions
- Combined portfolio performance
- Win rate per symbol
- P&L per symbol and combined

### Multi-Symbol Session Summary

View aggregate metrics:
- Total trades across all symbols
- Combined P&L
- Win rate across all symbols
- Correlation effects on performance

## Tips for Effective Multi-Chart Backtesting

1. **Start simple**: Begin with 2 highly correlated instruments
2. **Match timeframes**: Use same timeframe on related charts initially
3. **Color coding**: Use chart colors to distinguish instruments
4. **Notes**: Document correlation observations
5. **Regular breaks**: Multi-chart analysis is demanding; take breaks
6. **Review sessions**: Analyze completed sessions for pattern learning

---

## See also
- [How to Create a Backtesting Session](./create-backtesting-session.md)
- [Jump to a Specific Candle in Backtesting](./jump-to-candle.md)
- [Keyboard Shortcuts in Backtesting](./keyboard-shortcuts-backtesting.md)
