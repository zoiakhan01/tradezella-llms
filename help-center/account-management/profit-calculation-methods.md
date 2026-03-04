---
title: Profit Calculation Methods - FIFO, LIFO, Weighted Average
description: Three profit calculation methods available in TradeZella and when to use each method
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/6826141-different-profit-calculation-methods-in-tradezella-fifo-lifo-weighted-average
  md: https://www.tradezella.com/help-center/account-management/profit-calculation-methods.md
---

# Profit Calculation Methods - FIFO, LIFO, Weighted Average

TradeZella supports three different profit calculation methods for determining how trades are matched and profit is calculated. The method you choose affects your reported P&L and can have tax implications. Understanding each method helps you select the best approach for your trading style.

## Overview of Calculation Methods

TradeZella uses the method you select to determine:

- Which specific shares/contracts are being closed when you partially exit a position
- Cost basis for each trade exit
- Profit and loss amounts
- Long-term vs. short-term gains (for US tax purposes)
- Overall account performance metrics

## FIFO (First In, First Out)

FIFO is the default and most commonly used method. With FIFO:

- The oldest shares/contracts purchased are assumed to be sold first
- When you buy 100 shares at $10, then 100 shares at $15, and sell 100 shares, the first 100 at $10 are assumed sold
- Profit = Sale price - original cost of oldest purchase
- Ideal for buy-and-hold traders and retirement accounts
- Simplest method for record-keeping

**When to Use FIFO**:
- Default choice for most traders
- Required for certain retirement accounts
- When you want straightforward, chronological accounting
- If you're unsure which method to use

## LIFO (Last In, First Out)

With LIFO, the most recent shares/contracts purchased are sold first:

- When you buy 100 shares at $10, then 100 shares at $15, and sell 100 shares, the 100 shares at $15 are assumed sold first
- Profit = Sale price - cost of most recent purchase
- Can result in higher taxable gains if prices have risen
- May benefit traders with specific tax strategies
- More complex accounting

**When to Use LIFO**:
- For tax loss harvesting strategies
- Traders making frequent entries and exits
- When you need specific cost basis matching
- Complex trading strategies with multiple buy levels
- Not allowed for certain asset types (check IRS rules)

## Weighted Average

The weighted average method calculates cost basis across all shares:

- Cost basis = Total cost of all shares / Total shares held
- All shares are treated as having the same cost basis
- Profit = Sale price - average cost per share
- Smooths out profit calculations across multiple entries
- Moderate complexity

**When to Use Weighted Average**:
- Dollar-cost averaging strategies
- Consistent position building over time
- When you want averaged profit calculations
- Simplicity between FIFO and LIFO
- Some brokers require or prefer this method

## Comparison Example

Scenario: Buy 100 shares at $10, buy 100 shares at $15, sell 100 shares at $20

| Method | Shares Sold | Cost Basis | Profit |
|--------|------------|-----------|--------|
| FIFO | First 100 @ $10 | $1,000 | $1,000 |
| LIFO | Most recent 100 @ $15 | $1,500 | $500 |
| Weighted Average | 100 @ $12.50 avg | $1,250 | $750 |

## Setting Your Calculation Method

### During Account Creation

1. When creating a new TradeZella Account
2. Select your preferred profit calculation method from the dropdown
3. FIFO is pre-selected as default
4. You can change this after creation

### In Account Settings

1. Navigate to your account's **"Trade Settings"** or **"Account Settings"**
2. Find the **"Profit Calculation Method"** dropdown
3. Select your desired method (FIFO, LIFO, or Weighted Average)
4. Click **"Save Changes"**
5. The method applies to all future profit calculations

## Important Considerations

- **Tax Implications**: Different methods may result in different tax consequences. Consult a tax professional.
- **Broker Requirements**: Some brokers specify which methods are acceptable
- **Consistency**: Choose a method and stick with it for the calendar year
- **IRS Compliance**: For US traders, document your choice for tax reporting
- **Past Trades**: Changing methods may recalculate P&L on historical trades

## Changing Your Method

You can change your profit calculation method in Account Settings. However:

- The change applies to future trades
- Historical trades may be recalculated based on the new method
- Performance reports will reflect the new calculation
- Always consult a tax professional before changing methods

---

## See also
- [Trade Settings Tab Explained](trade-settings.md)
- [Creating an Account in TradeZella](creating-account.md)
- [How to Set Default Commissions and Fees](default-commissions.md)
