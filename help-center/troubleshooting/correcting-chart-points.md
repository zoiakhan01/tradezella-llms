---
title: Correcting Chart Entry and Exit Points
description: Adjust entry and exit price points in the TradeZella chart tool
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/6153644-correcting-chart-entry-and-exit-points-in-tradezella
  md: https://www.tradezella.com/help-center/troubleshooting/correcting-chart-points.md
---

# Correcting Chart Entry and Exit Points

The chart tool in TradeZella allows you to visually mark trade entry and exit points. If your entry or exit markers are incorrect, you can easily adjust them. This guide explains how to correct entry and exit points on your charts.

## Understanding Chart Entry and Exit Points

### What They Show

Entry and exit points on charts:

- **Entry Point**: Shows where you bought or sold (opening price)
- **Exit Point**: Shows where you closed the position (closing price)
- **Visual Markers**: Displayed as arrows or dots on price chart
- **Time Markers**: Show exact time of entry and exit
- **Profit/Loss Line**: Line connecting entry to exit shows direction

### Why They Matter

Accurate chart points:

- Show your actual trade execution
- Help you analyze your entries
- Show decision-making visually
- Identify pattern recognition
- Compare intended vs. actual prices
- Improve future trade planning

## Accessing the Chart Tool

To view and edit chart entry/exit points:

1. Go to your **Trade Journal**
2. Find the trade you want to review
3. Click the trade to open details
4. Look for **"Chart"** or **"View Chart"** button
5. Chart opens showing the trade on price bars

## Viewing Entry and Exit Points

The chart displays:

- **Price Bars**: OHLC (open, high, low, close) candles
- **Entry Marker**: Usually an arrow pointing up (long) or down (short)
- **Exit Marker**: Arrow showing close direction
- **Entry Time**: Timestamp of entry
- **Exit Time**: Timestamp of exit
- **Price Labels**: Shows entry and exit prices

## Correcting Entry Points

### Identifying Incorrect Entry

Entry points may be wrong if:

- Marker appears at wrong time on chart
- Price marked is different from actual filled price
- Marker is in the middle of candle but you bought at edge
- You remember buying at different price than shown
- Entry shows outside market hours

### Adjusting Entry Price

To change the entry price:

1. Open the trade details
2. Find the **"Entry Price"** field
3. Click to edit
4. Enter the correct price
5. Click **"Update"** or **"Save"**
6. Chart updates with new entry point

### Adjusting Entry Time

To change when the entry is marked:

1. In trade details, find **"Entry Time"** or **"Entry Date"**
2. Click to edit the time
3. Select the correct date and time
4. Confirm the change
5. Chart redraws with correct timing

### Adjusting Entry on Chart Directly

Some brokers allow direct chart editing:

1. Click on the chart area
2. Look for **"Edit"** mode or pencil icon
3. Click and drag the entry marker
4. Position it at correct price and time
5. Release to set new position
6. Changes save automatically

## Correcting Exit Points

### Identifying Incorrect Exit

Exit points may be wrong if:

- Exit marker is at wrong price
- Time is incorrect
- Closed differently (assignment vs. sale) than shown
- Price was slipped at market close
- Exit appears on wrong day

### Adjusting Exit Price

To change the exit price:

1. Open the trade details
2. Find **"Exit Price"** field
3. Edit to correct price
4. Update and save
5. Trade P&L recalculates automatically
6. Chart shows updated exit point

### Adjusting Exit Time

To change the exit timestamp:

1. In trade details, find **"Exit Time"** or **"Exit Date"**
2. Edit to correct date and time
3. Confirm changes
4. Chart redraws with correct exit timing

### Exit Adjustments for Partial Closes

If you partially closed a position:

1. First close: Original exit
2. Subsequent closes: May need separate records
3. In TradeZella, record full close at the final exit
4. Or break into multiple trades if tracking separately
5. Chart shows the final complete exit

## Common Correction Scenarios

### Gap Fill Entry

Scenario: You bought the open (before gap fill), but chart shows middle of opening range.

Fix:
1. Adjust entry price to your actual fill
2. Adjust entry time to correct time
3. Chart now reflects your actual entry
4. P&L updates correctly

### Late Exit Recording

Scenario: You closed the trade but recorded it later, chart position is wrong.

Fix:
1. Correct the exit time to when you actually closed
2. Update exit price to actual close price
3. If closed after hours, note that in trade comments
4. Chart reflects actual exit

### Wrong Direction (Long vs. Short)

Scenario: You marked a short position as long entry (or vice versa).

Fix:
1. This usually requires editing the trade type
2. Go to trade details and change position type
3. Entry/exit arrows reverse direction
4. Chart shows correct direction
5. P&L calculation updates

### Assignment/Exercise Conversion

Scenario: Option was exercised and shares assigned, but exit shows as option close.

Fix:
1. Option trade: Mark as "Exercised" instead of sale
2. Add stock trade separately if needed
3. Or edit option trade close method
4. Chart updates to show exercise instead of sale

## Verifying Corrections

After correcting entry/exit points:

1. **Check Chart**: Verify markers are at correct spots
2. **Check P&L**: Confirm profit/loss matches your records
3. **Check Time**: Verify times match your broker records
4. **Compare**: Cross-reference with broker statements
5. **Document**: Add notes if unusual circumstances

## Bulk Corrections

For multiple trades with same issue:

1. Go to **Trade Journal**
2. Filter for specific date or broker
3. Select multiple affected trades
4. Click **"Bulk Edit"**
5. Correct common field (e.g., entry time offset)
6. Apply to all selected
7. Verify results before saving

## Chart Viewing Options

To better see and correct points:

- **Zoom In**: See detail on price bars near entry/exit
- **Change Timeframe**: Switch to 15-min, hourly, or daily bars
- **Add Indicators**: MA, support/resistance lines
- **Overlays**: Compare with other trades or patterns
- **Annotations**: Add notes to key chart points

## Synced Broker Charts

For synced accounts (Schwab, Interactive Brokers):

- Chart data comes directly from broker
- May auto-populate entry/exit
- If broker data incorrect, may need manual correction
- Contact broker if data is consistently wrong
- Can override broker data in TradeZella

## Manual Entry Charts

For manually entered trades:

- No broker data to reference
- You control entry/exit accuracy
- Review trade notes if available
- Use memory/journal to verify
- Enter best-estimate if exact prices forgotten

## Tips for Accurate Entry/Exit Points

1. **Record Immediately**: Enter data right after closing
2. **Use Broker Data**: Check broker confirms and compare
3. **Keep Notes**: Write entry/exit prices and times
4. **Verify**: Cross-check against screenshots/statements
5. **Correct Early**: Don't let errors accumulate
6. **Review Regularly**: Weekly check for discrepancies

## When to Contact Support

Contact TradeZella Support if:

- Chart tool won't load
- Corrections don't save
- Entry/exit points won't update
- Broker data synced incorrectly
- Can't access chart for specific trade
- P&L not updating after correction

Include:
- Trade symbol and date
- Screenshot of issue
- What you've already tried
- Expected vs. actual values

---

## See also
- [I See My Trades as Duplicates in TradeZella](duplicate-trades.md)
- [Why Are My Thinkorswim Trades Not Syncing?](thinkorswim-not-syncing.md)
- [Resolving TOS/Charles Schwab Account Sync Failure Issues](schwab-sync-issues.md)
