---
title: My Expired Option Trades Are Showing as Open
description: How to fix expired options still showing as open positions in TradeZella
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/6082670-my-expired-option-trades-are-showing-as-open
  md: https://www.tradezella.com/help-center/troubleshooting/expired-options-open.md
---

# My Expired Option Trades Are Showing as Open

If your expired option contracts are still showing as open positions in TradeZella, this is a common issue that can be resolved. Learn how to identify and fix expired options showing as open trades.

## Why Options Show as Open

Options can remain open in TradeZella for several reasons:

- **Not Marked as Expired**: TradeZella doesn't automatically detect expiration
- **Manual Entry Needed**: Manually entered options require manual closing
- **Import Issues**: Broker sync may not have imported expiration data
- **Exercise or Assignment**: Options were exercised/assigned but not marked closed
- **System Delay**: Broker data not updated in TradeZella yet
- **Rolled Position**: Option was rolled to next contract but not closed

## Identifying Expired Options

### Check Expiration Dates

1. Go to your **Trade Journal**
2. Look at your open positions
3. Check the **Expiration Date** column
4. Any date in the past = expired
5. Expired contracts should be closed, not open

### Checking Position Status

1. Click on an open option trade
2. View trade details
3. See the expiration date
4. If today's date is after expiration, it's expired
5. Status should show "Closed" or "Expired"

## How to Close Expired Options

### Automatic Sync (Synced Accounts)

If your account is connected to your broker:

1. Go to your account settings
2. Check **"Sync Status"** or **"Auto-Sync"** settings
3. Force a manual sync:
   - Click **"Sync Now"** button
   - Check if expired options update
4. Wait for sync to complete
5. Refresh your Trade Journal
6. Expired options may auto-close after sync

If they still show as open, you may need to manually close them.

### Manual Closure (Manual Entry or Failed Sync)

To manually close an expired option:

1. Go to your **Trade Journal**
2. Find the expired option trade
3. Click the trade to open details
4. Click **"Close Trade"** or **"Edit Trade"**
5. Choose closing method:
   - **Expired/Worthless**: For options expiring worthless
   - **Assigned**: If stock was assigned (calls) or put
   - **Exercised**: If you exercised the option
   - **Custom Close**: Manually enter closing price

### Recording Expiration

1. In the trade details, find the close method
2. Select **"Expired"** or **"Worthless Expiration"**
3. Set the close date to expiration date
4. Set closing price:
   - Zero for worthless puts/calls
   - Or actual value if partially preserved
5. Add any fees or adjustments
6. Click **"Save"** or **"Close Trade"**

### Bulk Closing Expired Options

To close multiple expired options at once:

1. In **Trade Journal**, filter for options
2. Select expired options using checkboxes
3. Click **"Bulk Actions"**
4. Select **"Close Multiple Trades"**
5. Set close method: **"Expired"**
6. Confirm closing price (usually $0)
7. Click **"Apply to All"**
8. All selected trades close at once

## Recording Assignments and Exercises

### Option Assignment

When a short option is assigned:

1. Open the **option trade** details
2. Find close method options
3. Select **"Assigned"**
4. Set assignment date (usually expiration date)
5. Confirm shares assigned (usually 100)
6. If assigned shares need closing:
   - Record stock position separately
   - Or link to stock closing trade
7. Save the assignment

### Option Exercise

When you exercise an option you own:

1. Open the **option trade** details
2. Select **"Exercised"** as close method
3. Set exercise date
4. Confirm shares or contracts
5. If stock received/delivered:
   - Record stock trade separately
   - Or link stock transaction
6. Save the exercise

## Checking Broker Data

### Synced Account Issues

If your broker sync shows expired options as open:

1. Log into your broker platform directly
2. Check if options show as closed there
3. If closed at broker but open in TradeZella:
   - Your sync may be out of date
   - Try syncing again
   - Contact Support if persistent

### Recent Expirations

For options that expired recently:

- Broker data may take 24-48 hours to sync
- TradeZella may not have latest data yet
- Check back tomorrow
- Manually close if needed for accuracy

### Third-Friday Expirations

Standard options expire on third Friday of each month:

- March, June, September, December: Third Friday
- All other months: Standard third Friday
- Some brokers update slowly after expiration
- Give 1-2 days for sync to catch up

## Impact on Performance

Open expired options affect:

- **Open Position P&L**: Shows unrealized loss on expired options
- **Account Statistics**: Skewed by open losing positions
- **Risk Metrics**: Inflated by positions that should be closed
- **Accuracy**: Your performance report is inaccurate until closed

Closing them updates all performance metrics immediately.

## Common Scenarios

### Sold Call Expires Worthless

Expected behavior:
1. Call you sold expires worthless
2. You keep the premium
3. Position should close at $0 profit
4. Status: Closed/Expired

If still open:
1. Manually close the trade
2. Set close price to $0
3. Closing profit should equal premium received

### Bought Put Expires Worthless

Expected behavior:
1. Put you bought expires worthless
2. You lose the premium paid
3. Position closes at loss
4. Status: Closed/Expired

If still open:
1. Manually close
2. Set close price to $0
3. Loss equals premium paid

### Spread Expires Partially

If you had a spread (bought and sold):

1. Both legs need closing
2. If only one leg appears open, find the pair
3. Close both legs to complete the spread
4. Ensure profit reflects all commissions

## Preventing Future Issues

### Enable Auto-Sync

If available for your broker:

1. Go to **Account Settings**
2. Enable **"Automatic Broker Sync"**
3. Set sync frequency (real-time or hourly)
4. Sync will auto-close expired options
5. Monitor for sync issues

### Manual Expiration Tracking

For manual trading:

1. Keep calendar of expiration dates
2. Close trades on/before expiration
3. Review open trades regularly
4. Close anything past expiration date
5. This prevents data pile-up

### Import Correctly

When importing trades:

1. Include expiration/close data
2. Don't skip closed positions
3. Verify imports completed successfully
4. Review new imports for accuracy
5. Close anything not already closed

## When to Contact Support

If expired options still show as open after:

1. Manual closing attempts
2. Multiple sync attempts
3. 48 hours of auto-sync
4. Broker data confirms closure

Contact TradeZella Support with:
- Account name
- Option symbol and expiration date
- Screenshot of open position
- Screenshot from broker showing closure
- Date expired

## FAQ

**Q: Can I recover profit from options I didn't close?**
A: Once closed, the trade is accurate. Missing closure means incorrect P&L until closure is recorded.

**Q: Why didn't my broker sync auto-close them?**
A: Some brokers' sync data is delayed or incomplete. TradeZella requires explicit close data.

**Q: Will expiration hurt my stats permanently?**
A: No, once closed, all metrics recalculate correctly.

**Q: How do I close options assigned/exercised into stock?**
A: Close the option as assigned/exercised, then separately record the stock trade.

---

## See also
- [Why Are My Thinkorswim Trades Not Syncing?](thinkorswim-not-syncing.md)
- [Why Are My Interactive Brokers Trades Not Syncing?](interactive-brokers-not-syncing.md)
- [I See My Trades as Duplicates in TradeZella](duplicate-trades.md)
