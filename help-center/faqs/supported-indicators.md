---
title: List of Supported Indicators in TradeZella
description: Full list of technical indicators available including moving averages, RSI, MACD, and ICT-specific indicators
lastUpdated: 2026-03-04
source_url:
  html: https://help.tradezella.com/en/articles/10502927-list-of-supported-indicators-in-tradezella
  md: https://www.tradezella.com/help-center/faqs/supported-indicators.md
---

# List of Supported Indicators in TradeZella

TradeZella's charting platform includes a comprehensive suite of technical indicators covering trend, momentum, volatility, and volume analysis. Whether you're a traditional technical analyst using moving averages and MACD, or a price action trader using ICT (Inner Circle Trading) concepts, TradeZella provides the tools needed for various trading methodologies. All indicators are fully customizable with adjustable periods, colors, and display options to match your trading style.

The indicator library is continuously updated to include both classic technical analysis tools and emerging indicators used by modern traders. Each indicator has built-in reasonable defaults while allowing full customization for advanced traders. Indicators can be overlaid on charts, displayed in separate panels, or used in combination to create custom trading systems. Many indicators integrate with TradeZella's alerting system so you can receive notifications when specific conditions are met.

## Trend Indicators

### Moving Averages
- **Simple Moving Average (SMA):** Unweighted average of closing prices over N periods
- **Exponential Moving Average (EMA):** Weighted average giving more weight to recent prices
- **Weighted Moving Average (WMA):** Moving average with linearly increasing weights
- **Adaptive Moving Average:** Adjusts period based on market volatility (Kaufman AMA)
- **Hull Moving Average:** Faster, less lag than traditional moving averages
- **VWAP (Volume Weighted Average Price):** Price average weighted by trading volume
- **VWMA (Volume Weighted Moving Average):** Moving average incorporating volume

**Customization Options:**
- Period length (e.g., 20-day, 50-day, 200-day)
- Color, line style (solid, dashed, dotted)
- Display multiple averages simultaneously
- Use as levels/bands rather than lines

### MACD (Moving Average Convergence Divergence)
- Shows relationship between two moving averages
- Displays: MACD line, signal line, histogram
- Generate signals from line crossovers
- Used for trend confirmation and momentum

### ADX (Average Directional Index)
- Measures trend strength (not direction)
- Values above 25 indicate strong trend
- Values below 20 indicate weak trend
- Useful for filtering ranging vs. trending markets

### Parabolic SAR (Stop and Reverse)
- Shows trend direction and provides stop loss levels
- SAR dots appear below price in uptrends, above in downtrends
- Useful for trailing stops
- Alerts when SAR flips (potential reversal)

### Ichimoku Cloud
- Comprehensive indicator showing support, resistance, and trend
- Components: Tenkan (conversion), Kijun (baseline), clouds, lagging line
- Shows multiple timeframes of support/resistance
- Popular in Japanese price action trading

## Momentum Indicators

### RSI (Relative Strength Index)
- Measures momentum on scale from 0-100
- Values above 70 = overbought
- Values below 30 = oversold
- Standard period = 14
- Custom periods available (7, 21, etc.)

### Stochastic Oscillator
- Compares closing price to price range
- Two lines: %K (fast) and %D (slow signal)
- Overbought above 80, oversold below 20
- Shows momentum and potential reversals

### CCI (Commodity Channel Index)
- Measures cyclical trends in commodities and other assets
- Values above 100 = strong uptrend
- Values below -100 = strong downtrend
- Good for mean-reversion setups

### ROMC (Rate of Change)
- Shows percentage change over N periods
- Positive values = uptrend momentum
- Negative values = downtrend momentum
- Useful for divergences with price

### KDJ Indicator
- Similar to Stochastic but with additional signal line
- Three lines: K, D, J
- Primarily used in Asian markets
- Good for short-term trading

## Volatility Indicators

### Bollinger Bands
- Shows mean (SMA) with upper/lower bands based on standard deviation
- Band width indicates volatility level
- Price touching upper band = potential resistance
- Price touching lower band = potential support
- Adjustable period and standard deviation multiplier

### ATR (Average True Range)
- Measures volatility over recent periods
- Higher ATR = higher volatility
- Lower ATR = lower volatility
- Useful for position sizing (wider stops in high ATR environments)

### Keltner Channels
- Similar to Bollinger Bands but uses ATR instead of standard deviation
- Less whipsaw in trending markets
- Good for breakout confirmation

### Standard Deviation
- Measures how far prices deviate from the mean
- Higher standard deviation = higher volatility
- Used to establish Bollinger Band width

### Historical Volatility
- Calculated standard deviation of past returns
- Shows actual realized volatility
- Useful for options traders assessing option value

## Volume Indicators

### Volume (On-Chart)
- Displays volume bars below price chart
- Color coding: bullish volume (green), bearish volume (red)
- Height shows relative volume strength
- Identify high-volume support/resistance levels

