---
title: Tradovate P&L Issues
description: Troubleshoot and resolve profit and loss calculation issues with Tradovate accounts
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/8423105-tradovate-p-l-issues
  md: https://www.tradezella.com/help-center/troubleshooting/tradovate-pnl-issues.md
---

# Tradovate P&L Issues

If your Tradovate futures trades are showing incorrect profit and loss calculations in TradeZella, this guide will help you identify and resolve P&L discrepancies.

## Understanding Tradovate P&L

### How Tradovate Reports P&L

Tradovate calculates P&L as:

- **Gross Profit**: Exit price - Entry price (per contract)
- **Multiplied by**: Contract size (multiplier)
- **Futures**: Typically $1 to $50 per point depending on contract
- **Micro Contracts**: Smaller multiplier than standard contracts
- **Commissions**: Deducted from gross profit
- **Fees**: Also deducted (regulatory, exchange fees)

### How TradeZella Calculates P&L

TradeZella needs:

- **Entry Price**: Exact fill price at entry
- **Exit Price**: Exact fill price at exit
- **Contract Size**: Correct contract multiplier
- **Commissions**: All trading fees
- **Micro vs. Standard**: Correct contract type
- **Quantity**: Number of contracts

Mismatch in any field causes P&L discrepancy.

## Common Causes of P&L Issues

### Wrong Contract Multiplier

Most common issue:

- **Standard Contracts**: E.g., ES (S&P 500) = $50 per point
- **Micro Contracts**: E.g., MES (Micro S&P 500) = $5 per point
- **Nano Contracts**: E.g., NQ might be even smaller
- **TradeZella Misconfigured**: System using wrong multiplier
- **Import Data Wrong**: Tradovate data imported with wrong values

### Entry/Exit Price Discrepancies

Prices not matching Tradovate:

- **Slippage**: Actual fill worse than displayed
- **Multiple Fills**: Large orders filled at multiple prices
- **Rounding**: Different rounding between systems
- **Quote vs. Trade**: Using quote price instead of actual fill
- **After-Hours**: Trading outside standard hours at different price

### Commissions Not Applied

Tradovate charges commissions:

- **Per Round-Turn**: Charge per open and close
- **Per Contract**: Varies by contract ($1-$5 typical)
- **Micro Contracts**: Usually lower commissions
- **TradeZella Default**: May not have Tradovate rates set
- **Not Imported**: Commission data not included in import

### Partial Fills on Large Orders

Orders may fill in multiple parts:

- **Quantity Mismatch**: TradeZella shows different quantity than filled
- **Multiple Entries**: Large order split into multiple fills
- **Multiple Exits**: Closed in stages, not all recorded
- **Split Position**: Closed part and rolled part separately
- **System Combines**: Some systems auto-combine, some don't

### Overnight Funding Charges

Tradovate charges for holding positions:

- **Overnight Hold**: Charge for keeping position overnight
- **Funding Rate**: Variable based on utilization
- **Not Trade P&L**: Separate from trade profit/loss
- **Deducted from Account**: Shows as account fee, not trade P&L
- **May Not Import**: These fees often separate from trade data

## Troubleshooting Steps

### Step 1: Verify Tradovate Account Data

1. Log into Tradovate directly
2. Go to **Trade History** or **Account Statement**
3. Find the specific trade
4. Note exact entry price
5. Note exact exit price
6. Note commission charged
7. Note contract type (standard vs. micro)
8. Compare all with TradeZella

### Step 2: Check Contract Specifications

1. In TradeZella, view the trade
2. Check the contract symbol
3. Verify contract type:
   - Is it standard or micro?
   - ES vs. MES (different multipliers)
   - NQ vs. MNQ
   - YM vs. MYM
4. If micro, make sure TradeZella knows it's micro

### Step 3: Verify Multiplier Settings

1. Go to your Tradovate account settings in TradeZella
2. Look for **"Contract Specifications"** or **"Multipliers"**
3. Verify each contract has correct multiplier:
   - ES (S&P 500): $50/point
   - MES (Micro): $5/point
   - NQ (Nasdaq): $20/point
   - MNQ (Micro): $2/point
   - YM (Dow): $5/point
   - MYM (Micro): $0.50/point
4. Update if incorrect
5. Past trades recalculate with correct multiplier

### Step 4: Check Commission Settings

1. In **Account Settings** > **Trade Settings**
2. Find **"Commissions"** or **"Default Fees"**
3. Verify Tradovate commission structure
4. Standard Tradovate: Usually $2-$2.50 per round-turn
5. Micro contracts: May be $1-$1.50 per round-turn
6. Update if different
7. Set as default commission

### Step 5: Review Import Data

If importing from Tradovate:

