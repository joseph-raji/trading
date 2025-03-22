# 📈 Trading

## What You’ll Learn
- Implement a trading strategy  
- Backtest it using historical data  

---

## Strategy Development Steps

1. Download price data  
2. Add indicators  
3. Define entry/exit signals  
4. Implement the strategy  
5. Backtest   

---

## Bollinger Scalping Strategy  
**Timeframe:** 5-minute candles

### Indicators
- **EMA (30 & 50):** Detect trend direction  
- **ATR:** Define stop loss and take profit  
- **Bollinger Bands (15):** Identify overbought/oversold conditions  

### Signal Logic
- EMA crossover over 7 candles → Buy (`2`) or Sell (`1`)  
- Price deviation > 1.5σ from 15-period SMA → Confirm signal  
- Final signal = intersection of both conditions  

### Trade Rules
- Only one trade open at a time  
- SL/TP based on:
  - `TPSL` ratio  
  - `SL_coef` derived from ATR  
