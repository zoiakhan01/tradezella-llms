---
title: How to Set Default Commissions and Fees
description: Configure auto-applied commissions per trade for accurate P&L calculations in TradeZella
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/6954370-how-to-set-default-commissions-and-fees-for-your-trades
  md: https://www.tradezella.com/help-center/account-management/default-commissions.md
---

# How to Set Default Commissions and Fees

Setting default commissions and fees in TradeZella ensures accurate profit and loss calculations. When you apply commissions to trades, they reduce your net profit, giving you a true picture of your trading performance.

## Why Commissions Matter

Commissions and fees directly impact your P&L:

- **Without Commissions**: A $1,000 profit trade appears as $1,000 gain
- **With Commissions**: If you paid $20 in commissions, your actual profit is $980
- **Cumulative Effect**: Commissions add up quickly, especially for active traders
- **Accurate Tracking**: Including commissions shows your true trading results

## Types of Fees You Can Track

TradeZella allows you to record:

- **Entry Commissions**: Fees paid when opening a position
- **Exit Commissions**: Fees paid when closing a position
- **Trading Fees**: Per-trade fees from your broker
- **Regulatory Fees**: SEC fees or exchange fees
- **Option Fees**: Special fees for options trading
- **Spread Costs**: Bid-ask spread costs (if tracking)
- **Other Costs**: Any other trading-related expenses

## Setting Default Commissions

### Step 1: Access Commission Settings

1. Go to your account's **"Trade Settings"**
2. Look for the **"Commissions"** or **"Default Commissions"** section
3. Click **"Edit Commissions"** or **"Configure Defaults"**

### Step 2: Configure Commission Types

Select how you want to input commissions:

**Per Trade Commission**: A fixed amount per trade
- Enter a dollar amount (e.g., $5.00 per trade)
- Applied automatically to every entry and exit

**Per Share Commission**: Calculate based on shares traded
- Enter cost per share (e.g., $0.01 per share)
- Multiply by shares in each trade
- Better for large share quantities

**Per Contract Commission**: For options and futures
- Cost per contract (e.g., $0.65 per contract)
- Applied based on contracts traded

**Percentage-Based Commission**: As a percentage of trade value
- Enter percentage (e.g., 0.1%)
- Calculated as a percentage of total trade value

### Step 3: Enter Your Rates

1. Select your commission type from the dropdown
2. Enter the amount or percentage
3. Specify if it applies to:
   - Entries only
   - Exits only
   - Both entries and exits
4. Save your settings

## Applying Commissions to Trades

### Automatic Application

Once default commissions are set:

- They apply automatically to all new trades you enter
- Manual trades receive the default commission upon entry
- Imported trades may include imported commission data

### Manual Override

For individual trades, you can:

1. Open the trade details
2. Edit the commission field
3. Enter a different amount for just that trade
4. Save the trade

## Different Commissions Per Asset Class

If your commissions vary by asset type:

1. Set defaults for each asset class separately
2. Different accounts can have different default commissions
3. Per-trade overrides allow flexibility for varying commissions

## Broker-Specific Commissions

Popular broker commission structures:

**Charles Schwab / Thinkorswim**:
- $0 stock commissions
- $0.65 per options contract
- Small regulatory fees for stocks

**Interactive Brokers**:
- Tiered pricing based on volume
- Typical: $0.005 per share minimum $1
- Options: $0.65 per contract

**Tradovate**:
- ~$2.50 per micro futures contract
- Variable based on contract type

**Questrade**:
- $4.95 per stock trade
- $0.95 per options contract

Check your broker's fee schedule and enter accordingly.

## Reviewing Commission Impact

To see how commissions affect your P&L:

1. View your trade journal or performance report
2. Look at the "Commission" column
3. Compare gross profit vs. net profit (profit minus commissions)
4. Review total commissions paid for the period

## Modifying Commissions Later

To change your default commissions:

1. Return to **Trade Settings** > **Commissions**
2. Update the rates or percentage
3. New trades will use updated rates
4. Existing trades retain their original commissions
5. You can edit individual trade commissions if needed

## Commission vs. Profit Tracking

TradeZella tracks:

- **Gross Profit**: Profit before commissions
- **Net Profit**: Profit after commissions
- **Commission Total**: Total fees paid in the period
- **ROI**: Return on Investment calculated with net profit

Always review net profit to see your true trading results.

---

## See also
- [Trade Settings Tab Explained](trade-settings.md)
- [Profit Calculation Methods](profit-calculation-methods.md)
- [Creating an Account in TradeZella](creating-account.md)
