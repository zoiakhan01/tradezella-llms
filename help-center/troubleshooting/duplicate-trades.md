---
title: I See My Trades as Duplicates in TradeZella
description: Identify and remove duplicate trades in your TradeZella journal
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/6153629-i-see-my-trades-as-duplicates-in-tradezella
  md: https://www.tradezella.com/help-center/troubleshooting/duplicate-trades.md
---

# I See My Trades as Duplicates in TradeZella

If you're seeing duplicate trades in your trade journal, this is often caused by importing the same trades multiple times or using overlapping data sources. Learn how to identify and remove duplicates.

## Why Duplicates Appear

Duplicates usually happen when:

- **Multiple Imports**: Imported the same file twice
- **Overlapping Periods**: Imported multiple files with date overlap
- **Broker Sync Issues**: Auto-sync imported data multiple times
- **Manual + Import Mix**: Manually entered trades then imported same ones
- **Merger/Roll Positions**: Positions rolled or merged showing as separate
- **Partial Fills**: Multiple entries for single multi-leg position
- **System Sync Delay**: Synced again before previous completed

## Identifying Duplicates

### Manual Visual Inspection

1. Go to your **Trade Journal**
2. Look for trades with:
   - Same symbol
   - Same entry date/time (or within seconds)
   - Same entry price
   - Same size (shares/contracts)
   - Same exit date and price
3. Compare trades that look identical
4. Check if all details match

### Duplicate Detection Tools

Some import methods show duplicates:

1. Before finalizing an import
2. TradeZella flags "Likely Duplicates"
3. Shows matched trades with percentages
4. 100% match = definite duplicate
5. 80-90% match = likely duplicate

Select which trades to import; skip identified duplicates.

### Filtering for Duplicates

To filter and view possible duplicates:

1. In **Trade Journal**, find filter options
2. Look for **"Show Duplicates"** or similar filter
3. Filter by date range of import
4. Or sort by symbol and date to spot duplicates
5. Manual review shows matching pairs

## How to Remove Duplicates

### Identifying Which to Delete

When you find duplicates:

1. Compare both trades carefully
2. Check which has more detail (keep this one)
3. Check import source - keep original if one is manual
4. Note the trade ID of the duplicate to delete

### Deleting Individual Trades

To delete a single duplicate:

1. Open the duplicate trade
2. Click **"Delete"** or the trash icon
3. Confirmation dialog appears:
   - "Are you sure?"
   - Shows trade details
4. Confirm deletion: **"Yes, Delete This Trade"**
5. Trade is permanently removed

Once deleted:
- P&L updates immediately
- All metrics recalculate
- Account balance adjusts
- Statistics refresh

### Bulk Duplicate Deletion

To delete multiple duplicates at once:

1. In **Trade Journal**, select all duplicate trades
2. Use checkboxes to select
3. Click **"Bulk Actions"** or **"Delete Multiple"**
4. Confirm trades selected
5. Click **"Delete All Selected"**
6. Confirm bulk deletion
7. All selected trades removed at once

## Preventing Duplicates

### Import Carefully

1. Check file dates before importing
2. Avoid importing overlapping date ranges
3. Keep track of what you've already imported
4. Review flagged duplicates before confirming import
5. Use "Skip Duplicates" option if available

### Managing Multiple Sources

If using multiple data sources:

1. Keep a list of what you've imported
2. Note dates and sources
3. Don't overlap import periods
4. Merge different sources (e.g., stocks + options) separately
5. Check for duplicates after each import

### Disabling Auto-Sync Temporarily

If manual importing:

1. Disable auto-sync from broker
2. Complete manual imports first
3. Then re-enable auto-sync
4. Prevents overlap from simultaneous imports

### Import Source Organization

Create a system:

1. Monthly imports: Import Jan 1-31, then Feb 1-28, etc.
2. CSV files: Name by date range ("trades-jan-2024.csv")
3. Broker sync: Once enabled, don't also manually import
4. Backup imports: Keep separate from main account

## Understanding Partial Fills

Sometimes duplicates aren't duplicates:

### Multiple Fill Parts

A large order might fill in parts:
- Trade 1: Buy 50 shares at 10:30am
- Trade 2: Buy 50 shares at 10:31am
- Both may look duplicate but are separate fills

### Identifying Partial Fills

1. Check timestamps: Are they seconds/minutes apart?
2. Check size: Does total equal expected position?
3. Review broker statement: Confirms if multiple fills
4. If multiple fills: Keep both (not duplicates)
5. Combine in TradeZella if you prefer single entry

### Merging Partial Fills

To combine multiple fills into one trade:

1. Some platforms offer "merge trades" option
2. Or manually delete partial fills
3. Re-enter as single larger trade
4. Use average entry price for combined entry
5. Or keep separate for detailed analysis

## Handling Options and Spreads

### Multi-Leg Spreads

A spread is multiple related legs:
- Long Call + Short Call = Call Spread (2 legs)
- Long Stock + Short Call = Covered Call (2 legs)

These may appear as separate trades if:
- Imported separately from broker
- Entered manually as individual legs
- System doesn't recognize relationship

To verify:
1. Check dates and times
2. If exact same time, likely same spread
3. Related symbols (same exp date)
4. If they're a matched pair, that's correct

### Options Rolled Positions

When rolling an option:
1. Close old contract
2. Open new contract
3. Two separate trades (not duplicate)
4. Different expiration dates
5. Both should appear in journal

Don't delete rollovers as duplicates.

## After Removing Duplicates

### Performance Recalculation

After deletion:
- Trade count reduces
- Win rate recalculates
- P&L updates immediately
- ROI adjusts
- Account statistics refresh

### Verify Accuracy

1. Check Trade Journal count matches broker
2. Compare total P&L with broker statements
3. Verify account balance reflects deletions
4. Review performance metrics make sense
5. Look for any remaining obvious duplicates

### Backup After Cleanup

Once cleaned up:
1. Export your corrected trade journal
2. Save backup copy
3. Provides recovery point
4. Ensures data safety

## Special Cases

### Dividend Adjustments

Some systems show dividends as trades:

1. Not duplicates, actual events
2. Important for P&L accuracy
3. Keep these separate
4. Don't delete as duplicates

### Corporate Actions

Stock splits, mergers, spinoffs:

1. May create multiple entries
2. Adjustment trades are real
3. Keep for accurate accounting
4. Don't remove as duplicates

### Assignment and Exercise

Options assigned or exercised:

1. Option trade closes
2. Stock trade opens (from assignment/exercise)
3. Two separate trades (not duplicates)
4. Both should be kept
5. Related but distinct events

## When to Contact Support

If you:

- Can't identify which is duplicate
- System won't delete trades
- Notice duplicate issues after import
- Have recurring duplicate problems
- System shows false duplicate warnings

Contact Support with:
- Account name
- Trade details (symbol, date, price)
- Screenshots of duplicates
- What you've already tried
- Import method used

---

## See also
- [Import History on TradeZella](../account-management/import-history.md)
- [Correcting Chart Entry and Exit Points](correcting-chart-points.md)
- [Why Are My Thinkorswim Trades Not Syncing?](thinkorswim-not-syncing.md)
