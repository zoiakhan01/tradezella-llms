---
title: How to Switch Between Regular and Extended Trading Hours in TradeZella
description: Toggle between regular and extended/pre-market/after-hours sessions
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/11379735-how-to-switch-between-regular-and-extended-trading-hours-in-tradezella
  md: https://www.tradezella.com/help-center/faqs/extended-trading-hours.md
---

# How to Switch Between Regular and Extended Trading Hours in TradeZella

TradeZella supports trading during both regular market hours and extended trading sessions (pre-market and after-hours). The platform allows you to toggle between regular and extended hours views, helping you analyze trades executed outside normal market hours. This is particularly important for traders who participate in pre-market or after-hours sessions, or who trade assets that have different market hour conventions globally.

Understanding extended trading hours is essential for accurate trade analysis and compliance with your broker's requirements. Different assets have different extended hour availability—US equities offer pre-market and after-hours trading, while futures markets have nearly 24-hour sessions, and cryptocurrency trades continuously. TradeZella's extended hours functionality ensures your trades are properly categorized and analyzed according to the actual market conditions they occurred in.

## Understanding Trading Sessions

### Regular Market Hours (US Equities)
- **Opening Time:** 9:30 AM ET
- **Closing Time:** 4:00 PM ET (16:00 ET)
- **Duration:** 6.5 hours per trading day
- **Volume:** Highest liquidity and trading volume
- **Spreads:** Tightest bid-ask spreads
- **Default view:** TradeZella shows regular hours by default

### Pre-Market Session (Early Trading)
- **Start Time:** 4:00 AM ET
- **End Time:** 9:30 AM ET (market open)
- **Duration:** 5.5 hours
- **Volume:** Lower liquidity, wider spreads
- **Participants:** Institutions, professional traders, market makers
- **Use Cases:** Traders reacting to overnight news or economic data

### After-Hours Session (Evening Trading)
- **Start Time:** 4:00 PM ET (market close)
- **End Time:** 8:00 PM ET
- **Duration:** 4 hours
- **Volume:** Lower liquidity, wider spreads
- **Participants:** Institutions, swing traders, option expirations
- **Use Cases:** Reacting to earnings announcements, handling gap trades

### 24-Hour Markets
- **Forex:** Trades Sunday evening through Friday evening continuously
- **Cryptocurrency:** Trades 24/7 every day
- **Futures:** Most contracts trade nearly 24 hours with brief maintenance windows
- No regular/extended hours distinction needed

## Switching Between Trading Hours

### In Chart View
1. Open the **Charts** module in TradeZella
2. Load a stock chart
3. Look for the **"Trading Hours"** toggle or dropdown (typically top-right of chart)
4. Select:
   - **Regular Hours:** Shows only 9:30 AM - 4:00 PM ET
   - **Extended Hours:** Shows pre-market (4:00 AM) through after-hours (8:00 PM)
5. Chart redraw with selected hours, eliminating data outside the selected range

### In Trade Journal View
1. Navigate to **Trade Journal** or **Trades** tab
2. Use **Filters** to access trading hours options
3. Select **"Trading Hours"** filter
4. Choose:
   - **All Hours:** Shows trades from any time
   - **Regular Hours Only:** Shows only 9:30 AM - 4:00 PM ET trades
   - **Extended Hours Only:** Shows pre-market + after-hours trades
5. Results filter to show only trades from selected time periods

### In Settings
1. Go to **Settings > Trading Preferences**
2. Look for **"Default Chart Hours"** setting
3. Select your preference:
   - **Regular Hours:** Default view
   - **Extended Hours:** Default view
4. This becomes your default for all new charts
5. You can still manually override on individual charts

## Analyzing Extended Hours Trades

### Comparing Performance
1. Filter to **Extended Hours Only** trades
2. Review metrics: win rate, avg win, avg loss, trade expectancy
3. Compare these metrics to your **Regular Hours** performance
4. Question: Do you trade better during regular hours or extended hours?

### Pre-Market vs. After-Hours Performance
1. Create two filter views: one for pre-market trades, one for after-hours
2. Tag trades with time-of-day (pre-market, regular, after-hours)
3. Analyze if certain strategies work better at certain times
4. Some traders find they have an edge in pre-market breakouts but lose in after-hours

### Volatility Impact
- Extended hours typically have lower volume and wider spreads
- Compare your average R-multiple and win rates between hours
- Example: You might win 60% during regular hours but only 50% in extended hours due to volatility

## Extended Hours Trading Considerations

### Liquidity Challenges
- **Pre-market and after-hours** have significantly lower trading volume
- Wider bid-ask spreads can negatively impact your entry and exit prices
- Large position sizes may move the market or fail to fill

### Price Gaps
- Overnight gaps from after-hours trading can create large morning openings
- Asian market moves might gap US markets at the 4:00 AM pre-market open
- Your stop losses should account for possible gap risk

### Lower Trading Volume
- Lower trading volume means:
  - Fewer shares available at the best bid/ask price
  - Wider spreads (larger cost per trade)
  - Potentially harder to exit positions
  - More volatile price action

### Broker Connectivity
- Not all brokers support extended hours trading
- Some brokers charge higher commissions for extended hours
- Check your broker's specific extended hours policies

## Best Practices for Extended Hours Trading

**Test Your Strategy:** Use filters to analyze historical performance of your strategies during extended hours vs. regular hours. Do you have an edge?

**Understand Liquidity:** Realize that extended hours have lower liquidity. Adjust position sizes or use limit orders rather than market orders.

**Account for Gaps:** Your risk management should account for possible gaps at market open. Don't place stops too tight.

**Use More Conservative Stops:** Wide spreads in extended hours mean your stops should be placed wider to account for normal volatility vs. adverse movement.

**Document Session Type:** Tag trades with when they occurred (pre-market, regular, after-hours) so you can later analyze session-specific performance.

**Monitor Before Trading:** Check the economic calendar and overnight news before trading pre-market. Major announcements can cause volatility.

**Limit Extended Hours Activity:** Many professional traders restrict their extended hours trading to specific setups they've validated historically.

## Extended Hours for Different Assets

### Equities & ETFs
- Pre-market: 4:00 AM - 9:30 AM ET
- Regular: 9:30 AM - 4:00 PM ET
- After-hours: 4:00 PM - 8:00 PM ET

### Futures Contracts
- Most trade 23 hours per day with 1-hour maintenance windows
- No distinction between regular and extended hours
- TradeZella shows all trading times available

### Forex
- Trades Sunday evening (5:00 PM ET) through Friday evening (5:00 PM ET)
- Continuous trading, no regular/extended distinction
- Different currency pairs may have slight timing variations

### Options
- Trade during regular hours only (9:30 AM - 4:00 PM ET) in most cases
- Some brokers offer extended options trading

### Cryptocurrency
- 24/7 trading on most exchanges
- No market hours concept
- Monitor to understand if your trades occurred during different global market sessions

---

## See also
- [How to Filter Your Trades in TradeZella](/help-center/faqs/how-to-filter-trades.md)
- [Exploring the Economic Calendar in TradeZella](/help-center/faqs/economic-calendar.md)
- [What Trading Assets Are Supported?](/help-center/faqs/supported-trading-assets.md)