### Volume Moving Average
- Average volume over N periods (typically 20-day)
- Compare current volume to average
- High volume on breakouts = confirmation
- Low volume breakouts = weak signal

### OBV (On-Balance Volume)
- Accumulates volume for up and down days
- OBV rising = volume supporting uptrend
- OBV falling = volume supporting downtrend
- Good for confirming trend strength

### VWAP (Volume Weighted Average Price)
- Already listed under Trend Indicators
- Important for institutional traders
- Daily VWAP resets at market open

### Money Flow Index (MFI)
- Combines price and volume to measure buying/selling pressure
- Scale 0-100 (similar to RSI but volume-weighted)
- Values above 80 = overbought
- Values below 20 = oversold

### Accumulation/Distribution (A/D)
- Measures cumulative buying and selling pressure
- Uses closing price position within the day's range and volume
- Rising A/D line confirms uptrend
- Divergences signal potential reversals

## ICT (Inner Circle Trading) Specific Indicators

### Fair Value Gap (FVG)
- Areas where price gaps in the order flow
- Imbalance between buyers and sellers
- Potential areas of price return/rejection
- Customizable gap size threshold

### Order Block
- Prior candlestick before a significant move
- Support/resistance level for future pullbacks
- Identifies areas of liquidity
- Can be manually drawn or auto-detected

### Breaker Block
- Order block that was breached by price
- Often provides strong support/resistance on retest
- Used for mean-reversion entries

### Liquidity Level
- Areas where stops or limit orders are clustered
- Price often moves to "grab liquidity" before reversing
- Marked at obvious round numbers or technical levels
- Useful for predicting short-term price action

### Displacement
- Large candle or series of candles showing strong directional move
- Often followed by consolidation or pullback
- Indicates strong buying/selling pressure
- Used to identify trend exhaustion

### Smart Money Concepts
- Custom indicator package based on ICT methodology
- Shows: FVG, order blocks, liquidity levels, displacement
- Can enable/disable individual components
- Popular with price action traders

## Statistical Indicators

### Linear Regression
- Best-fit line through recent price data
- Shows overall trend direction and rate
- Bands around regression line show standard error
- Good for identifying trend strength

### Correlation
- Measures how two symbols move together
- Values +1 = perfectly correlated
- Values -1 = perfectly inversely correlated
- Useful for portfolio analysis and pair trading

### Beta
- Measures volatility relative to a benchmark (e.g., SPY for stocks)
- Beta > 1 = more volatile than market
- Beta < 1 = less volatile than market

## Alert & Notification Indicators

All indicators support custom alerts:
- **Price-based alerts:** Alert when indicator hits specific value
- **Crossover alerts:** Alert when one line crosses another
- **Threshold alerts:** Alert when indicator crosses above/below level
- **Alert notifications:** Popup, email, SMS, or in-app notification

Example: "Alert when RSI crosses below 30" or "Alert when price closes above 200-day EMA"

## Using Multiple Indicators Together

### Popular Combinations
- **Trend Confirmation:** Use EMA for trend + MACD for momentum
- **Entry Signals:** RSI oversold + Price at support + Volume spike
- **Exit Signals:** RSI overbought or MACD histogram divergence
- **Risk Management:** ATR for stop placement, volume for breakout confirmation

### Best Practices
- Start with 2-3 core indicators rather than 10+
- All indicators should serve your trading plan
- Use indicators to confirm price action, not replace it
- Test combinations on historical data before trading live

## Indicator Settings & Customization

### Period/Length Settings
- Most indicators allow period adjustment
- Shorter periods = more sensitive, more false signals
- Longer periods = slower, fewer false signals
- Test different periods to match your timeframe and style

### Color & Display Options
- Customize colors for personal preference
- Adjust line thickness for visibility
- Choose display mode: overlay on chart, separate panel, or both

### Indicator Calculation Methods
- Some indicators offer alternative calculation methods
- Example: RSI uses "wilder's smoothing" vs. "ema smoothing"
- Test different methods to see which works best for your setup

## Chart Panel Management

### Overlay Indicators
- Display directly on the price chart
- Examples: Moving averages, Bollinger Bands, VWAP
- Can stack multiple overlays
- Be careful not to clutter the chart

### Separate Panel Indicators
- Display in dedicated panels below or beside the chart
- Examples: RSI, MACD, Volume, OBV
- Can create multiple panels for different indicator families
- Resize panels to adjust visibility

### Indicator Menu
- Access all available indicators from the Indicators menu
- Add/remove indicators instantly
- Modify settings without closing/reopening

---

## See also
- [List of Supported Indicators in TradeZella](/help-center/faqs/supported-indicators.md)
- [How to Copy Drawings from TradingView to TradeZella](/help-center/faqs/copy-drawings-tradingview.md)
- [Extended Trading Hours in TradeZella](/help-center/faqs/extended-trading-hours.md)
