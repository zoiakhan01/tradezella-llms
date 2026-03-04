---
title: How to Edit Trades in TradeZella
description: Steps to edit trade details including entry/exit prices, dates, notes, and tags
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/10254436-how-to-edit-trades-in-tradezella
  md: https://www.tradezella.com/help-center/faqs/how-to-edit-trades.md
---

# How to Edit Trades in TradeZella

TradeZella allows you to edit trade details after they've been imported or created. Whether you need to correct a price that was entered incorrectly, update the entry or exit date, add notes about what you were thinking during the trade, or assign tags for strategy organization, the edit functionality gives you full control over your trading data. Edited trades immediately recalculate all associated metrics, ensuring your performance analytics reflect accurate information.

Making corrections to trades is important for maintaining trading integrity. An incorrect entry price of $100 vs. the actual $101 might seem minor, but across 100 trades, these small errors compound into inaccurate performance metrics. TradeZella's edit feature is designed to be simple and intuitive, allowing single-trade edits or batch editing of multiple trades with similar corrections needed.

## Editing Individual Trades

### Opening Trade Editor
1. Navigate to your **Trade Journal** or **Trades** tab
2. Locate the trade you want to edit
3. Click the three-dot menu icon (⋯) on the trade row
4. Select **"Edit Trade"**
5. The trade editor window opens showing all editable fields

### Fields You Can Edit

**Entry Price:** Modify the entry price per share, contract, or pip
- Click the field and enter the corrected price
- Useful for correcting OCR errors from statement imports or typos

**Exit Price:** Change the price at which you exited the position
- Updates your profit/loss calculation immediately
- Can be left blank for open (unrealized) positions

**Entry Date & Time:** Adjust the date and time you entered the trade
- Affects trade sequencing and can impact strategy analysis if timing matters
- Select from calendar picker or type the date

**Exit Date & Time:** Modify when you closed the position
- Important for holding period calculations and tax reporting

**Quantity:** Change the number of shares or contracts traded
- Useful if position size was imported incorrectly
- Recalculates P&L based on new quantity

**Symbol/Instrument:** Change the trading symbol if it was imported wrong
- Select from dropdown or search for correct symbol
- Updates asset class categorization automatically

**Account:** Assign trade to correct broker account if imported to wrong one
- Dropdown shows all connected accounts
- Helps organize trades across multiple brokers

**Commission & Fees:** Add or adjust commission amounts
- Important for accurate P&L calculation
- Can specify per-share commission or flat fee

**Type:** Modify trade type if needed
- Options: Long, Short, Call, Put, Covered Call, etc.
- Ensures proper classification for analytics

**Notes:** Add or update trade notes
- Document what you were thinking, setup confirmation, news events, etc.
- Useful for reviewing trades later to identify patterns

**Tags:** Add or remove custom tags
- Examples: "breakout," "pullback," "scalp," "swing," "high-volatility"
- Use consistent tagging for reliable filtering and analysis

**Strategy:** Assign or change the strategy classification
- Helps you analyze performance by trading approach
- Essential for evaluating individual strategies

## Editing Multiple Trades (Batch Edit)

### Batch Edit Process
1. In your **Trade Journal**, use **Filters** to narrow to trades needing the same edit
   - Example: All trades from a specific date or symbol that need commission adjustments
2. Select multiple trades using the checkboxes on the left
3. Click **"Batch Edit"** button that appears
4. Select which field(s) you want to change
5. Enter the new value or adjustment
6. Choose to **Replace** the current value or **Add** to existing value
7. Click **"Apply to Selected Trades"**
8. Confirm the batch operation

### Batch Edit Examples
- **Add commission to all trades from March:** Filter by date, select all, batch edit to add $5 commission to each
- **Tag all losing trades:** Filter to losing trades, batch add tag "loss review needed"
- **Correct symbol across multiple imports:** Filter by incorrect symbol, batch change to correct symbol
- **Update strategy classification:** Filter by date range, batch assign all to correct strategy name

## Real-Time Metrics Updates

After editing a trade, TradeZella automatically recalculates:
- **Profit/Loss:** Updated based on new prices or quantity
- **Win Rate:** If you changed a trade from winning to losing or vice versa
- **Average Win/Loss:** Recalculated across all trades in filters
- **Trade Expectancy:** Updated if metrics change materially
- **R-Multiple:** Adjusted if entry/exit prices or risk amount changed
- **All Charts and Reports:** Dashboard visualizations update immediately

This real-time recalculation ensures your analytics always reflect your actual trading data.

## Trade Edit History & Undo

### Viewing Edit History
1. Open a trade in edit mode
2. Look for **"Edit History"** or **"View Changes"** link
3. See a log of all modifications made to this trade
4. View who made changes and when (important for team accounts)

### Undoing an Edit
- If you made an incorrect edit, click **"Undo Last Change"** while the trade is open
- Or close without saving to discard unsaved changes
- Saved changes are permanent but can be re-edited anytime

## Best Practices for Editing Trades

**Correct Immediately:** Fix import errors as soon as you notice them, rather than letting incorrect data accumulate.

**Use Tags Consistently:** Develop a standard tagging system (e.g., "breakout," "pullback," "support-bounce") and apply consistently for reliable filtering.

**Document Context:** In notes, write what you saw in the market when you took the trade. This helps you review and identify patterns in your decision-making.

**Verify Large Corrections:** If adjusting prices significantly, verify against your broker statement or trading platform to ensure accuracy.

**Batch Edit When Possible:** For systematic corrections (like adding commission to a batch of trades), use batch edit rather than editing individually.

**Maintain Audit Trail:** Keep notes of major corrections for your own records, especially important for tax purposes.

## Common Edit Scenarios

**Import Decimal Error:** Symbol was imported as "100.5" when it should be "100.50" → Edit to correct price

**Wrong Symbol:** Imported ES trade as "SPY" by mistake → Edit symbol field to "ES"

**Missing Commission:** Broker charged $10 per trade but wasn't included → Edit commission field to add

**Incorrect Date:** System imported trade date one day off → Edit entry and exit dates

**Missing Strategy Tag:** Imported old trades before you started tagging → Use batch edit to add strategy tag

---

## See also
- [How to Filter Your Trades in TradeZella](/help-center/faqs/how-to-filter-trades.md)
- [How to Undo Imports in TradeZella](/help-center/faqs/how-to-undo-imports.md)
- [What Is Trade Expectancy, and How Does It Help?](/help-center/faqs/trade-expectancy.md)
