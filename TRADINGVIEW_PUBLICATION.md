# TradingView Publication Description

## Title
VantageLogics Order Block Finder [SMC]

## Short Description (for script header)
Institutional-grade Order Block detection with strength grading. Non-repainting SMC methodology.

---

## Full Description (Copy this to TradingView)

### What is an Order Block?

An **Order Block (OB)** is a price zone where institutional traders (banks, hedge funds) placed large orders that caused a significant price move. These zones often act as **support/resistance** when price returns to them.

**Think of it like this:** When a big player buys heavily at a price, that zone becomes "defended" - if price comes back, there's often buying interest waiting there.

---

### How This Indicator Works

**Bullish Order Block (Buy Zone)**
- Detects the last bearish candle before a strong upward breakout
- Price breaking above with momentum signals institutional buying
- When price returns to this zone = potential BUY opportunity

**Bearish Order Block (Sell Zone)**
- Detects the last bullish candle before a strong downward breakout
- Price breaking below with momentum signals institutional selling
- When price returns to this zone = potential SELL opportunity

---

### Understanding the Grades

Each Order Block receives a strength grade:

| Grade | Meaning | What to Do |
|-------|---------|------------|
| **A+** (Gold) | Strongest signal - high institutional conviction | Best trade opportunities |
| **A** | Strong signal | Good trade setups |
| **B** | Moderate signal | Use with confluence |
| **C** | Weak signal | Requires additional confirmation |

**Pro Tip:** Focus on A+ and A grade Order Blocks for highest probability trades.

---

### How to Trade with This Indicator

#### Step 1: Identify the Order Block
- **Gold box** = A+ premium signal (highest conviction)
- **White box** = Standard signal (A, B, or C grade)
- **Dashed box** = Mitigated (price already tested the zone)

#### Step 2: Wait for Price to Return
- Order Blocks work when price **comes back** to the zone
- This is called "mitigation" - marked with `[M]` on the label
- The first touch of an unmitigated OB often provides the best entry

#### Step 3: Entry Strategy

**For Bullish OB (Buy):**
1. Wait for price to drop INTO the OB zone
2. Look for bullish confirmation (engulfing candle, pin bar, etc.)
3. Enter long with stop-loss below the OB zone
4. Target: Previous swing high or 1:2 risk-reward

**For Bearish OB (Sell):**
1. Wait for price to rise INTO the OB zone
2. Look for bearish confirmation (engulfing candle, shooting star, etc.)
3. Enter short with stop-loss above the OB zone
4. Target: Previous swing low or 1:2 risk-reward

---

### Reading the Statistics Panel

On Daily and 4-Hour charts, you'll see a statistics panel showing:
- **Bull / Bear count**: Total Order Blocks detected in each direction
- **A+ Signals**: Number and percentage of premium-grade signals

**Interpretation:**
- High A+ percentage (>30%) = Market showing clear institutional activity
- Balanced Bull/Bear = Ranging market, trade both directions
- One-sided dominance = Trending market, trade with the trend

---

### Multi-Timeframe (MTF) Feature

The MTF feature allows you to see **higher timeframe Order Blocks on your lower timeframe chart**. This is powerful for:

**Example Workflow:**
1. Enable "Higher Timeframe OBs" in settings
2. Select "D" (Daily) as your higher timeframe
3. View your chart on 1H or 4H
4. You'll see Daily OBs displayed with colored boxes (Blue = Bullish, Red = Bearish)
5. Use the Daily OB zones to identify high-probability entry areas on lower timeframes

**MTF Settings:**
| Setting | Default | Description |
|---------|---------|-------------|
| Enable Higher Timeframe OBs | OFF | Toggle MTF display |
| Higher Timeframe | D | Select: 4H, D, W, M |
| HTF Order Blocks to Show | 2 | How many HTF OBs to display |
| HTF Bullish OB Color | Blue | Customize bullish zone color |
| HTF Bearish OB Color | Red | Customize bearish zone color |

**Pro Tip:** Identify OBs on Daily, then drop to 4H/1H to find precise entries within those zones.

---

### Best Practices

**DO:**
- Use on higher timeframes (4H, Daily) for strongest signals
- Wait for price to return to OB zones before trading
- Combine with trend analysis (trade OBs in trend direction)
- Use proper risk management (1-2% per trade)
- Use MTF to identify Daily/Weekly OBs while trading intraday

**DON'T:**
- Trade every Order Block - focus on A+ and A grades
- Enter immediately when OB forms - wait for mitigation
- Ignore the overall trend - OBs work best with trend confluence
- Risk more than you can afford to lose

---

### Settings Guide

| Setting | Recommended | Description |
|---------|-------------|-------------|
| Show Recent Order Blocks | 2-5 | More = cluttered chart, fewer = cleaner view |
| Order Block Lookback | 100 | Increase for more history, decrease for recent only |
| Minimum OB Strength | 1.5 | Higher = fewer but stronger signals |
| Show Mitigated OBs | ON | Helps track which zones are "used up" |

---

### FAQ - Common Questions

**Q: Why do I see different signals on different timeframes?**

This is **normal and expected**. Each timeframe shows its own market structure:
- **Daily** shows institutional positioning over days/weeks
- **4H/1H** shows shorter-term price movements

Example: Daily shows Bearish OB while 1H shows Bullish OB means there's a short-term bounce within a larger bearish trend. Experienced traders use this information for confluence - when both timeframes align, signals are stronger.

**Q: Why is my A+ percentage different on 1D vs 4H?**

Different timeframes have different price action characteristics. Higher timeframes (Daily, Weekly) typically show cleaner institutional moves, while lower timeframes have more noise. This is why many traders prefer 4H+ for Order Block analysis.

**Q: Should I only trade A+ signals?**

A+ signals have the highest institutional conviction, but A and B grades can also be valid with additional confluence (trend direction, support/resistance, other indicators). C grades should be avoided or require strong confirmation.

**Q: Why did an Order Block "disappear"?**

Order Blocks are removed when:
1. They exceed the lookback period (default: 100 bars)
2. You have "Show Recent Order Blocks" set to a low number

Adjust these settings if you want to see more historical OBs.

**Q: The MTF OBs show different direction than current timeframe OBs?**

This is valuable information! It shows:
- **Aligned** (both bullish or both bearish) = High confluence, stronger signal
- **Conflicting** = Caution, possible reversal or pullback in progress

Pro traders wait for alignment or use the higher timeframe as the "bias" and lower timeframe for entry timing.

---

### Risk Disclaimer

This indicator is a **tool for analysis**, not a trading signal generator.

- Past performance does not guarantee future results
- Always use proper risk management
- Never risk more than you can afford to lose
- This is not financial advice - do your own research

---

### About VantageLogics.ai

Professional Smart Money Concepts methodology for serious traders.

**Features:**
- Non-repainting logic (what you see is what you get)
- Institutional-grade detection algorithms
- Clean, professional visualization
- Performance-optimized code

---

*Free indicator - Use at your own discretion*

---

## Tags (for TradingView)
orderblock, smartmoney, smc, institutional, supplydemand, supportresistance, priceaction, forex, crypto, stocks

## Category
Trend Analysis
