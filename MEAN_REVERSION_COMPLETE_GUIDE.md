# Mean Reversion Trading: Complete Guide

## Overview
**Mean reversion trading** is based on the financial theory that asset prices and historical returns eventually revert to their long-term mean or average level. This strategy assumes that prices fluctuate around a central value and that significant deviations from this average are likely to be corrected over time.

---

## Table of Contents
1. [Core Concepts](#core-concepts)
2. [Key Principles](#key-principles)
3. [Statistical Methods](#statistical-methods)
4. [Trading Indicators](#trading-indicators)
5. [Entry and Exit Signals](#entry-and-exit-signals)
6. [Risk Management](#risk-management)
7. [Position Sizing](#position-sizing)
8. [Common Applications](#common-applications)
9. [Advantages and Disadvantages](#advantages-and-disadvantages)
10. [Best Practices](#best-practices)

---

## Core Concepts

### 1. **The Mean (Average)**
- The "mean" is typically a **moving average** of an asset's price over a set period (e.g., 20-day or 50-day MA)
- Represents the central value to which prices are expected to revert
- Can be calculated using Simple Moving Average (SMA) or Exponential Moving Average (EMA)
- The mean is not static—it changes as new price data is added

### 2. **Reversion**
- When an asset's price **deviates significantly** from its mean (either up or down), it is expected to move back ("revert") toward this average
- This is rooted in the concept of mean-reversion or regression to the mean
- The stronger the deviation, the stronger the expected reversion

### 3. **Overbought/Oversold Conditions**
- **Overbought**: When a price is significantly above its mean
  - Signals a potential **sell opportunity**
  - Suggests the price has been driven up excessively and may fall back
  
- **Oversold**: When a price is significantly below its mean
  - Signals a potential **buy opportunity**
  - Suggests the price has been driven down excessively and may rise back

---

## Key Principles

### 1. **Market Inefficiencies**
- **Assumption**: Investor overreactions and market inefficiencies cause excessive price moves away from the mean
- These are typically followed by corrections/reversions

### 2. **Range-Bound Markets**
- Mean reversion strategies work **best in range-bound or sideways markets**
- Less effective during strong directional trends
- May produce losses if prices trend far from the mean for an extended period

### 3. **The "Mean Can Stay Irrational Longer Than You Can Remain Solvent" Risk**
- Extreme price moves can last longer than expected
- This can cause significant losses even if the strategy is theoretically sound
- Requires proper risk management and stop-losses

### 4. **Time Horizon**
- Mean reversion typically works over **medium to short time horizons**
- Not a long-term buy-and-hold strategy
- More suitable for active traders with defined holding periods

---

## Statistical Methods

### 1. **Z-Score**
**What it measures**: How many standard deviations a price is from the mean

**Formula**:
```
Z = (Price - Mean) / Standard Deviation
```

**Interpretation**:
- Z-score = 0: Price is at the mean
- Z-score = 2: Price is 2 standard deviations above the mean (likely overbought)
- Z-score = -2: Price is 2 standard deviations below the mean (likely oversold)
- Extreme Z-scores (e.g., ±2 or ±3) often precede mean reversion

**Trading Application**:
- Buy when Z-score < -2 (oversold)
- Sell when Z-score > +2 (overbought)

### 2. **Bollinger Bands**
**What it does**: Plots bands at a specified number of standard deviations above and below a moving average

**Structure**:
- Middle band: Moving average (typically 20-period SMA)
- Upper band: Moving average + (2 × Standard Deviation)
- Lower band: Moving average - (2 × Standard Deviation)

**Mean Reversion Signal**:
- When price touches the upper band, it may revert to the mean (middle band)
- When price touches the lower band, it may revert to the mean
- Band squeeze indicates low volatility and potential breakout/mean reversion setup

### 3. **Stationarity Testing (Augmented Dickey-Fuller Test)**
**What it does**: Statistical tests that check if a price series tends to revert to a mean (stationary) or follows a random walk (non-stationary)

**Common Tests**:
- Augmented Dickey-Fuller (ADF) test
- KPSS test

**Importance**: Essential for identifying which assets/pairs exhibit mean-reverting behavior

### 4. **Cointegration (Pairs Trading)**
**What it means**: When two or more stocks/assets move together (cointegrated), divergences suggest mean reversion opportunities

**Application**: Popular in pairs trading where:
- Two correlated stocks move apart
- Traders bet they will converge back together

---

## Trading Indicators

### 1. **Relative Strength Index (RSI)**
**What it measures**: Oscillator that indicates overbought or oversold conditions

**Typical Settings**:
- Period: 14 (standard)
- Overbought threshold: Above 70
- Oversold threshold: Below 30

**Mean Reversion Signal**:
- RSI > 70: Overbought condition → consider selling
- RSI < 30: Oversold condition → consider buying
- Divergences can signal potential reversions

### 2. **Stochastic Oscillator**
**What it compares**: A security's closing price to its price range over a specified period

**Thresholds**:
- Overbought: Above 80
- Oversold: Below 20

**Mean Reversion Signal**:
- When Stochastic > 80, expect reversal downward
- When Stochastic < 20, expect reversal upward

### 3. **Commodity Channel Index (CCI)**
**What it measures**: The deviation of price from its average

**Thresholds**:
- High CCI (above +100): Overbought → potential reversal
- Low CCI (below -100): Oversold → potential reversal

### 4. **Moving Average Convergence Divergence (MACD)**
**Primary Use**: Trend indicator, but can signal mean reversion when:
- MACD line diverges significantly from its moving average
- MACD line crosses zero line (indicating extremes)

### 5. **Simple/Exponential Moving Averages (SMA/EMA)**
**Application**: 
- Prices that strongly diverge from their moving average tend to revert
- Can be combined with volatility measures for stronger signals

---

## Entry and Exit Signals

### Entry Signals
Traders enter mean reversion positions when:
1. Price moves an **extreme distance from the mean** (e.g., 2+ standard deviations)
2. Confirmation from indicators (RSI < 30 or > 70, Bollinger Band extremes, etc.)
3. Market conditions suggest mean reversion rather than trending market

**Entry Examples**:
- **Buy Entry**: Price falls below lower Bollinger Band AND RSI < 30
- **Sell Entry**: Price rises above upper Bollinger Band AND RSI > 70

### Exit Signals
Traders exit mean reversion positions:
1. **Target Exit**: Once the price returns closer to the mean
   - Exit when price crosses the moving average
   - Exit when Z-score returns to 0 or -1/+1
   
2. **Stop Loss Exit**: If the trend continues against the trade
   - Predefined loss limit (e.g., 2% account loss)
   - Price breaks beyond an extended level
   
3. **Time Exit**: If the reversion doesn't occur within a defined timeframe
   - Helps prevent holding losing positions indefinitely

---

## Risk Management

### 1. **Stop Loss Strategy**
- Set a **maximum loss per trade** (fixed percentage or ATR-based)
- Stop losses are critical because mean reversion can fail during strong trends
- Typical stop loss: 1-2% of account per trade

### 2. **Maximum Drawdown Control**
- Define a **maximum drawdown** at which you pause or stop trading
- Prevents catastrophic losses during regime changes
- Helps preserve capital during unfavorable market conditions

### 3. **Avoiding Overfitting**
- Test strategy on **out-of-sample data**
- Use **walk-forward analysis** for robust validation
- Avoid optimizing parameters too specifically to historical data

### 4. **Market Regime Detection**
- **Filter out or avoid trading** during:
  - High volatility periods
  - Strong trending markets
  - Low liquidity environments
  
- Use indicators for regime detection:
  - **ADX (Average Directional Index)**: Identifies trending markets
  - **Volatility filters**: Avoid extreme volatility
  - **Moving average slope**: Identifies trend direction

### 5. **Diversification**
- Apply mean reversion strategies to **multiple uncorrelated assets**
- Reduces risk from concentrated positions
- Helps smooth out returns

---

## Position Sizing

### 1. **Fixed Fractional Method**
**Concept**: Risk a set percentage of capital per trade

**Calculation**:
```
Position Size = (Account Size × Risk %) / Stop Loss (in $ or points)
```

**Example**:
- Account size: $10,000
- Willing to risk: 1% = $100
- Stop loss: 0.5% move = $0.50 per share
- Position size = $100 / $0.50 = **200 shares**

**Typical Risk Percentages**: 0.5% to 2% per trade

### 2. **Volatility-Based Position Sizing**
**Concept**: Adjust position sizes based on current volatility

**Method**:
- Calculate volatility (using ATR or standard deviation)
- **Lower volatility** → Larger positions
- **Higher volatility** → Smaller positions

**Advantages**:
- Handles regime changes better
- Automatically scales positions
- Reduces risk during high-volatility periods

### 3. **Kelly Criterion** (Advanced)
**Concept**: Theoretically maximizes long-term growth

**Caution**: Can be too aggressive for real-world trading due to:
- Estimation errors
- "Fat tails" (extreme events)
- Sequence risk

**Not recommended** for mean reversion strategies without modifications

### 4. **Position Sizing Best Practices**
- **Conservative approach**: Use 0.5-1% risk per trade for mean reversion
- **Scaling in and out**: Can add positions as price deviates further, but use strict limits
- **Correlation awareness**: Don't enter multiple trades on highly correlated assets
- **Event risk**: Reduce position size around earnings, macro events, or major news

---

## Common Applications

### 1. **Stocks**
- Mean reversion within a stock's trading range
- Sector pairs trading (correlated stocks diverging)

### 2. **Forex (Foreign Exchange)**
- Currency pairs reverting to historical averages
- Interest rate differentials creating mean-reverting dynamics

### 3. **Commodities**
- Commodity prices reverting to production costs
- Seasonal patterns creating mean reversion opportunities

### 4. **Options Trading**
- Implied volatility mean reversion
- Options premium decay patterns

### 5. **Crypto**
- Bitcoin and altcoin price reversions
- Correlation pairs trading in crypto markets

### 6. **Pairs Trading**
- Tracking price relationships between two correlated assets
- Entering when the relationship diverges, expecting convergence

---

## Advantages and Disadvantages

### Advantages ✅
1. **Defined Risk**: Stop losses can be set clearly based on extremes
2. **Systematic**: Rules-based approach, easy to backtest
3. **Works in Certain Markets**: Highly effective in range-bound, sideways markets
4. **Scalable**: Can be applied to many assets
5. **Reduces Emotional Trading**: Objective entry/exit criteria

### Disadvantages ❌
1. **Trend Risk**: Fails significantly when strong trends develop
2. **Drawdown Potential**: Extreme moves can last longer than expected, causing large losses
3. **Parameter Sensitivity**: Performance depends heavily on indicator settings
4. **Regime Dependency**: Requires detection and avoidance of trending markets
5. **Whipsaw Risk**: Multiple small losses if price keeps reversing without mean reversion
6. **Limited in Momentum Markets**: Works poorly when momentum is strong in one direction

---

## Best Practices

### 1. **Backtesting Protocol**
- Test on at least 3-5 years of historical data
- Include different market regimes (bull, bear, sideways)
- Use walk-forward analysis to avoid overfitting
- Test on out-of-sample data

### 2. **Market Filtering**
- Only trade mean reversion in range-bound markets
- Avoid strong trending environments
- Use ADX or trend filters to identify suitable markets
- Consider time of day, day of week, and seasonal patterns

### 3. **Position Management**
- Start with smaller position sizes while learning
- Gradually scale up as confidence and track record improve
- Monitor correlation between open positions
- Adjust position size based on current account volatility

### 4. **Continuous Monitoring**
- Regular strategy performance reviews
- Track metrics: Win rate, Profit Factor, Max Drawdown, Sharpe Ratio
- Adjust parameters if market regime shifts
- Be ready to pause strategy if conditions change

### 5. **Multiple Indicators Confirmation**
- Don't rely on a single indicator
- Combine multiple signals for stronger entries
- Example: RSI + Bollinger Bands + Volume confirmation

### 6. **Emotional Discipline**
- Follow the trading plan strictly
- Don't override stops due to "intuition"
- Keep a trading journal to learn from trades
- Accept losses as part of the process

---

## Key Takeaways

1. **Mean reversion** assumes "what goes up must come down (and vice versa)"
2. **Timing and risk management** are crucial for success
3. **Works best in range-bound markets**, struggles in trends
4. **Statistical tools** (Z-score, Bollinger Bands) help identify extremes
5. **Indicator confirmation** strengthens entry signals
6. **Conservative position sizing** (0.5-1% risk per trade) is essential
7. **Regime detection** helps avoid disastrous trend trades
8. **Backtesting and discipline** separate profitable traders from losers

---

## Quick Reference: Setup Template

### Minimal Mean Reversion Setup
1. **Moving Average**: 20-period SMA (for mean)
2. **Deviation Measure**: Bollinger Bands (2 standard deviations) or Z-score
3. **Confirmation Indicator**: RSI (14-period)
4. **Entry**: Price > Upper Band AND RSI > 70 (Sell) OR Price < Lower Band AND RSI < 30 (Buy)
5. **Exit**: Price crosses moving average OR stop loss hit
6. **Position Size**: 1% account risk per trade
7. **Stop Loss**: Beyond the Bollinger Band extreme (typically 2.5-3 standard deviations)

---

**Last Updated**: June 2026

---

