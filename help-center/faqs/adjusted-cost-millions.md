---
title: Why Is My Adjusted Cost Showing Up in Millions? It Seems Incorrect
description: Explains why adjusted cost may appear in millions (usually forex lot size calculation) and how to fix it
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/8431316-why-is-my-adjusted-cost-showing-up-in-millions-it-seems-incorrect
  md: https://www.tradezella.com/help-center/faqs/adjusted-cost-millions.md
---

# Why Is My Adjusted Cost Showing Up in Millions? It Seems Incorrect

If you're seeing an "Adjusted Cost" figure in the millions when you only invested hundreds or thousands, this is usually a calculation error caused by forex lot size misinterpretation or incorrect position quantity entry during import. The most common culprit is that your position size was imported as "1 lot" but the system calculated it as though you traded 1,000 units (or similar) without properly converting the lot size to actual units. This guide explains how adjusted cost is calculated, why the error occurs, and how to fix it.

TradeZella's adjusted cost feature is designed to account for scale-ins (adding to positions over multiple entries) and calculate your true average cost basis across all fills in a trade. When the calculation goes wrong, it's almost always due to an import data issue rather than a platform error. The good news is that identifying and correcting the problem is straightforward once you understand what happened.

## Understanding Adjusted Cost

### What Is Adjusted Cost?

Adjusted Cost is the total capital you've deployed across all entries into a position, accounting for scale-ins where you've added to a position over multiple trades. It represents your true cost basis for the entire position.

**Formula:**
Adjusted Cost = (Entry Price 1 × Quantity 1) + (Entry Price 2 × Quantity 2) + ... (Entry Price N × Quantity N)

### Example: Single Entry
- Entry 1: 100 shares at $50
- Adjusted Cost: $50 × 100 = $5,000

### Example: Scaled Entry (Multiple Fills)
- Entry 1: 100 shares at $50
- Entry 2: 50 shares at $52 (scaling in)
- Entry 3: 25 shares at $51
- Adjusted Cost: ($50 × 100) + ($52 × 50) + ($51 × 25) = $5,000 + $2,600 + $1,275 = **$8,875**

## Why Adjusted Cost Shows Millions: Common Causes

### Cause 1: Forex Lot Size Error (Most Common)

**The Problem:**
Forex lot sizes are confusing because "1 lot" = 100,000 units of the base currency. When you import a forex trade, the system must properly convert lot notation to actual units.

**Example Error:**
- You traded 0.1 lot of EUR/USD
- 0.1 lot = 10,000 EUR (0.1 × 100,000)
- Entry price: 1.1000
- **Incorrect calculation:** 0.1 × 1.1000 = 0.11 (treating it as units)
- **Correct calculation:** 10,000 × 1.1000 = $11,000

If TradeZella imports "0.1" but treats it as though you traded "100,000," it calculates:
- 100,000 × 1.1000 = $110,000 (massive adjusted cost!)

### Cause 2: Position Size Not Converted Properly

**The Problem:**
Your broker import included position size in one format, but TradeZella interpreted it differently.

**Example:**
- Broker file shows: "Quantity: 1, Lot: 0.5" (meaning 0.5 lot = 50,000 units)
- TradeZella imports "Quantity: 1" and misses the "Lot: 0.5"
- System treats it as 1 unit × 1,000,000 (default forex lot conversion)
- Calculation explodes to millions

### Cause 3: Decimal Place Misinterpretation

**The Problem:**
Comma vs. period decimal usage, or scientific notation being misread.

**Example:**
- European system shows: "1,500" (meaning 1.500 or 1500 units)
- Imported as: "1500" which gets converted to 1,500,000

### Cause 4: Multiple Fill Import Error

If importing scale-in trades where quantity information is duplicated:
- Entry 1: 0.5 lot
- Entry 2: 0.3 lot
- But system reads both as "1" instead of separate quantities
- Adjusted cost multiplies incorrectly

## How to Identify the Problem

### Step 1: Check Trade Details
1. Navigate to the trade with incorrect adjusted cost
2. Click to open trade details
3. Look at: Entry Price, Quantity, and Adjusted Cost
4. Note if these numbers seem to match the issue described above

### Step 2: Compare to Broker Statement
1. Pull up your original broker statement
2. Find the matching trade
3. Compare:
   - Entry price (should match)
   - Quantity (should match in same units)
   - Position size/lot notation
4. Identify the discrepancy

### Step 3: Verify Entry Price
- If adjusted cost is millions but entry price looks normal, quantity is the culprit
- If both entry price and quantity look wrong, data corruption occurred during import

**Example Analysis:**
- TradeZella shows: Entry Price: 1.1050, Quantity: 100,000
- Broker shows: Entry Price: 1.1050, Quantity: 0.1 lot
- **Issue identified:** Quantity imported as units (100,000) instead of lots (0.1)

## How to Fix Adjusted Cost Errors

### Fix Method 1: Edit the Trade

