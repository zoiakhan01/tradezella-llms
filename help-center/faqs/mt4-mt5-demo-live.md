---
title: Does TradeZella Support Both Demo and Live Accounts for MT4/MT5 Integration?
description: Yes, TradeZella supports both demo and live MT4/MT5 accounts
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/8042672-does-tradezella-support-both-demo-and-live-accounts-for-mt4-mt5-integration
  md: https://www.tradezella.com/help-center/faqs/mt4-mt5-demo-live.md
---

# Does TradeZella Support Both Demo and Live Accounts for MT4/MT5 Integration?

Yes, TradeZella fully supports both demo and live MetaTrader 4 (MT4) and MetaTrader 5 (MT5) accounts through direct API integration. Whether you're trading a demo account to practice and test strategies, or executing live trades with real capital, TradeZella can import and track all your trades from both account types. This flexibility allows traders to seamlessly switch between demo and live trading while maintaining accurate records and analytics in TradeZella.

The MT4/MT5 integration imports trades with complete historical data, commission information, spread details, and all other transaction specifics. Both demo and live trades are tracked side-by-side in TradeZella, allowing you to compare performance between paper trading and real money trading. This is particularly valuable for traders who want to validate their strategies on demo before risking capital, then transition to live trading with confidence that TradeZella will continue tracking performance accurately.

## MT4/MT5 Integration Overview

### What Is Supported
- **MetaTrader 4 (MT4):** All versions and broker variants
- **MetaTrader 5 (MT5):** All versions and broker variants
- **Demo Accounts:** Paper trading accounts with virtual money
- **Live Accounts:** Real money trading accounts
- **Multiple Accounts:** Import trades from multiple MT4/MT5 accounts simultaneously

### What Gets Imported
- All executed trades (buy/sell orders that filled)
- Entry price, exit price, quantity, and direction
- Entry date/time and exit date/time with precision
- Profit/loss calculation per trade
- Commissions, spreads, and fees
- Symbol/instrument information
- Account balance and equity at time of trade
- Overnight/weekend gaps and slippage
- Pending orders and order modifications

### What Doesn't Get Imported
- Pending orders that never fill (by design)
- Cancelled orders
- Rejected orders
- Internal account transfers or deposits/withdrawals (can be added manually if needed for context)

## Setting Up MT4/MT5 Integration

### Prerequisites
1. Active TradeZella account (create one if needed)
2. Active MT4 or MT5 account with a broker
3. Ability to access your MT4/MT5 account credentials
4. Stable internet connection

### Integration Steps

**Step 1: Access Integration Settings**
1. Log into TradeZella
2. Navigate to **Settings > Broker Connections**
3. Look for **"MetaTrader 4/MT5"** option
4. Click **"Connect New Account"**

**Step 2: Select Account Type**
1. Choose: **Demo Account** or **Live Account**
2. Select MetaTrader version: **MT4** or **MT5**
3. Select your broker from dropdown list (hundreds supported)
4. Click **"Continue"**

**Step 3: Enter Credentials**
1. Enter your MT4/MT5 server address
   - Example: "ICMarkets-Demo" or "ICMarkets-Live"
   - Your broker provides this in your MT4/MT5 terminal
2. Enter your Account Number (login)
   - Your numeric account ID from the MT4/MT5 terminal
3. Enter your Password
   - Your master password (not investor password)
4. Confirm credentials and click **"Connect"**

**Step 4: Permission Authorization**
1. TradeZella requests read-only access to your account
2. You must authorize this permission
3. Click **"Authorize"** to proceed
4. Authorization typically completes within seconds

**Step 5: Configure Import Settings**
1. Select: **Full History** or **Recent Trades**
2. Full History: Imports all trades ever taken on the account
3. Recent Trades: Imports last 30/60/90 days (faster initial setup)
4. Choose import frequency: **Real-time, Hourly, Daily**
5. Click **"Complete Setup"**

**Step 6: Initial Import**
1. TradeZella begins importing your trading history
2. First import may take minutes for large histories
3. You'll receive confirmation once complete
4. Your trades appear in Trade Journal
5. Analytics and metrics calculate automatically

## Demo Account Setup Specifics

### Demo Account Benefits for TradeZella Users

**Strategy Testing:** Validate your trading strategy before risking real money. Import demo trades into TradeZella to analyze performance on paper.

**Learning:** Practice using TradeZella's analytics while trading demo, so you're familiar with the platform before going live.

**Comparison:** Keep both demo and live accounts connected. Later compare your demo performance to live performance to understand the psychological difference.

**Risk-Free Experimentation:** Test new strategies on demo, tracked in TradeZella, to see if they have edge before deploying capital.

### Connecting Demo Account
1. In MT4/MT5, note your demo server address (e.g., "DemoServer" or "Broker-Demo")
2. In TradeZella, follow integration steps but select **"Demo Account"**
3. Enter demo account credentials
4. Authorize and import
5. Demo trades immediately appear in TradeZella labeled as demo

### Demo Trade Identification
- TradeZella marks demo trades in the trade journal
- Can filter to show only demo or only live trades
- Account designation shows "Demo" or "Live" in account selection

## Live Account Setup Specifics

### Security Considerations

**Password Safety:** TradeZella uses industry-standard encryption and never stores your password in plain text.

**Read-Only Access:** TradeZella only reads your account data. It cannot place, modify, or close trades without your direct action in MT4/MT5.

