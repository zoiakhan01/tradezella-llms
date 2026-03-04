---
title: Import History on TradeZella
description: View all past imports, see import details, undo imports if needed in TradeZella
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/6706087-import-history-on-tradezella
  md: https://www.tradezella.com/help-center/account-management/import-history.md
---

# Import History on TradeZella

Import History shows all past imports you've made into your TradeZella account. You can view details about each import, see what trades were added, and even undo imports if needed. This feature provides complete visibility into how your trade data was populated.

## Accessing Import History

To view your import history:

1. Navigate to your **"Accounts"** section
2. Select the account you want to review
3. Click on **"Settings"** or **"Account Settings"**
4. Look for **"Import History"** in the menu
5. Click to open the Import History panel

The Import History page shows a chronological list of all imports for the selected account.

## Understanding Import History

Each import record displays:

- **Import Date**: When the import occurred (timestamp)
- **Import Source**: Where data was imported from (broker, CSV file, etc.)
- **Number of Trades**: How many trades were imported in that batch
- **Success Status**: Whether the import completed successfully
- **Import Type**: Broker sync, CSV upload, manual import, etc.
- **User**: Who initiated the import (in multi-user accounts)

## Viewing Import Details

To see details about a specific import:

1. Find the import in your Import History list
2. Click on the import row or **"View Details"** button
3. A details panel opens showing:
   - Complete import timestamp
   - Source file name or broker name
   - List of all trades added in this import
   - Any errors or warnings that occurred
   - Number of successful vs. failed trades
   - Manual notes if you added any

### Import Details Include

- **Trade Symbols**: All stocks, options, or contracts imported
- **Date Range**: Earliest and latest trade dates in the import
- **Trade Types**: Mix of long, short, options trades, etc.
- **Status**: Completed, Partial, Failed
- **Warnings**: Any issues that might need attention
- **Duplicate Flags**: Trades that matched existing trades

## Undoing Imports

If you imported incorrect data, you can undo the import:

1. Find the import in **Import History** you want to undo
2. Click the **three-dot menu** next to the import
3. Select **"Undo Import"**
4. A confirmation dialog appears
5. Review what trades will be removed
6. Click **"Yes, Undo This Import"** to proceed

**Important**:
- Undoing an import removes ALL trades from that batch
- You cannot selectively undo specific trades from an import
- The undo is permanent and cannot be reversed
- Your account balance returns to its pre-import state

## Viewing Imported vs. Manual Trades

TradeZella distinguishes between:

- **Imported Trades**: Added via broker sync, CSV import, or file upload
- **Manual Trades**: Entered directly into TradeZella by you

In your Import History:
- Only imported trades appear in Import History
- Manual trades are not listed
- You can still see which trades came from which import

## Common Import Sources

### Broker Syncs

Automated imports from connected brokers:

- **Charles Schwab / Thinkorswim**: Real-time or periodic sync
- **Interactive Brokers**: Scheduled sync
- **Tradovate**: Automated data sync
- **Others**: Varies by broker

View which broker each import came from in the Import History.

### CSV Imports

Manual file uploads:

- Shows filename in Import History
- Date of upload
- Number of trades processed
- Any parsing errors

### API Connections

Third-party service imports:

- Shows the service name
- Timestamp of sync
- Number of trades added
- Connection status

## Managing Import Issues

### Duplicate Trades

If you see duplicates:

1. Check Import History for overlapping imports
2. Sometimes the same trades sync multiple times
3. You can undo the duplicate import
4. Or manually delete duplicate trades in your journal

### Partial Imports

If an import shows errors:

1. View the import details
2. See which trades failed to import
3. Check error messages for each failed trade
4. Possible causes:
   - Invalid data format
   - Missing required fields
   - Symbol not recognized

Partially imported data is saved; you can fix errors and re-import.

### Failed Imports

Complete import failures:

1. Check the error message in Import History
2. Common causes:
   - File format issues
   - Broker connection timeout
   - Invalid credentials
   - File corruption
3. Retry the import after fixing the issue

## Filtering Import History

Most Import History views allow filtering:

- **By Date**: Show imports from specific date range
- **By Source**: Show imports from specific broker or file
- **By Status**: Show successful, partial, or failed imports
- **By User**: Show imports by specific account user

Use filters to quickly find specific imports.

## Exporting Import History

To export your import history:

1. In **Import History**, look for **"Export"** button
2. Choose export format:
   - CSV file
   - PDF report
   - Excel spreadsheet
3. Click **"Export"**
4. File downloads to your computer

Useful for record-keeping and audit trails.

## Import History and Account Recovery

Import History is important for:

- **Account Audits**: See exactly what data was imported
- **Troubleshooting**: Identify when issues started
- **Recovery**: Find when specific trades were added
- **Compliance**: Maintain record of data sources

Keep your Import History intact for reference.

## Best Practices for Imports

1. **Review Before Importing**: Check file or sync settings
2. **Monitor First Imports**: Watch for errors on new imports
3. **Verify Data**: Spot-check trades after import
4. **Keep History**: Don't delete import history unnecessarily
5. **Document Sources**: Note where each import comes from
6. **Regular Syncs**: Set up periodic broker syncs if available

## Limitations

- Import History shows 12 months of data by default
- Older imports may be archived or deleted after extended time
- Individual import records cannot be modified (only undone entirely)
- Undone imports cannot be re-applied automatically

---

## See also
- [Creating an Account in TradeZella](creating-account.md)
- [Trade Settings Tab Explained](trade-settings.md)
- [Tag Management in TradeZella](tag-management.md)
