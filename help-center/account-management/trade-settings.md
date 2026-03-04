---
title: Trade Settings Tab Explained
description: Understand per-account trade settings including calculation method, commissions, and breakeven range
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/8164984-trade-settings-tab-explained
  md: https://www.tradezella.com/help-center/account-management/trade-settings.md
---

# Trade Settings Tab Explained

The Trade Settings tab in your TradeZella account contains important configuration options that directly affect how trades are calculated and tracked. These settings determine your profit calculations, commission handling, and trading parameters.

## Accessing Trade Settings

To access Trade Settings:

1. Navigate to the **"Accounts"** section
2. Select your desired account
3. Click the **"Settings"** tab or icon
4. Look for **"Trade Settings"** in the left sidebar
5. The Trade Settings panel will open

## Main Settings Categories

### Profit Calculation Method

This setting determines how profits are calculated when you partially exit positions:

- **FIFO (First In, First Out)**: Default method, oldest shares sold first
- **LIFO (Last In, First Out)**: Newest shares sold first
- **Weighted Average**: Uses average cost basis across all shares

**Impact**: Changes which purchase price is matched with your sale price, affecting profit amounts. Important for tax reporting.

### Default Commissions

Configure automatic commission deduction from your trades:

**Commission Type**:
- Fixed per trade (e.g., $5 per trade)
- Per share (e.g., $0.01 per share)
- Per contract (e.g., $0.65 per contract for options)
- Percentage-based (e.g., 0.1% of trade value)

**When Applied**:
- Entry only
- Exit only
- Both entry and exit

These commissions automatically deduce from your profit calculations, showing true net profit.

### Breakeven Range

The breakeven range helps identify when trades are near their break-even point:

**Setting Breakeven Sensitivity**:
- Enter a dollar amount (e.g., $50)
- Or enter a percentage (e.g., 2%)
- Trades within this range of breakeven are highlighted

**Use Cases**:
- Identify near-breakeven trades for easier management
- Set risk parameters
- Filter trades for analysis
- Track trades close to profitability

Trades are marked as "breakeven" when profit/loss falls within your specified range.

### Trade Tracking Options

**Automatic Trade Sync**:
- Enable automatic import from your broker
- Choose sync frequency (real-time, hourly, daily)
- Broker: Select your connected broker
- Sync status: Shows if connection is active

**Manual Trade Entry**:
- Choose default entry fields
- Set up templates for recurring trade types
- Configure keyboard shortcuts

### Asset Class Specific Settings

Depending on your account's asset class:

**Stocks**:
- Dividend tracking
- Stock split adjustments
- Long-term capital gains designation

**Options**:
- Expiration tracking
- Option-specific commission rates
- Assignment vs. exercise handling

**Futures**:
- Contract specifications
- Rollover handling
- Point value tracking

**Forex**:
- Pip value calculations
- Leverage tracking
- Currency conversion settings

## Performance Calculation Settings

### P&L Calculation Method

Choose how P&L is displayed:

- **Trade-by-Trade**: Each trade shows individual profit/loss
- **Position-Based**: Cumulative P&L for each position
- **Daily Summary**: Aggregate daily performance

### Return Metrics

Configure how your returns are calculated:

**Return on Investment (ROI)**:
- Calculated as: (Net Profit / Account Balance) × 100%
- Uses net profit after commissions
- Important for comparing performance

**Win Rate**:
- Percentage of profitable trades
- Affected by calculation method chosen

## Saving Your Changes

After modifying any Trade Settings:

1. Review all changes in the settings panel
2. Click **"Save Changes"** or **"Update Settings"** button
3. A confirmation message will appear
4. Changes apply immediately to new trades
5. Some changes may recalculate historical trades

## Common Trade Settings Combinations

**Conservative Trader**:
- FIFO method (standard approach)
- Fixed commission per trade
- Wide breakeven range (±$100 or more)

**Day Trader**:
- FIFO method (for consistency)
- Per-share commission (high volume)
- Narrow breakeven range (±$25)

**Options Trader**:
- FIFO or Weighted Average
- Per-contract commissions ($0.65 typical)
- Expiration tracking enabled

**Futures Trader**:
- FIFO method
- Per-contract commissions
- Contract-specific settings enabled

## Resetting Settings to Defaults

To reset Trade Settings to TradeZella defaults:

1. Go to Trade Settings
2. Click **"Reset to Defaults"** (if available)
3. Confirm the reset action
4. All settings return to TradeZella defaults
5. You can then customize as needed

## Important Notes

- Settings are per-account, not global
- Each account maintains independent settings
- Changes affect future profit calculations
- Historical trades may be recalculated when changing methods
- Always review settings changes before confirming

---

## See also
- [Profit Calculation Methods](profit-calculation-methods.md)
- [How to Set Default Commissions and Fees](default-commissions.md)
- [Creating an Account in TradeZella](creating-account.md)
- [Setting Your Account Balance in TradeZella](account-balance.md)
