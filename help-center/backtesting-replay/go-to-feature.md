---
title: What Is the "Go-To Feature" Within TradeZella?
description: Using the Go-To feature to jump to specific dates and times in backtesting
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/8866853-what-is-the-go-to-feature-within-tradezella
  md: https://www.tradezella.com/help-center/backtesting-replay/go-to-feature.md
---

# What Is the "Go-To Feature" Within TradeZella?

The "Go-To" feature is a powerful navigation tool in TradeZella that allows you to instantly jump to a specific date and time within your backtesting session. This feature saves significant time when analyzing specific market events or reviewing particular trading periods.

## What the Go-To Feature Does

The Go-To feature enables you to:
- Jump directly to a specific date in your backtesting session
- Navigate to exact times on intraday charts
- Skip past irrelevant market data instantly
- Find specific price levels or events quickly
- Resume backtesting from a precise point

Instead of playing through hours or days of market data, you can jump directly to the exact moment you want to analyze.

## Accessing the Go-To Feature

### Method 1: Keyboard Shortcut

Press **Ctrl+G** (Windows) or **Cmd+G** (Mac) to open the Go-To dialog while backtesting.

### Method 2: Menu Navigation

1. Click the **Navigation** menu in the backtesting toolbar
2. Select **Go to Date/Time**
3. The Go-To dialog box appears

### Method 3: Toolbar Button

1. Look for the **Go-To button** (calendar or clock icon) in the main backtesting toolbar
2. Click to open the date/time picker
3. Enter your desired date and time

## Using the Go-To Feature

### Step 1: Open the Go-To Dialog

Use any of the access methods above to open the Go-To interface.

### Step 2: Enter Your Target Date

Enter the date you want to jump to:
- **Format**: MM/DD/YYYY or MM/DD/YYYY HH:MM
- **Example**: 02/15/2024 or 02/15/2024 14:30
- **Flexibility**: The feature understands various date formats

### Step 3: Specify Time (Optional)

For intraday analysis, include the time:
- **Format**: HH:MM (24-hour or 12-hour with AM/PM)
- **Example**: 14:30 (2:30 PM), 09:15 (9:15 AM)
- **Precision**: Exact to the minute

### Step 4: Execute the Jump

1. Click **Go** or press **Enter**
2. TradeZella instantly navigates to that date/time
3. The chart displays the candle at that moment
4. You're positioned exactly where you want to be

## Common Use Cases

### Analyzing Specific Market Events

Jump to a date when:
- A major economic news event occurred
- A support/resistance level was tested
- A currency pair hit a new high/low
- A specific trading setup appeared

**Example**: "Go to 03/14/2024" to see how the market reacted to the Fed announcement.

### Finding Missed Trades

Quickly locate trading opportunities you might have missed:
1. Use Go-To to jump to the relevant date
2. Review the setup at normal speed
3. Analyze why you missed it
4. Document lessons learned

### Reviewing Specific Sessions

Jump to different time periods to test multiple strategies:
1. Start session at date 1
2. Test strategy from date 1 to date 2
3. Use Go-To to jump to date 3
4. Test same strategy in different market conditions

### Analyzing Market Reversals

Find pivot points and reversal dates:
1. Know the date a reversal occurred
2. Jump to that exact date
3. Analyze the price action leading up to it
4. Study the reversal pattern in detail

## Go-To with Multiple Timeframes

### Using Go-To Across Timeframes

The Go-To feature works consistently across different timeframes:
- **1-minute chart**: Jump to exact minute and time
- **Daily chart**: Jump to specific date
- **Weekly chart**: Jump to specific week
- **Monthly chart**: Jump to specific month

### Multi-Timeframe Analysis

1. Backtest on primary timeframe (e.g., 4-hour)
2. Identify interesting candles
3. Use Go-To to jump to that same point on daily chart
4. Review higher timeframe context
5. Confirm strategy validity across timeframes

## Navigation After Using Go-To

Once you've jumped to a specific date:

### Resume Normal Backtesting
- Use **Play** button to continue from that point
- Adjust playback speed as needed
- Click **Pause** to examine specific candles
- Use arrow keys to move candle-by-candle

### Jump Again
- Press **Ctrl+G** to jump to another date
- Explore multiple time periods in sequence
- Build comprehensive understanding of market conditions

### Return to Current Position
- Click **Current** or **Now** to return to starting point
- Or use Go-To to jump back to your original date

## Go-To Tips and Tricks

### Keyboard Shortcuts with Go-To
- **Ctrl+G**: Open Go-To dialog
- **Left arrow**: Previous candle (after jumping)
- **Right arrow**: Next candle (after jumping)
- **Spacebar**: Play/Pause from jump point

### Quick Navigation
- Jump to round dates (01/01/2024, 06/01/2024)
- Use month transitions (01/31/2024 to 02/01/2024)
- Jump to week boundaries
- Navigate to known trade setups

### Combining with Chart Tools
- Jump to a date
- Use ICT FVG tool to identify gaps
- Analyze order blocks at specific dates
- Review support/resistance at historical levels

## Advanced Go-To Usage

### Scanning Multiple Dates Efficiently

1. Create a list of dates to analyze
2. Use Go-To to jump to first date
3. Analyze setup and note results
4. Go-To the next date on your list
5. Build a comprehensive analysis across multiple periods

### Testing Strategy Rules on Specific Dates

1. Identify dates with potential setups
2. Jump to each date individually
3. Test your entry/exit rules manually
4. Document which dates provided valid trades
5. Refine strategy based on date-specific patterns

### Date Range Analysis

Jump between specific date ranges:
- Bull markets: Jump to months showing strong trends
- Range-bound markets: Find consolidation periods
- Volatile markets: Locate high volatility dates
- Quiet markets: Identify low activity periods

## Go-To Limitations

### What Go-To Cannot Do
- Cannot jump to times when markets are closed
- May skip to next available candle if exact time is between candles
- Does not work across different symbols (stay within same symbol)
- Cannot jump beyond your session's date range

### If No Data Exists

If you jump to a date with no trading data:
- System automatically moves to next available candle
- Message indicates jump to next available data point
- Useful for skipping weekends or holidays

## Keyboard Shortcut Reference

| Action | Windows | Mac |
|--------|---------|-----|
| Open Go-To | Ctrl+G | Cmd+G |
| Play/Pause | Spacebar | Spacebar |
| Next Candle | Right Arrow | Right Arrow |
| Previous Candle | Left Arrow | Left Arrow |

---

## See also
- [Jump to a Specific Candle in Backtesting](./jump-to-candle.md)
- [Keyboard Shortcuts in Backtesting](./keyboard-shortcuts-backtesting.md)
- [Backtesting Window Overview](./backtesting-window.md)