**Credential Protection:** Your login credentials are encrypted and stored securely. TradeZella never logs into your account to place trades automatically.

**Two-Factor Authentication:** Some brokers support 2FA; TradeZella accommodates this during initial connection.

### Connecting Live Account
1. In MT4/MT5, note your live server address (e.g., "LiveServer" or "Broker-Real")
2. In TradeZella, follow integration steps but select **"Live Account"**
3. Enter live account credentials
4. Authorize and import
5. Live trades immediately appear in TradeZella labeled as live

### Permissions Review
- Before authorizing, review what TradeZella accesses
- Verify that you're granting read-only access only
- Confirm you're connecting to the correct live server
- Check your broker's website to verify TradeZella is a recognized partner

## Managing Multiple MT4/MT5 Accounts

### Adding Multiple Accounts
1. You can connect multiple MT4/MT5 accounts simultaneously
2. Each account appears separately in Trade Journal
3. Can be same broker (multiple accounts) or different brokers
4. Example: MT4 forex account + MT5 futures account + MT4 demo account

### Switching Between Accounts
1. In Trade Journal, use **Account Filter**
2. Select which account(s) to display
3. Metrics recalculate for selected accounts only
4. Compare performance across accounts

### Mixed Demo/Live Tracking
1. Connect both demo and live accounts to TradeZella
2. Filter to view them separately or combined
3. Compare demo performance to live performance
4. Analyze: Are you trading better on demo vs. live? By how much?

## Demo vs. Live Comparison Analysis

### Why Traders Compare

**Psychological Difference:** Many traders perform worse live than on demo due to emotional pressure. Comparing helps quantify this.

**Slippage Impact:** Demo trades might fill perfectly; live trades may have slippage. Comparison shows actual execution quality.

**Strategy Validation:** If strategy works on demo but fails on live, suggests psychological or execution issue.

**Risk Management:** Some traders trade more conservatively on live than demo. Comparison reveals this behavior.

### Setting Up Comparison Analysis
1. Connect both demo and live accounts to TradeZella
2. Create two filter views:
   - **View 1:** Demo account, selected date range
   - **View 2:** Live account, same date range
3. Compare metrics side-by-side:
   - Win rate (demo vs. live)
   - Average win/loss (demo vs. live)
   - Trade expectancy (demo vs. live)
   - R-multiple distribution
4. Analyze differences and identify improvement areas

### Example Comparison
**Demo Trading (Last 30 days):**
- Trades taken: 50
- Win rate: 58%
- Average win: $320
- Average loss: $280
- Expectancy: +$58 per trade

**Live Trading (Same 30 days):**
- Trades taken: 25 (half the frequency)
- Win rate: 50%
- Average win: $200
- Average loss: $400
- Expectancy: -$50 per trade

**Analysis:** Live trading shows:
- Reduced frequency (fear reducing trades taken)
- Lower win rate (possibly worse entries)
- Smaller wins, larger losses (poor risk management under pressure)
- Negative expectancy (opposite of demo strategy)

## Troubleshooting MT4/MT5 Integration

### Connection Issues

**"Cannot Connect to Server"**
- Verify server address is correct (check MT4/MT5 terminal)
- Ensure internet connection is active
- Check if your broker's server is down
- Confirm account number is correct format

**"Invalid Credentials"**
- Double-check account number (numeric only)
- Verify password is correct (case-sensitive)
- Ensure you're using master password, not investor password
- Try resetting password in MT4/MT5 if unsure

**"Authorization Denied"**
- Broker may not support third-party integrations
- Contact your broker to enable API access
- Some brokers require manual approval for integrations

### Import Issues

**"Trades Not Importing"**
- Check if initial import is still processing (may take time for large histories)
- Verify import frequency is set (real-time, hourly, or daily)
- Confirm TradeZella still has authorization
- Try re-authorizing connection

**"Missing Recent Trades"**
- If import frequency is daily, it takes until next day to appear
- Change to real-time or hourly for faster updates
- Manual import may be needed for immediate data

**"Incorrect P&L"**
- Some brokers quote prices differently; verify entry/exit prices match MT4/MT5
- Commission calculations may differ; check if commissions are included
- Overnight gaps may affect P&L calculations
- Contact TradeZella support if discrepancy persists

### Account Disconnect

**Auto-Reconnection:** TradeZella automatically reconnects if connection drops

**Manual Reconnection:**
1. Go to **Settings > Broker Connections**
2. Find disconnected account
3. Click **"Reconnect"**
4. Re-enter credentials if needed
5. Re-authorize if prompted

## Best Practices

**Start with Demo:** Connect demo account first to test the integration and become familiar with TradeZella.

**Validate Then Go Live:** Once confident in TradeZella and your strategy, connect live account.

**Keep Both Connected:** Maintain both demo and live accounts in TradeZella for comparative analysis.

**Review Regularly:** Check imported trades weekly to verify accuracy and ensure integration is working.

**Use TradeZella Analytics:** Leverage TradeZella's superior analytics vs. MT4/MT5's built-in reporting. This is where the real value is.

**Document Changes:** If you modify your strategy, note in TradeZella so you can analyze impact on performance.

---

## See also
- [How to Edit Trades in TradeZella](/help-center/faqs/how-to-edit-trades.md)
- [How to Filter Your Trades in TradeZella](/help-center/faqs/how-to-filter-trades.md)
- [What Trading Assets Are Supported?](/help-center/faqs/supported-trading-assets.md)
