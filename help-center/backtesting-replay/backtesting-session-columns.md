---
title: What Information Is Displayed in the Backtesting Session Tab Columns?
description: Understanding the data columns displayed in your backtesting sessions list
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/8800490-what-information-is-displayed-in-the-backtesting-my-session-tab-columns-for-backtesting
  md: https://www.tradezella.com/help-center/backtesting-replay/backtesting-session-columns.md
---

# What Information Is Displayed in the Backtesting Session Tab Columns?

The Backtesting Sessions tab displays key information about each of your backtesting sessions in organized columns. Understanding these columns helps you quickly evaluate session performance and manage your backtesting library effectively.

## Primary Session Columns

### Session Name
- **Description**: The custom name you assigned to the session
- **Why it matters**: Identifies the session for easy reference
- **Format**: User-defined (e.g., "ES Scalp Strategy v2", "EURUSD Swing Test")
- **Editable**: Yes - click to rename sessions
- **Sort capability**: Alphabetically sortable

### Symbol
- **Description**: The trading instrument used in the session
- **Examples**: ES, NQ, EURUSD, GBPJPY, AAPL, BTC
- **Why it matters**: Quick identification of what market was traded
- **Format**: Standard symbol notation
- **Filter capability**: Filter sessions by symbol

### Timeframe
- **Description**: The candle timeframe used for analysis
- **Options**: M1, M5, M15, M30, H1, H4, D1, W1, MN
- **Why it matters**: Determines trading style (scalping, day trading, swing)
- **Sort capability**: Sortable by timeframe
- **Format**: Standardized timeframe abbreviations

### Date Range
- **Description**: The historical period covered by the session
- **Format**: MM/DD/YYYY - MM/DD/YYYY
- **Example**: 01/01/2024 - 02/28/2024
- **Why it matters**: Shows the market conditions and timeframe tested
- **Duration**: Total days of data included

## Performance Metrics Columns

### Total Trades
- **Description**: The total number of trades executed in the session
- **Range**: 0 to unlimited trades
- **Why it matters**: Indicates trading frequency and activity level
- **Example**: 25 trades, 152 trades
- **Use case**: Identify sample size for strategy validation

### Winning Trades
- **Description**: Number of profitable trades
- **Calculation**: Trades with P&L > 0
- **Format**: Numeric count
- **Related metric**: Used to calculate win rate

### Losing Trades
- **Description**: Number of losing trades
- **Calculation**: Trades with P&L < 0
- **Format**: Numeric count
- **Context**: Balance against winning trades

### Win Rate
- **Description**: Percentage of trades that were profitable
- **Calculation**: (Winning Trades / Total Trades) × 100
- **Format**: Percentage (0-100%)
- **Example**: 55%, 42.5%
- **Benchmark**: Generally, 50%+ is considered good

### Profit Factor
- **Description**: Ratio of gross profit to gross loss
- **Calculation**: Total Profit / Total Loss
- **Format**: Decimal (1.0 = breakeven)
- **Example**: 1.5 means $1.50 profit for every $1 loss
- **Interpretation**: Higher is better (2.0+ is excellent)

## Profitability Columns

### Gross Profit
- **Description**: Total profit from all winning trades combined
- **Format**: Currency amount (e.g., $5,250)
- **Calculation**: Sum of all positive P&L
- **Example**: $15,000 total profit from wins
- **Notes**: Doesn't account for losing trades

### Gross Loss
- **Description**: Total loss from all losing trades combined
- **Format**: Currency amount (e.g., -$2,100)
- **Calculation**: Sum of all negative P&L
- **Example**: -$8,500 total loss from losses
- **Notes**: Always displayed as negative value

### Net Profit (P&L)
- **Description**: Overall profit or loss for the entire session
- **Calculation**: Gross Profit + Gross Loss (algebraically)
- **Format**: Currency amount (green if positive, red if negative)
- **Example**: +$6,500, -$2,300
- **Importance**: The bottom line of session performance
- **Sort capability**: Sortable (highest/lowest profit)

## Risk and Return Columns

### Maximum Drawdown
- **Description**: The largest peak-to-trough decline in equity
- **Format**: Currency amount and percentage
- **Example**: -$5,200 (15.3%)
- **Why it matters**: Indicates worst-case loss scenario
- **Risk metric**: Critical for risk management

### Sharpe Ratio
- **Description**: Risk-adjusted return metric
- **Calculation**: (Return - Risk-free rate) / Standard deviation
- **Interpretation**: Higher is better
- **Example**: 1.5, 2.3
- **Benchmark**: Above 1.0 is good, above 2.0 is excellent

### Average Win
- **Description**: Average profit per winning trade
- **Calculation**: Gross Profit / Winning Trades
- **Format**: Currency amount
- **Example**: $600 per win
- **Use case**: Understand typical winner size

### Average Loss
- **Description**: Average loss per losing trade
- **Calculation**: Gross Loss / Losing Trades
- **Format**: Currency (shown as negative)
- **Example**: -$425 per loss
- **Risk/Reward**: Compare to Average Win for R:R ratio

## Additional Information Columns

### Duration
- **Description**: Total time spent in this session
- **Format**: Hours, minutes
- **Example**: 4 hours, 23 minutes
- **Use case**: Identify active backtesting sessions

### Last Updated
- **Description**: When the session was last modified
- **Format**: Date and time
- **Example**: Today at 2:30 PM, 3 days ago
- **Sorting**: Sortable by recency

### Status
- **Description**: Current state of the session
- **Options**:
  - Active (currently trading)
  - Completed (finished trading)
  - Paused (temporarily stopped)
  - Archived (stored for reference)
- **Color coding**: Different colors for each status

## Column Customization

### Showing/Hiding Columns

1. Click **Column Settings** (gear icon) in session header
2. Toggle columns on/off based on your preferences
3. Save your column layout
4. Layout persists across sessions

### Recommended Column Combinations

**Quick Overview**
- Session Name, Symbol, Total Trades, Win Rate, Net Profit

**Detailed Analysis**
- Session Name, Symbol, Date Range, Total Trades, Win Rate, Profit Factor, Net Profit, Max Drawdown

**Risk Management Focus**
- Session Name, Total Trades, Average Win, Average Loss, Max Drawdown, Sharpe Ratio

## Sorting and Filtering

### Sort Options
- Click column header to sort ascending/descending
- Multi-column sorting available
- Sorting persists in your view

### Filter Options
- Filter by symbol
- Filter by date range
- Filter by performance (positive/negative P&L)
- Filter by status (active, completed, archived)

## Understanding Session Columns at a Glance

A strong backtesting session typically shows:
- Win rate between 40-60%
- Profit factor above 1.5
- Positive net profit
- Maximum drawdown within acceptable risk levels
- Sharpe ratio above 1.0

---

## See also
- [How to Create a Backtesting Session](./create-backtesting-session.md)
- [Do Backtested Trades Get Automatically Journaled in TradeZella?](./auto-journal-backtesting.md)
- [Understanding Different Order Types in TradeZella Backtesting](./order-types-backtesting.md)
