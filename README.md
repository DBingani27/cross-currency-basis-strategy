# Cross-Currency Basis Quant Strategy

This project investigates arbitrage opportunities and USD funding stress using the USD/JPY cross-currency basis. It combines econometric regression, PCA, and trading signal backtests to evaluate two systematic FX strategies.

---

## 📊 Strategies

### 1. Mean Reversion Strategy
- Trades when USD/JPY basis deviates from its historical mean
- Z-score entry/exit logic
- Strong Sharpe Ratio and low drawdown

### 2. PCA-Based Strategy
- Uses principal component analysis across USD/JPY and USD/EUR basis
- Attempts to isolate stress-driven signals (PC1)
- Underperformed in backtests

---

## 📈 Sample Plot

![Cumulative PnL](path_to_your_uploaded_image_or_remove_this)

---

## 🔧 Tools & Methods

- Python (pandas, sklearn, statsmodels, matplotlib)
- Linear Regression: basis ~ VIX + TED + Fed Liquidity
- PCA: extract common factor from USD/JPY and USD/EUR basis
- Signal generation using Z-scores
- Strategy backtest and performance metrics

---

## 📁 Files

- `Cross_Currency_Basis_Final_Notebook.ipynb` – full project notebook
- `merged_data.csv` – macroeconomic and basis series (optional)

---

## 📚 Results

| Strategy       | Total Return | Sharpe Ratio | Max Drawdown | Win Rate |
|----------------|--------------|---------------|--------------|----------|
| Mean Reversion | 24.49        | 5.46          | -6.77%       | 13.98%   |
| PCA-Based      | -24.53       | -5.46         | -24.53%      | 0.96%    |

---

## 💡 Conclusion

The USD/JPY cross-currency basis shows predictable mean-reverting behavior that can be exploited using statistical triggers. PCA may provide additional insights into systemic stress, but requires better filtering to generate tradeable signals.

---
