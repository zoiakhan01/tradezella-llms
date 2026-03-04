---
title: Why Are My Interactive Brokers Trades Not Syncing?
description: Troubleshoot Interactive Brokers trade synchronization issues with TradeZella
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/6492635-why-are-my-interactive-brokers-trades-not-syncing-to-tradezella
  md: https://www.tradezella.com/help-center/troubleshooting/interactive-brokers-not-syncing.md
---

# Why Are My Interactive Brokers Trades Not Syncing?

If your Interactive Brokers trades aren't syncing properly to TradeZella, follow this troubleshooting guide to identify and resolve the issue.

## Understanding Interactive Brokers Sync

### How IB Sync Works

Interactive Brokers syncing with TradeZella:

- **API Connection**: TradeZella uses IB's API to pull data
- **Account Link**: Your IB account authorized for data access
- **Trade Import**: Trades fetched from IB servers
- **Periodic Updates**: Updates happen on scheduled intervals
- **Manual Options**: Can force sync manually anytime

### Required for IB Sync

To sync Interactive Brokers:

- **Active IB Account**: Account must be open and funded
- **Trader Workstation**: May need TWS running (depends on integration)
- **API Enabled**: IB API access must be enabled
- **Account Authorization**: Permission granted to TradeZella
- **Network Connection**: Internet connection required

## Common Causes of IB Sync Issues

### Account or Access Issues

Problems with your IB account itself:

- **Account Inactive**: Account closed or in liquidation
- **Account Suspended**: Suspended for compliance or other reason
- **Access Restricted**: Account has API restrictions
- **Not Enabled**: Account type doesn't support API
- **Paper Account**: Paper trading may have different settings

### API Configuration Issues

Problems with Interactive Brokers API settings:

- **API Not Enabled**: Disabled in account settings
- **IP Restriction**: IB blocking TradeZella's IP
- **Firewall**: Your firewall blocking connection
- **Permissions**: Insufficient permissions for data access
- **Account Permission**: Specific account not authorized

### TWS Platform Issues

If your setup requires Trader Workstation:

- **TWS Offline**: Workstation not running
- **Session Expired**: TWS session timed out
- **Connection Lost**: Network issue broke connection
- **Version Outdated**: TWS needs update
- **Paper Account**: May require TWS to be running

### Credentials and Authorization

Your authentication with IB:

- **Expired Token**: Authorization token expired
- **Password Changed**: Changed IB password
- **2FA Issues**: Two-factor authentication problem
- **Account ID Wrong**: Using incorrect account ID
- **Revoked Access**: You revoked TradeZella access at IB

### Data Issues from IB

Problems with data IB is sending:

- **API Outage**: IB's API temporarily down
- **Data Lag**: Delayed trade data from IB
- **Incomplete Data**: Missing fields in data
- **Scheduled Maintenance**: IB doing maintenance
- **System Issues**: IB experiencing technical problems

## Troubleshooting Steps

### Step 1: Verify Your IB Account Works

1. Log into Interactive Brokers account portal
2. Or open Trader Workstation if using that
3. Verify you can access your account
4. Check that account status is active
5. Look for any restrictions or alerts
6. Verify the account type supports API
7. If issues here, contact IB first

### Step 2: Check API Status at IB

1. Log into IB Account Management
2. Go to **Settings** > **API**
3. Verify API is **enabled**
4. Check **Account Access Level**:
   - Limited: May restrict data access
   - Full: Full access to data
5. Look for **Trusted IPs** or firewall settings
6. Verify TradeZella's IP isn't blocked (if IP restriction exists)
7. If blocked, add TradeZella IP or remove restriction

### Step 3: Check Sync Status in TradeZella

1. Go to **Accounts** section
2. Find your Interactive Brokers account
3. Click to view account details
4. Look for **Sync Status** indicator
5. Note when last sync occurred
6. Read any error message displayed
7. Click error details for more information

### Step 4: Force Manual Sync

1. In your IB account settings in TradeZella
2. Look for **"Sync Now"** button
3. Click to manually trigger sync
4. Wait 30-60 seconds for attempt
5. Watch for status to update
6. Note any error message
7. Repeat if it appears to be temporary error

### Step 5: Disconnect and Reconnect

Re-authorize your account:

1. Go to **Account Settings**
2. Find **"Disconnect IB Account"** or **"Revoke Access"**
3. Click to disconnect (data remains in TradeZella)
4. Click **"Connect Interactive Brokers"** or **"Add IB Account"**
5. Redirected to IB login page
6. Log in with your IB credentials
7. Grant permission to TradeZella
8. Return to TradeZella
9. Verify sync now works

### Step 6: Update IB Credentials

If you recently changed your password:

1. Go to **Account Settings**
2. Find **"Update Credentials"** or **"Edit Account"**
3. Enter your updated IB username
4. Enter your new password
5. Save changes
6. Try syncing again

### Step 7: Check Network/Firewall

