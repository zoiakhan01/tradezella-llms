---
title: Understanding Different Order Types in TradeZella Backtesting
description: Market, limit, stop orders and other order types available in backtesting
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/9981393-understanding-different-order-types-in-tradezella-backtesting
  md: https://www.tradezella.com/help-center/backtesting-replay/order-types-backtesting.md
---

# Understanding Different Order Types in TradeZella Backtesting

TradeZella backtesting supports all major order types, allowing you to test realistic trade execution. Understanding order types is essential for developing realistic and profitable strategies.

## Market Orders

### What is a Market Order?

A market order executes immediately at the current best available price:
- **Execution**: Instant
- **Price**: Current market price
- **Slippage**: Applies realistically
- **Use case**: Immediate entry/exit when timing is critical

### How Market Orders Work in Backtesting

1. **Click to place order**: Click on chart or use keyboard shortcut (B for buy, S for sell)
2. **Order executes immediately**: At market price on current candle
3. **Slippage applied**: Based on market volatility and volume
4. **Position opens**: Immediately enters the market
5. **Spreads included**: Account for bid/ask spread

### Example Market Order

**Scenario**: ES at 4500 (bid/ask 4500.00/4500.25)
1. Click "Buy Market"
2. Executes at 4500.25 (ask price)
3. Position opens at 4500.25
4. Slippage: +0.25 cost of entry

### When to Use Market Orders

- **Fast entries**: Need immediate execution on breakouts
- **Urgent exits**: Escape losing trades quickly
- **Volatile markets**: When price moves fast
- **Support/resistance breaks**: Don't want to miss entry

## Limit Orders

### What is a Limit Order?

A limit order only executes at your specified price (or better):
- **Price**: Exact price you specify
- **Execution**: Only if market reaches your price
- **Fill guarantee**: May not fill if price doesn't reach limit
- **Use case**: Precise entry points, protecting against slippage

### How Limit Orders Work in Backtesting

1. **Specify target price**: Entry price you want
2. **Place limit order**: (L for limit buy, K for limit sell)
3. **Order waits**: Remains open until price is hit
4. **Automatic fill**: Fills when market reaches your price
5. **No slippage**: Executes at your specified price (or better)

### Limit Buy Order Example

**Setup**: Want to buy ES at 4500 exactly
1. Click on price level 4500
2. Select "Place Limit Buy"
3. Quantity: 1 contract
4. Order placed at 4500
5. Waits for price to reach 4500
6. Fills when market hits 4500

### Limit Sell Order Example

**Setup**: Want to sell position at 4550 (take profit)
1. From open position (bought at 4500)
2. Right-click position
3. Select "Place Limit Sell"
4. Target price: 4550
5. Quantity: 1 contract
6. Fills when price reaches 4550

### When to Use Limit Orders

- **Specific entry prices**: Want entries at exact levels
- **Support/resistance**: Enter at key technical levels
- **Tight risk control**: Reduce slippage impact
- **Pre-planned exits**: Pre-set take profit levels
- **Lower cost**: Avoid overpaying for entry

## Stop Orders (Stop-Loss)

### What is a Stop Order?

A stop order becomes a market order when price reaches your stop level:
- **Trigger price**: Price that activates order
- **Execution**: Market order once triggered
- **Use case**: Risk protection, automatic loss limiting

### How Stop Orders Work

1. **Specify stop price**: Your loss-limit price
2. **Place stop order**: Set quantity
3. **Order waits**: Remains dormant above/below trigger
4. **Price hits trigger**: Becomes market order automatically
5. **Executes at market**: Fills at market price (may exceed stop)

### Stop Loss Buy Example

**Short position setup**:
- Short 1 ES at 4500
- Want to limit loss at 4510 (10-point stop)

1. Right-click position
2. Select "Place Stop Buy"
3. Stop price: 4510
4. Quantity: 1 contract
5. Price rises to 4510
6. Converts to market buy
7. Fills, stopping short loss

### Stop Loss Sell Example

**Long position setup**:
- Long 1 ES at 4500
- Want to limit loss at 4490 (10-point stop)

1. Right-click position
2. Select "Place Stop Sell"
3. Stop price: 4490
4. Quantity: 1 contract
5. Price drops to 4490
6. Converts to market sell
7. Stops the loss

### When to Use Stop Orders

- **Risk management**: Protect against catastrophic losses
- **Automatic exits**: Don't want to monitor position
- **Pre-set stops**: Disciplined loss limiting
- **Portfolio protection**: Quick exit on key levels

## Stop-Limit Orders

### What is a Stop-Limit Order?

A stop-limit order combines stop and limit functionality:
- **Stop price**: Triggers the order
- **Limit price**: Maximum/minimum execution price
- **Use case**: More control than stop orders

### How Stop-Limit Orders Work

