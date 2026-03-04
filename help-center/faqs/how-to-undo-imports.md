---
title: How to Undo Imports in TradeZella
description: Steps to reverse or undo trade imports if incorrect data was uploaded
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/7898222-how-to-undo-imports-in-tradezella
  md: https://www.tradezella.com/help-center/faqs/how-to-undo-imports.md
---

# How to Undo Imports in TradeZella

Accidentally imported trades with incorrect data? TradeZella provides several methods to undo imports and recover your account to a previous state. Whether you imported duplicate trades, trades with wrong prices, or data from the wrong broker, you have options to correct the situation without losing all your trading history. The undo functionality is designed to be straightforward while maintaining data integrity.

Understanding how to properly undo imports is essential for maintaining accurate trading records in TradeZella. This process differs depending on whether you need to undo a recent import, delete specific trades from an import batch, or restore your entire account. TradeZella keeps detailed records of all imports, making it possible to identify and remove problematic data with precision.

## Method 1: Undo Recent Import

The quickest way to undo an import is immediately after completing it:

1. After the import completes, look for the **"Undo Import"** notification that appears at the top of the screen
2. Click the **"Undo"** button within the notification banner
3. TradeZella will immediately reverse the import and restore your account to its pre-import state
4. Your previous data will be restored exactly as it was before the import

**Important:** This undo notification typically appears for 5-10 seconds after import completion. Once the notification disappears, you'll need to use alternative methods.

## Method 2: Delete Trades from Import History

If you need to remove specific trades from an import batch that's already been processed:

1. Navigate to **Settings > Import History** in your account
2. Locate the import batch you want to undo or modify (imports are listed with timestamp and number of trades)
3. Click on the import entry to expand details and see all trades from that batch
4. Select the trades you want to delete (use checkboxes next to each trade)
5. Click the **"Delete Selected Trades"** button
6. Confirm the deletion when prompted
7. TradeZella will remove only those trades and recalculate all your metrics

**Note:** This method preserves other trades while removing only the problematic ones, which is useful if you imported a mixture of good and bad data.

## Method 3: Full Account Rollback

For more serious issues where you need to revert your entire account to a previous date:

1. Go to **Settings > Account & Data**
2. Scroll to the **"Account Rollback"** section
3. Click **"View Restore Points"**
4. You'll see a list of available restore points (snapshots of your account from previous dates)
5. Select the date/time you want to restore to
6. Click **"Restore to This Point"**
7. Review the trades that will be removed/restored and confirm
8. TradeZella will reset your account state to the selected restore point

Restore points are automatically created daily, so you typically have 30+ days of restore options available.

## Method 4: Delete Individual Trades

If you only need to remove one or two problematic trades:

1. Navigate to your **Trade Journal** or **Trades** tab
2. Find the trade(s) you want to delete
3. Click the three-dot menu icon next to the trade
4. Select **"Delete Trade"**
5. Confirm the deletion
6. The trade will be removed and metrics recalculated immediately

## Preventing Import Errors

### Before Importing
- **Review CSV/Excel files** in a spreadsheet program first to verify data accuracy
- **Check decimal places** for prices and quantities to ensure correct formatting
- **Verify dates** are in the correct format expected by TradeZella
- **Test with small batch** of trades first if importing from a new broker or format

### During Import
- **Map columns correctly** when prompted during the import wizard
- **Verify preview data** before finalizing the import
- **Check for duplicates** if importing from multiple sources

### After Import
- **Review summary statistics** immediately after import
- **Spot-check several trades** to ensure prices and dates are correct
- **Compare total trades count** with your broker statement

## Common Import Issues

**Duplicate Trades:** If you imported the same trades twice, use Method 2 to delete the duplicate batch and keep only one copy.

**Incorrect Prices:** Prices sometimes get corrupted during import. Delete the affected trades and re-import with corrected data.

**Wrong Broker Data:** If you imported trades from the wrong broker account, use Method 3 for full rollback or Method 2 to delete the entire incorrect batch.

**Formatting Errors:** If column mapping was incorrect, undo the import and retry with proper column selection.

---

## See also
- [How to Edit Trades in TradeZella](/help-center/faqs/how-to-edit-trades.md)
- [How to Filter Your Trades in TradeZella](/help-center/faqs/how-to-filter-trades.md)
- [What Trading Assets Are Supported?](/help-center/faqs/supported-trading-assets.md)
