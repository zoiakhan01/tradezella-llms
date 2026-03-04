---
title: Why Are My Thinkorswim Trades Not Syncing?
description: Troubleshoot Thinkorswim trade synchronization issues with TradeZella
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/6492631-why-are-my-thinkorswim-trades-not-syncing
  md: https://www.tradezella.com/help-center/troubleshooting/thinkorswim-not-syncing.md
---

# Why Are My Thinkorswim Trades Not Syncing?

If your Thinkorswim trades aren't syncing to TradeZella, here are the most common causes and how to fix them.

## Understanding Sync

### What Sync Does

Thinkorswim sync in TradeZella:

- **Imports Trades**: Automatically pulls trades from your Thinkorswim account
- **Real-Time Updates**: Brings in fills as trades complete
- **Ongoing**: Continues pulling new trades periodically
- **Account Balance**: May update account balance info
- **Historical**: Can import past trades on initial sync

### When Sync Fails

Sync failures show as:

- No new trades appearing
- "Last sync: [hours ago]" with error
- Red warning icon on account
- Specific error message when trying to sync
- Trades visible in Thinkorswim but not TradeZella

## Common Causes of Sync Failures

### Authentication Issues (Most Common)

Your Thinkorswim credentials need refreshing:

- **Expired Token**: Connection token expired
- **Password Changed**: Updated password at TD Ameritrade/Schwab
- **2FA Changed**: Two-factor authentication settings modified
- **Account Permissions**: API access was disabled
- **Device Revoked**: Thinkorswim revoked TradeZella device access

### Thinkorswim Disconnection

Your API connection isn't active:

- **Thinkorswim Closed**: Platform needs to be open for sync
- **Lost Connection**: Network disconnection broke link
- **Session Timeout**: Thinkorswim session expired
- **API Not Enabled**: API access disabled in TOS settings
- **Rate Limited**: Too many connection attempts

### Account or Platform Issues

Problems specific to your account:

- **Account Type**: Certain account types don't support API
- **Restricted**: Account has restrictions preventing API access
- **On Hold**: Account suspended or on hold
- **Paper Trading**: May have limitations
- **Account Closed**: If you closed the account, sync stops

### Thinkorswim Data Issues

Problems with data Thinkorswim is sending:

- **Incomplete Data**: Missing required fields
- **API Malfunction**: Thinkorswim API not returning data
- **Scheduled Maintenance**: TOS doing maintenance
- **System Issues**: TOS experiencing technical problems

## Troubleshooting Steps

### Step 1: Verify Thinkorswim is Working

1. Open Thinkorswim desktop platform directly
2. Log in to verify credentials work
3. Check that you can view trades
4. Ensure the account shows trades
5. If TOS is down, wait for restoration
6. If you can't log in, reset password first

### Step 2: Check Sync Status in TradeZella

1. Go to your **Accounts** section
2. Find your Thinkorswim account
3. Click on it to view settings
4. Look for **"Sync Status"** indicator
5. Note last successful sync time
6. Read any error message shown
7. Click error for more details if available

### Step 3: Force a Manual Sync

1. In your account settings
2. Look for **"Sync Now"** button
3. Click it to manually trigger sync
4. Wait 30-60 seconds for it to attempt
5. Watch for status update
6. Note any error message
7. Try again if temporary error

### Step 4: Disconnect and Reconnect

Refresh your authorization:

1. Go to **Account Settings**
2. Find **"Disconnect"** or **"Remove Authorization"**
3. Click to disconnect (data stays in TradeZella)
4. Click **"Connect Thinkorswim"** or **"Reconnect"**
5. You'll be redirected to Schwab/TD login
6. Log in with your credentials
7. Grant permission to TradeZella
8. Return to TradeZella
9. Sync should now work

This refreshes your authentication token.

### Step 5: Update Your Credentials

If you recently changed your password:

1. Go to **Account Settings**
2. Find **"Update Credentials"** or similar
3. Enter your updated Thinkorswim username
4. Enter your new password
5. Save changes
6. Try sync again

### Step 6: Check Thinkorswim API Settings

In your Thinkorswim account settings:

1. Log into Thinkorswim
2. Go to **Settings** > **API**
3. Verify API is **enabled**
4. Check if any connected apps are listed
5. Look for TradeZella in the list
6. If TradeZella is there, make sure it's enabled
7. If missing, you may need to re-authorize

If API is disabled:
1. Enable API in Thinkorswim settings
2. Return to TradeZella
3. Try syncing again

### Step 7: Check Internet Connection

1. Verify your internet is working
2. Try opening other websites
3. If connection is down, fix that first
4. If using VPN, try disabling it
5. Check if firewall is blocking TradeZella
6. Try connecting from different network if possible