1. **Price hits stop level**: Order becomes limit order
2. **Limit price active**: Only fills at limit price or better
3. **May not fill**: If market gaps past limit price
4. **More control**: Prevents excessive slippage on stop fill

### Stop-Limit Example

**Long position at 4500:**
- Stop at 4490 (limit loss)
- Limit at 4485 (don't sell below 4485)

1. Price falls to 4490
2. Order activates
3. Becomes limit sell at 4485
4. Fills at 4485 or better
5. Won't fill below 4485

### When to Use Stop-Limit Orders

- **Volatile markets**: Prevent extreme slippage
- **Gap risk**: Don't want bad fills on gaps
- **Precision stops**: Exact loss amount
- **News events**: Before volatile announcements

## Advanced Order Types

### Trailing Stop Orders

A stop loss that moves up with profitable positions:
- **Fixed distance**: Stays X points below price
- **Automatic movement**: Adjusts as price moves favorably
- **Loss protection**: Locks in profits as you rise

**Trailing Stop Example:**
- Buy ES at 4500
- Set trailing stop 20 points
- Price goes to 4520: Stop moves to 4500 (breakeven)
- Price goes to 4550: Stop moves to 4530
- Price drops to 4530: Stop triggers, closes at 4530

### Conditional Orders

Orders that activate based on conditions:
- **If-then logic**: "If price breaks 4510, place buy at 4515"
- **Multiple conditions**: Combine several conditions
- **Automated entries**: Entry triggers on specific events

### One Cancels Other (OCO)

Two orders where filling one cancels the other:
- **Take profit order**: Limit order at profit target
- **Stop loss order**: Stop order at loss limit
- **Automatic**: Whichever fills first cancels the other
- **Efficient**: No manual management needed

**OCO Example:**
- Position at 4500
- OCO setup:
  - Take profit at 4550 (sells 1 contract)
  - Stop loss at 4490 (sells 1 contract)
- Whichever hits first executes
- Other automatically cancels

## Order Entry Methods in Backtesting

### Method 1: Chart Clicking

1. **Click on chart** at your desired entry price
2. **Select order type** from menu
3. **Confirm quantity**
4. **Order places** on the chart

### Method 2: Keyboard Shortcuts

| Order Type | Windows | Mac |
|-----------|---------|-----|
| Market Buy | B | B |
| Market Sell | S | S |
| Limit Buy | L | L |
| Limit Sell | K | K |
| Stop Buy | Alt+B | Option+B |
| Stop Sell | Alt+S | Option+S |

### Method 3: Order Panel

1. **Right-click position** (for exits)
2. **Select order type**
3. **Enter price and quantity**
4. **Confirm order**

### Method 4: Drag-and-Drop

1. **Drag from entry level** to target level
2. **Automatically creates** limit order
3. **Release at price** sets order

## Order Execution Rules

### Realistic Execution

TradeZella simulates realistic execution:
- **Slippage**: Based on market volatility
- **Spreads**: Bid/ask spread applied
- **Volume**: Orders may not fill in thin markets
- **Gaps**: Orders skip price levels on gaps
- **Overnight gaps**: Gaps on overnight/weekend moves

### Fill Assumptions

- **Market orders**: Fill immediately at market price
- **Limit orders**: Fill only at limit price or better
- **Stop orders**: Fill at market after stop triggered
- **During candle close**: Fills at close price

## Order Combinations

### Entry + Exit Strategy

**Example: Simple Trade Setup**
1. **Limit buy at 4500**: Patient entry
2. **Limit sell at 4550**: Take profit target
3. **Stop sell at 4490**: Risk control

Result: Defined risk/reward, disciplined execution

### Scaling Out with Orders

1. **Initial entry**: Market buy 100 contracts
2. **First exit**: Limit sell 25 contracts at 4510
3. **Second exit**: Limit sell 25 contracts at 4520
4. **Final exit**: Stop sell 50 contracts at 4480

Result: Systematic profit-taking with protection

## Testing Order Types Through Backtesting

### Questions to Answer

1. **Do limit orders fill often enough?** Too conservative?
2. **Does slippage kill your trades?** Maybe use limit orders?
3. **What stop distance works best?** Test different levels
4. **Should you use OCO orders?** More efficient?
5. **Is market entry necessary?** Or can you wait for limits?

### Order Type Optimization

Through backtesting, optimize:
- **Limit prices**: Find best entry points
- **Stop placement**: Identify optimal stop distances
- **Order combinations**: Best entry/exit mix
- **Execution strategy**: Market vs limit decision rules

---

## See also
- [How to Create a Backtesting Session](./create-backtesting-session.md)
- [How to Take Partials in Backtesting](./take-partials-backtesting.md)
- [Understanding Different Order Types in TradeZella Backtesting](./order-types-backtesting.md)