1. Verify your internet connection is working
2. Open other websites to confirm
3. If using VPN, try disabling it temporarily
4. Check if your firewall allows TradeZella
5. Try connecting from different network (mobile hotspot)
6. Try at different time if network congested

### Step 8: Enable TWS if Required

If integration requires Trader Workstation:

1. Download latest version of TWS from IB website
2. Install or update to latest version
3. Open Trader Workstation
4. Log in with your credentials
5. Ensure it stays open during sync
6. Return to TradeZella and try sync

## Specific Error Resolution

### "Account Not Found" or "Invalid Account ID"

1. Verify your IB account ID/number
2. Check if you have multiple accounts at IB
3. Ensure you're selecting correct account
4. Account ID format usually: UXXXXX
5. Disconnect and reconnect, select correct account

### "API Not Enabled"

API access is disabled at IB:

1. Log into IB Account Management online
2. Go to **Account Settings** > **API**
3. Find **"Enable API"** option
4. Toggle ON to enable
5. May need to agree to API terms
6. Save changes
7. Return to TradeZella
8. Try syncing again

### "Access Denied" or "Permission Denied"

Insufficient permissions configured:

1. Log into IB Account Management
2. Go to **API** > **Settings**
3. Check **Account Access Level**
4. Should be set to **"Full"** or **"LiveTrading"**
5. If set to Limited, change to Full
6. Save changes
7. Return to TradeZella
8. Reconnect and try sync

### "Connection Failed" or "Timeout"

Connection can't reach IB's servers:

1. Wait a few minutes; may be temporary
2. Check your internet connection
3. Try pinging IB server (if technical)
4. Check if IB is having issues
5. Try from different location/network
6. Disable VPN if using one
7. Check firewall allows connection

### "TWS Session Not Available"

Trader Workstation connection issue:

1. Ensure TWS is open and logged in
2. If closed, open TWS
3. Check TWS login is still active
4. If logged out, log back in
5. Keep TWS running during sync
6. May need to restart TWS
7. Try sync again

### "Market Data Subscription Required"

Some data requires active subscriptions:

1. Not typically issue for trade sync
2. May affect option/detailed data
3. Check your IB market data subscriptions
4. Ensure subscriptions are active
5. Contact IB if subscriptions missing

## Interactive Brokers Account Types

### Individual Accounts

- Standard IB account
- API typically enabled by default
- Full market data access included
- Most straightforward to sync

### Advisor/Account Manager

- May have different API permissions
- May require specific setup
- Contact IB if having issues
- Permissions may be restricted

### Paper Trading

- Separate from live account
- May have different API access
- Check if paper account API enabled
- May need separate sync setup

## Preventing Future Sync Issues

### Monitor Regularly

1. Check sync status weekly
2. Note when last successful sync was
3. Watch for error messages
4. Act quickly if issues appear
5. Don't let problems persist

### Maintain Security

1. Use strong IB password
2. Don't change password without updating TradeZella
3. Update credentials in TradeZella immediately after password change
4. Keep 2FA secure
5. Monitor account for unauthorized access

### Keep Settings Updated

1. Verify API still enabled periodically
2. Check that IB doesn't disable API
3. Monitor IB communications about API
4. Keep account info current at IB
5. Respond to any IB security alerts

### Update TradeZella

1. Keep TradeZella updated
2. Updates may include IB integration improvements
3. Check for app updates regularly
4. Don't delay critical updates

## When to Contact Support

Contact TradeZella Support if:

1. Sync fails after all troubleshooting steps
2. Error message is unclear
3. Disconnect/reconnect doesn't work
4. Multiple IB accounts all failing to sync
5. Never synced successfully

Provide Support with:
- Error message (screenshot helpful)
- When it last synced successfully
- Steps you've already tried
- IB account type (individual/advisor/paper)
- Whether IB account itself works

## Contact Interactive Brokers

Contact IB if:

1. IB account itself isn't working
2. Can't log into IB accounts portal
3. Can't enable API or getting permission errors
4. Account is restricted or suspended
5. IB API appears to be down

IB Support:
- Website: https://www.interactivebrokers.com
- Phone: 1-877-885-4685
- Account Management portal support chat

## After Sync Restoration

Once sync is working:

1. **Check Connection**: Verify sync runs automatically
2. **Backfill Data**: May import recent missed trades
3. **Monitor**: Watch for errors over next 24 hours
4. **Verify**: Check one or two trades match IB data
5. **Ongoing**: Monitor weekly to catch issues early

## Sync Frequency

You can control sync schedule:

1. Go to **Account Settings**
2. Find **"Sync Frequency"** setting
3. Options may include:
   - Real-time
   - Every 15 minutes
   - Hourly
   - Daily
4. More frequent = more data usage
5. Adjust based on your trading volume

---

## See also
- [Why Are My Thinkorswim Trades Not Syncing?](thinkorswim-not-syncing.md)
- [Resolving TOS/Charles Schwab Account Sync Failure Issues](schwab-sync-issues.md)
- [I See My Trades as Duplicates in TradeZella](duplicate-trades.md)
