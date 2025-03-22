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
6. Parameter Optimization

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
---

## Result
![image](https://github.com/user-attachments/assets/17213bec-4bdf-44d0-957e-be797546b86b)

## Parameter Optimization result
![image](https://github.com/user-attachments/assets/9704642c-277b-4970-9bc8-6257a1032fa3)

