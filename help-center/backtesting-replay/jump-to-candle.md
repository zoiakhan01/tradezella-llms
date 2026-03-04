---
title: Jump to a Specific Candle in Backtesting
description: Navigate directly to a specific candle by date and time in backtesting
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/9688972-jump-to-a-specific-candle-in-backtesting
  md: https://www.tradezella.com/help-center/backtesting-replay/jump-to-candle.md
---

# Jump to a Specific Candle in Backtesting

The ability to jump directly to a specific candle in backtesting allows you to navigate instantly to any point in your trading data without playing through every candle. This feature is essential for efficient backtesting workflow.

## Understanding Candles in TradeZella

### What is a Candle?

A candle represents price action during a specific time period:
- **1-minute candle**: Price movement in one minute
- **5-minute candle**: Price movement in five minutes
- **1-hour candle**: Price movement in one hour
- **Daily candle**: Price movement in one day
- And so on for other timeframes

Each candle has:
- **Open**: Price at candle start
- **Close**: Price at candle end
- **High**: Highest price during period
- **Low**: Lowest price during period

## Methods to Jump to a Specific Candle

### Method 1: Using the Go-To Feature (Recommended)

The Go-To feature is the fastest way to jump to a specific candle:

1. **Press Ctrl+G** (Windows) or **Cmd+G** (Mac)
2. **Enter date and time** in the dialog box
3. **Format**: MM/DD/YYYY HH:MM or just MM/DD/YYYY
4. **Example**: 02/15/2024 14:30 jumps to 2:30 PM on Feb 15, 2024
5. **Click Go** or press Enter
6. Chart instantly displays the candle at that moment

### Method 2: Using the Timeline/Scroll Bar

1. **Locate the timeline** at the bottom of the chart
2. **Drag the scroll slider** left or right
3. Chart updates as you move the slider
4. Watch the date/time display change in real-time
5. Fine-tune position by clicking at specific points on timeline

### Method 3: Using the Date/Time Input Fields

1. **Look for date/time input fields** in the toolbar
2. **Click the date field** and enter your target date
3. **Click the time field** and enter your target time
4. **Press Enter** to jump to that candle
5. Chart updates to display the selected candle

### Method 4: Clicking Directly on the Chart

For a candle visible on screen:
1. **Hover over the candle** you want to analyze
2. **Click on the candle**
3. Chart locks to that candle
4. Detailed candle data appears
5. Ready for trade execution or analysis

## Candle Navigation Techniques

### Using Arrow Keys for Precision

After jumping to a general area:
1. **Right arrow key**: Move to next candle forward in time
2. **Left arrow key**: Move to previous candle backward in time
3. **Ctrl+Right**: Jump ahead multiple candles
4. **Ctrl+Left**: Jump back multiple candles
5. **Fine-tune**: Move one candle at a time to find exact entry point

### Keyboard Shortcuts for Candle Navigation

| Action | Shortcut |
|--------|----------|
| Jump to date/time | Ctrl+G or Cmd+G |
| Next candle | Right Arrow |
| Previous candle | Left Arrow |
| Next 5 candles | Shift+Right |
| Previous 5 candles | Shift+Left |
| Jump to current date | Ctrl+End or Cmd+End |
| Jump to start | Ctrl+Home or Cmd+Home |

## Finding Specific Types of Candles

### Identifying Key Candles

Before jumping, you might want to find:
- **Break of support/resistance**: Identify the date it broke
- **Reversal candles**: Pinbars, engulfing patterns
- **Economic data release**: Known news event dates
- **High volume candles**: Significant volume spikes
- **Gap candles**: Overnight or gap moves

### Using Chart Annotations

Mark important candles:
1. Jump to a significant candle
2. Add a marker or flag
3. Add a note explaining significance
4. Later, jump back to your marked candles

## Using Jump to Candle for Strategy Testing

### Testing Entry Signals

1. **Identify a potential setup** in your strategy
2. **Jump to that candle** using the date
3. **Examine the setup** in detail
4. **Place a test trade** at that candle
5. **Continue playing** to see if it works

### Analyzing Past Performance

1. **Review your trading journal**
2. **Note dates of your best trades**
3. **Jump to those candles** in backtesting
4. **Analyze the setups** to identify patterns
5. **Document lessons learned**

### Testing Multiple Scenarios

1. **Jump to date 1**: Test scenario in bullish market
2. **Analyze performance**
3. **Jump to date 2**: Test in bearish market
4. **Jump to date 3**: Test in ranging market
5. **Compare results** across different conditions

## Jump to Candle with Multiple Charts

### Synchronized Multi-Chart Navigation

When backtesting multiple symbols:
1. **Jump to date on primary chart**
2. **Secondary charts automatically sync** to same date
3. **All charts show the same candle** by time
4. **Compare setups** across multiple symbols simultaneously
5. **Symbols may be on different candles** if they have different closes

### Comparing Candle Patterns Across Symbols

1. **Jump to a date** where Symbol A had a significant candle
2. **Observe what Symbol B** was doing at same time
3. **Identify correlations** in candle patterns
4. **Spot divergences** when symbols break correlation
5. **Trade the divergence** if your strategy allows

## Tips for Efficient Candle Navigation

### Workflow Tips

1. **Start broad**: Jump to week of interest first
2. **Zoom in**: Use arrow keys to find exact candle
3. **Mark as you go**: Flag important candles
4. **Take notes**: Document what you observe
5. **Review later**: Return to marked candles in analysis phase

### Time-Saving Techniques

- **Batch similar jumps**: Jump to multiple setups of same pattern
- **Use bookmarks**: Save frequently-visited dates
- **Create jump list**: Write down dates to analyze before session
- **Speed up**: Use fastest playback between jumps
- **Pause at targets**: Jump to candle, pause, then analyze

## Exact Candle Timing

### Understanding Candle Timing

When you jump to a specific time:
- **The candle at that time is displayed**
- **You are positioned AT that candle**
- **NOT between candles**
- **Ready to trade on that candle**

### Example Scenarios

**Scenario 1: 1-Hour Chart**
- Jump to 02/15/2024 14:30
- You see the 2:30-3:30 PM candle
- Candle is complete or forming
- You can execute trades based on this candle

**Scenario 2: 5-Minute Chart**
- Jump to 02/15/2024 14:30
- You see the 14:30-14:35 candle
- Perfect for precise entry/exit analysis
- Fine-grained control over execution

## Limitations and Considerations

### What You Need to Know

- **Markets closed**: Jumping to weekend/holiday shows next available candle
- **Different timeframes**: Time jumps change which candle displays by timeframe
- **Within session range**: Can only jump within your session's date range
- **Data availability**: Only jumps to available data (forex 24/5, futures limited hours)

### If Candle Doesn't Exist

When jumping to a time with no data:
- System jumps to **next available candle**
- Message indicates "jumped to next available data"
- Useful for skipping market closures
- Prevents wasted navigation time

## Advanced Candle Jumping

### Creating Candle Analysis Sessions

1. **Backtest with multiple jumps**
2. **Document each jump location**
3. **Create list of candle dates**
4. **Analyze patterns across those candles**
5. **Build edge from pattern recognition**

### Identifying Personal Trade Setups

1. **Jump through months of data**
2. **Mark your high-probability setups**
3. **Create list of setup dates**
4. **Analyze common characteristics**
5. **Refine your trading rules**

---

## See also
- [What Is the "Go-To Feature" Within TradeZella?](./go-to-feature.md)
- [Keyboard Shortcuts in Backtesting](./keyboard-shortcuts-backtesting.md)
- [Backtesting Window Overview](./backtesting-window.md)