## Specific Error Resolution

### "Authentication Failed" or "Invalid Credentials"

Your login information is incorrect:

1. Verify your Thinkorswim username
2. Check if you recently changed password
3. Ensure you're using correct account (if multiple)
4. Reset password at Schwab if forgotten
5. Disconnect and reconnect (Step 4)

### "API Not Enabled"

API access is disabled:

1. Log into Thinkorswim
2. Go to **Settings** > **API**
3. Enable API for third-party connections
4. Look for **"Enable API"** option
5. May need to accept terms
6. Return to TradeZella and sync

### "Connection Timeout"

Thinkorswim not responding in time:

1. Wait a few minutes; retry
2. Ensure Thinkorswim is open and responsive
3. Check if TOS is undergoing maintenance
4. Try reconnecting
5. If persistent, contact Schwab

### "Account Restricted"

Your account has restrictions:

1. Log into Thinkorswim
2. Check **Account Settings** for restrictions
3. API access may be restricted
4. Contact Schwab Support if restricted
5. May be temporary due to security review

### "No Data Available"

Thinkorswim isn't returning data:

1. Ensure you have trades in your account
2. Try broader date range in manual sync settings
3. Wait and retry (may be temporary)
4. Check Thinkorswim shows trades for same period
5. Verify you're syncing the correct account

## Thinkorswim-Specific Settings

### Choosing Account to Sync

If you have multiple Thinkorswim accounts:

1. Each account needs separate setup in TradeZella
2. When connecting, select specific account
3. Verify you're syncing the right account
4. Can sync multiple accounts to separate TradeZella accounts

### Paper vs. Live Trading

If using paper trading account:

- Verify sync supports paper accounts
- Some integrations only support live accounts
- Check if you need to enable API for paper trades
- May have different settings

### TD Ameritrade Merger

If recently migrated from TD Ameritrade to Schwab:

- Account setup may have changed
- Login credentials may differ
- May need to re-authorize Thinkorswim
- Contact Schwab if auth issues persist

## Preventing Future Sync Issues

### Monitor Sync Status

1. Check sync status weekly
2. Note when last successful sync occurred
3. Watch for error messages
4. Act quickly if you see failures
5. Don't let issues persist for days

### Maintain Account Security

1. Use strong, unique passwords
2. Don't change password without updating TradeZella
3. If you change password, update TradeZella immediately
4. Keep 2FA secure
5. Update recovery methods

### Keep Thinkorswim Running

For real-time sync:

1. Keep Thinkorswim open during trading
2. Don't fully close the platform
3. Minimize if needed but keep active
4. Check connection status occasionally
5. Reconnect if you see disconnection

### Update Credentials Promptly

1. If you change Thinkorswim password, update TradeZella
2. Don't delay credential updates
3. Update immediately after password change
4. Verify sync works after updating

## When to Contact Support

Contact TradeZella Support if:

1. Sync still fails after all troubleshooting
2. Disconnecting and reconnecting doesn't work
3. You see an error code you don't understand
4. Sync worked but suddenly stopped
5. Multiple accounts all having same issue

Provide to Support:
- Error message (screenshot helpful)
- When sync last worked
- Steps already tried
- Whether Thinkorswim itself is working
- Your Thinkorswim account type (paper/live)

## Contact Schwab Support

Contact Charles Schwab/Thinkorswim if:

1. Thinkorswim itself isn't working
2. You can't log into Thinkorswim
3. API won't enable in settings
4. Account is restricted or suspended
5. You can't verify your own access

Schwab Support: 1-800-SCHWAB-1 (1-800-729-2225)

## After Sync Restoration

Once sync is working again:

1. **Automatic Resume**: Sync continues automatically
2. **Backfill**: May import recent trades you missed
3. **Monitor**: Watch for errors in next 24 hours
4. **Verify**: Check a few trades match Thinkorswim
5. **Regular Check**: Continue monitoring sync status

## Sync Frequency Settings

You can control how often sync happens:

1. Go to **Account Settings**
2. Find **"Sync Frequency"** or **"Auto-Sync"**
3. Options typically include:
   - Real-time (immediate)
   - Every 15 minutes
   - Hourly
   - Daily
4. More frequent = more data usage
5. Less frequent = may miss intraday trades

---

## See also
- [Why Are My Interactive Brokers Trades Not Syncing?](interactive-brokers-not-syncing.md)
- [Resolving TOS/Charles Schwab Account Sync Failure Issues](schwab-sync-issues.md)
- [I See My Trades as Duplicates in TradeZella](duplicate-trades.md)
