# 📈 EMA 10/50 Trend Pullback Strategy – Pine Script v5

This is a TradingView strategy script designed to trade **pullbacks to EMA 10** in the direction of a strong trend defined by **EMA 10 and EMA 50**. It aims to capture low-risk entries during trending conditions using a simple set of rules.

---

## ✅ Strategy Logic

### 🔻 Sell Setup (Short Trade)
- Price is **above EMA 10** and **EMA 50**
- EMA 10 is **above** EMA 50 (uptrend confirmation)
- Candle **touches EMA 10**
- The **open of the candle** is still **above EMA 10**
- **Only one open trade at a time**

### 🔼 Buy Setup (Long Trade)
- Price is **below EMA 10** and **EMA 50**
- EMA 10 is **below** EMA 50 (downtrend confirmation)
- Candle **touches EMA 10**
- The **open of the candle** is still **below EMA 10**
- **Only one open trade at a time**

### 🔚 Exit Conditions
- For long trades: exit when **price closes above EMA 10**
- For short trades: exit when **price closes below EMA 10**

---

## 📊 Indicators Used
- **EMA 10** (fast)
- **EMA 50** (slow)

These EMAs define trend direction and serve as dynamic support/resistance levels for trade entries and exits.

---

## 🔒 Risk Management
- No pyramiding (one open trade per direction only)
- Exits are clean and rule-based
- No stop loss or take profit is implemented in this version

---

## 🚀 How to Use
1. Copy and paste the script into TradingView's **Pine Editor**
2. Click **Add to Chart** or **Add Strategy**
3. Adjust EMAs or optimize in strategy tester if needed

---

## 🧠 Notes
- Works best in **strong trending markets**
- Avoid using it in **choppy or sideways conditions**
- You can add filters like RSI, volume, or ADX to improve performance

---

## 📦 To-Do / Extensions
- [ ] Add Stop Loss / Take Profit logic
- [ ] Add Trading Sessions filter (London, NY, etc.)
- [ ] Add alert conditions
- [ ] Add visual trade markers (entry/exit arrows)

---

## 🧾 License
This script is open for personal or educational use. Not financial advice. Use at your own risk.

