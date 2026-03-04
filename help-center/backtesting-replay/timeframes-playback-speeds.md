---
title: What Timeframes and Playback Speeds Can I Use in Backtesting?
description: Overview of available timeframes and playback speed options for backtesting
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/8800462-what-timeframes-and-playback-speeds-can-i-use-in-backtesting
  md: https://www.tradezella.com/help-center/backtesting-replay/timeframes-playback-speeds.md
---

# What Timeframes and Playback Speeds Can I Use in Backtesting?

TradeZella supports a comprehensive range of timeframes and playback speeds to accommodate different trading styles and analysis needs.

## Available Timeframes

TradeZella backtesting supports the following timeframes:

### Intraday Timeframes
- **1-minute (M1)**: For scalping and high-frequency strategies
- **5-minute (M5)**: Popular for day trading and breakout strategies
- **15-minute (M15)**: Intermediate day trading and swing entry timeframes
- **30-minute (M30)**: Extended intraday analysis
- **1-hour (H1)**: Standard hourly trading and analysis

### Swing and Position Trading Timeframes
- **4-hour (H4)**: Primary timeframe for swing traders
- **Daily (D1)**: Institutional-level price action analysis
- **Weekly (W1)**: Long-term trend identification
- **Monthly (MN)**: Strategic planning and market structure

## Playback Speed Options

Control the speed of market replay to simulate trading at different paces:

### Speed Settings
- **1x (Real-time speed)**: One second of real-time = one second of market data
- **2x (Double speed)**: Twice as fast as real-time
- **5x**: Five times faster than real-time
- **10x**: Ten times faster than real-time
- **20x**: Twenty times faster than real-time
- **Fastest (Unlimited)**: Skip through data as fast as your computer can handle

## Playback Speed Guidelines

**For Strategy Testing**: Use 10x to 20x speed to quickly review multiple trades and verify strategy logic without watching every candle form.

**For Detailed Analysis**: Use 1x to 2x speed when learning price action patterns or analyzing specific trade setups in detail.

**For Quick Reviews**: Use "Fastest" mode when scanning through session data to identify key moments to analyze further.

## Combining Timeframes and Speeds

The real power comes from combining timeframes effectively:

1. **Multi-timeframe analysis**: Backtest using a primary timeframe (e.g., 4-hour) while monitoring higher timeframes (daily structure) in adjacent charts
2. **Progressive speed adjustments**: Start at faster speeds, slow down when you find interesting setups, then speed back up
3. **Zoom navigation**: Jump between different date ranges at varying playback speeds

## Keyboard Shortcuts for Speed Control

- **Spacebar**: Play/Pause playback
- **Right arrow**: Next candle
- **Left arrow**: Previous candle
- **Number keys 1-9**: Adjust playback speed quickly

---

## See also
- [How to Create a Backtesting Session](./create-backtesting-session.md)
- [Keyboard Shortcuts in Backtesting](./keyboard-shortcuts-backtesting.md)
- [Jump to a Specific Candle in Backtesting](./jump-to-candle.md)