**For Forex Trades (Lot Size Error):**
1. Open the trade in edit mode
2. Locate the **Quantity** field
3. Convert from units back to lot notation:
   - 100,000 units = 1.0 lot
   - 10,000 units = 0.1 lot
   - 50,000 units = 0.5 lot
4. Change quantity to correct lot size (e.g., "0.1" instead of "100,000")
5. Save the trade
6. TradeZella recalculates adjusted cost correctly

**Example Fix:**
- Original (incorrect): Quantity: 100,000, Entry Price: 1.1050
- Corrected: Quantity: 0.1, Entry Price: 1.1050
- Adjusted Cost now calculates as: 0.1 × 1.1050 = 0.1105 (still seems low; may need different unit system)

**Better Approach:** Keep quantity in units but correct the scale
- Original (incorrect): Quantity: 100,000, Entry Price: 1.1050 = Adjusted Cost: $110,050
- Note: This is actually correct if you truly traded 100,000 units = 1 lot
- **The real fix:** Enter entry price correctly for your position size system

### Fix Method 2: Batch Edit

If multiple forex trades have the same error:
1. Filter trades by symbol or strategy where error exists
2. Select all affected trades using checkboxes
3. Click **Batch Edit**
4. Select **Quantity** field
5. Apply correction formula (e.g., divide all by 1,000,000)
6. Confirm batch operation

**Caution:** Use batch edit only if you're certain all trades have the same error pattern.

### Fix Method 3: Delete and Re-import

If adjustments seem risky or numerous:
1. Delete the problematic trades
2. Re-import from broker with corrected data
3. Verify adjusted cost calculation on re-import
4. Adjust column mapping if needed during import

## Understanding Forex-Specific Adjusted Cost

### Standard Forex Quote Convention
- Prices typically quoted to 4 decimal places (e.g., EUR/USD 1.1050)
- Lot sizes: 1 lot = 100,000 base currency units
- Micro lot: 0.01 lot = 1,000 units
- Mini lot: 0.1 lot = 10,000 units

### Adjusted Cost Calculation for Forex
**Formula:** Adjusted Cost = Lot Size × 100,000 × Entry Price

**Example:**
- 0.5 lot EUR/USD at 1.1050
- Adjusted Cost = 0.5 × 100,000 × 1.1050 = **$55,250**

This is correct for a 0.5 lot position. If you see $55,250,000, the quantity was entered as 50 instead of 0.5.

## Preventing Adjusted Cost Errors in Future Imports

### Best Practices for Forex Imports

**Use Standard Lot Notation:** When importing forex trades, always use lot notation (0.1, 0.5, 1.0) rather than unit notation (10,000, 50,000, 100,000).

**Verify Column Mapping:** During import, carefully review the column mapping:
- Confirm quantity column is identified correctly
- Check if lot size needs conversion
- Verify entry price is in correct decimal format

**Test With Small Batch:** Import 5-10 trades first, verify adjusted costs match broker statement, then import full history.

**Pre-Import Verification:** If importing from CSV, open the file and visually verify quantities and prices look reasonable before uploading.

### Broker-Specific Import Tips

**MetaTrader (MT4/MT5):**
- Usually imports correctly
- Verify account currency matches your accounting currency
- Check if commission/spread included in P&L calculation

**Interactive Brokers:**
- Downloads may use different decimal separators
- Verify no row duplication during import
- Check that quantity includes scale-in fills properly

**OANDA, IG, Other Forex Brokers:**
- Export in standard format before importing
- Verify lot size vs. units notation
- Some brokers use different conventions; test first

## Checking Adjusted Cost Across Multiple Trades

### Dashboard View
1. Go to **Analytics > Performance Summary**
2. Look at **Total Adjusted Cost** across filtered trades
3. If suspiciously high, investigate top 5 positions contributing most
4. Check if 1-2 errors are distorting the total

### Filtering to Find Problem Trades
1. Use **Filter > Adjusted Cost** (if available)
2. Sort by adjusted cost (highest first)
3. Review top adjustments costs
4. Check if these match your actual position sizes
5. Flag any outliers for editing

### Batch Review
1. Export trade journal to CSV
2. Calculate: Adjusted Cost / Entry Price = Expected Quantity
3. Compare calculated quantity to actual quantity in TradeZella
4. Large discrepancies indicate import errors

## When to Contact Support

**Contact TradeZella support if:**
- You've identified the error but can't fix it
- Multiple trades have the same systemic error
- Import from your specific broker consistently shows adjusted cost errors
- You suspect data corruption beyond simple lot size conversion

**Information to provide support:**
- Broker statement screenshots showing correct position size
- TradeZella screenshot showing incorrect adjusted cost
- Details of what you tried to fix it
- Information about broker and import method used

---

## See also
- [How to Edit Trades in TradeZella](/help-center/faqs/how-to-edit-trades.md)
- [How to Undo Imports in TradeZella](/help-center/faqs/how-to-undo-imports.md)
- [What Trading Assets Are Supported?](/help-center/faqs/supported-trading-assets.md)
