# Changelog

All notable changes to the VantageLogics Order Block Finder will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [1.1.0] - 2026-01-09

### Added
- **Multi-Timeframe (MTF) Support** - Display higher timeframe Order Blocks on lower timeframe charts
  - New setting: Enable Higher Timeframe OBs (default: OFF)
  - New setting: Higher Timeframe selection (4H, D, W, M)
  - New setting: HTF Order Blocks to Show (1-5)
  - New setting: Customizable HTF Bullish/Bearish colors
- MTF OB mitigation tracking on current timeframe
- Distinct visualization for HTF OBs (blue for bullish, red for bearish)
- HTF labels showing timeframe and grade

### Changed
- Statistics panel now shows on all timeframes (previously D/4H only)
- Added timeframe display in statistics panel
- Added "Show Statistics Panel" toggle setting

---

## [1.0.1] - 2026-01-09

### Changed
- Adjusted A+ signal threshold from 2.0 to 1.6 for balanced frequency (~15-20%)
- Proportionally adjusted Grade A threshold to 1.4
- Proportionally adjusted Grade B threshold to 1.2

### Fixed
- Statistics panel now shows actual Bull/Bear counts instead of fabricated metrics
- Replaced misleading "Signal Quality 85%" with real A+ percentage

---

## [1.0.0] - 2026-01-09

### Added
- Initial release of VantageLogics Order Block Finder
- **Order Block Detection**
  - Bullish OB: Last bearish candle before strong upward breakout
  - Bearish OB: Last bullish candle before strong downward breakout
  - SMC-compliant detection logic
- **Strength Grading System**
  - A+ (Premium): Gold visualization, highest conviction
  - A: Strong signal
  - B: Moderate signal
  - C: Weak signal
- **Mitigation Tracking**
  - Detects when price returns to OB zones
  - Visual indicators: dashed borders, [M] labels
- **Non-Repainting Logic**
  - All calculations guarded by `barstate.isconfirmed`
  - What you see is what you get
- **Performance Optimization**
  - `var` keyword for persistent arrays
  - Efficient array management with size limits
  - Cached ATR calculations
- **Brand-Conscious Design**
  - Void Black (#050507) background
  - Pure White (#FFFFFF) standard elements
  - Vantage Gold (#FCD34D) for A+ signals
- **Customizable Settings**
  - Show Recent Order Blocks (1-10)
  - Order Block Lookback Period (20-500)
  - Minimum OB Strength Ratio (1.0-3.0)
  - Toggle: Trigger Candles, Boxes, Labels, Mitigated OBs
- **Alert System**
  - New Bullish Order Block alert
  - New Bearish Order Block alert
  - Premium (A+) Bullish OB alert
  - Premium (A+) Bearish OB alert

---

## Roadmap

### Planned Features

- [ ] Fair Value Gap (FVG) Scanner integration
- [ ] Break of Structure (BOS) detection
- [ ] Change of Character (CHoCH) analysis
- [ ] Confluence grading system
- [ ] Additional alert conditions
- [ ] Performance dashboard

---

## Links

- [TradingView Publication](https://www.tradingview.com/)
- [GitHub Repository](https://github.com/)
- [VantageLogics.ai](https://vantagelogics.ai/)