1. Check what data was imported
2. Go to **Import History**
3. Find the Tradovate import
4. Click **"View Details"**
5. Verify:
   - All trades imported
   - Prices match Tradovate
   - Quantities correct
   - Commissions included
6. If data incomplete, manual correction needed

## Specific Resolution Steps

### Fixing Contract Multiplier Issue

Example: MES trades showing 10x profit (using ES multiplier instead of MES)

1. Find **Contract Settings** in Account Settings
2. Locate MES contract
3. Change multiplier from $50 to $5
4. Save changes
5. All MES trades recalculate
6. P&L should now be correct (10th of previous amount)
7. Verify one trade matches Tradovate

### Fixing Missing Commissions

Example: Gross profit shows $500 but Tradovate shows $497 (after commission)

1. Go to **Trade Settings**
2. Set commission to correct amount
3. Choose commission type:
   - Fixed per round-turn (e.g., $3)
   - Or per contract and side
4. Apply to account
5. Past trades recalculate with commissions
6. Net profit should now match Tradovate

### Fixing Partial Fill Issues

Example: Entered 2 contracts at different prices, but TradeZella shows 1 contract

1. Check if trades imported as separate or combined
2. If incorrectly combined:
   - Delete the combined trade
   - Manually re-enter both fills separately
   - Or use average price for both
3. Ensure quantity matches total Tradovate quantity
4. Check exit matches all contracts exited

### Fixing Price Discrepancies

Example: TradeZella shows entry at 4000.50, Tradovate shows 4000.75

1. Open the trade in TradeZella
2. Edit the entry price
3. Enter correct price from Tradovate
4. Save changes
5. P&L updates immediately
6. Verify profit matches Tradovate

## Tradovate-Specific Considerations

### Micro Contracts

When trading micros:

- Ensure contract symbol includes "M" or is identified as micro
- Micro multipliers are 1/10th of standard
- MES = $5/point (ES = $50/point)
- MNQ = $2/point (NQ = $20/point)
- Commissions typically lower for micros

### Contract Rollovers

If rolling contracts (e.g., ES Z23 to ESH24):

- Old contract: Record exit
- New contract: Record entry
- May show as two separate trades (correct)
- Or may need manual entry if not synced
- Don't delete as duplicates

### Spread Trades

If trading spreads (e.g., calendar spreads):

- Buy/sell both legs recorded as separate trades
- Or recorded as single spread trade
- Check if both legs imported
- Verify P&L reflects both legs
- May need manual entry if not synced

### Using Leverage

Tradovate allows leverage on accounts:

- Doesn't affect individual trade P&L
- Affects margin available
- Commissions may vary with leverage
- TradeZella calculates per trade, not leveraged
- Account stats should match regardless

## Sync Issues vs. Calculation Issues

### Sync Issues (Data Not Importing)

- Trades not appearing in TradeZella
- Delay in trades showing up
- Connection problems with Tradovate
- Solution: Check Tradovate connection

### Calculation Issues (Trades Show Wrong P&L)

- Trades appear but with wrong profit
- Prices are different
- P&L doesn't match Tradovate
- Solution: Verify and correct settings as above

## Manual Entry Alternative

If sync is consistently problematic:

1. Export trades from Tradovate
2. Manually enter into TradeZella
3. Use exact entry/exit prices from Tradovate
4. Apply correct commissions
5. Verify P&L matches
6. Gives you full control and accuracy

## Performance Verification

After fixing P&L issues:

1. **Review Account P&L**: Should match Tradovate total
2. **Win Rate**: Verify correct number of wins/losses
3. **Largest Win/Loss**: Check individual trade largest values
4. **Total Commissions**: Verify total matches
5. **ROI**: Recalculate based on correct account balance

## When to Contact Support

Contact TradeZella Support if:

1. Multiplier corrections don't resolve issue
2. Commission settings don't match reality
3. Prices still mismatched after verification
4. Sync is not working
5. Specific contract types not recognized
6. System shows persistent calculation errors

Provide Support with:
- Tradovate account username
- Specific trade details (symbol, date, prices)
- What contract multiplier should be
- Screenshots showing discrepancy
- Steps already taken

## Contact Tradovate Support

If the issue is with Tradovate data:

- Contact Tradovate directly
- Verify Tradovate account shows correct P&L
- Check if there are API/export issues
- Confirm contract specifications
- Tradovate Support: support@tradovate.com

---

## See also
- [Why Are My Thinkorswim Trades Not Syncing?](thinkorswim-not-syncing.md)
- [Why Are My Interactive Brokers Trades Not Syncing?](interactive-brokers-not-syncing.md)
- [Resolving TOS/Charles Schwab Account Sync Failure Issues](schwab-sync-issues.md)
