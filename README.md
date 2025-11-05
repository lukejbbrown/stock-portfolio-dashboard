# 📊 Stock Market & Portfolio Diversification Dashboard
A Python-based dashboard that analyzes and visualizes portfolio performance, diversification, and risk metrics using real ETF market data.

---

## 🧠 Overview
This project demonstrates how to build a complete **portfolio analytics and optimization dashboard** in Python.  
It automatically downloads daily ETF prices, calculates key performance metrics, visualizes correlations and risk, and computes the **efficient frontier** with a maximum Sharpe ratio portfolio.

---

## 🚀 Features
✅ **Market Data Automation**  
Fetches daily adjusted close prices for major ETFs via [Yahoo Finance](https://finance.yahoo.com/):
- SPY — U.S. Equities  
- QQQ — Technology  
- EFA — Developed International  
- EEM — Emerging Markets  
- VNQ — Real Estate  
- AGG / BND — Bonds  
- GLD — Gold  

✅ **Portfolio Analytics**
- Annualized return  
- Annualized volatility  
- Sharpe ratio  
- Maximum drawdown  
- Beta vs. S&P 500  

✅ **Visualizations**
- Growth of $1 (performance over time)  
- Correlation heatmap  
- Rolling volatility (6-month window)  
- Portfolio drawdowns  
- Efficient frontier and max-Sharpe portfolio  

✅ **Portfolio Comparisons**
- 60/40 (SPY/AGG) portfolio  
- 100 % Equity portfolio  
- Diversified multi-asset mix  

---

## ⚙️ How It Works
1. **Data Import & Cleaning** – Downloads adjusted close prices and fixes column structure  
2. **Return Calculation** – Computes daily simple returns  
3. **Portfolio Construction** – Weighted aggregation of asset returns  
4. **Performance Metrics** –  
   - Annualized Return = mean × 252  
   - Volatility = std × √252  
   - Sharpe = (Return − RF) / Vol  
   - Max Drawdown = min(Wealth / Peak − 1)  
   - Beta = Cov(Portfolio, SPY) / Var(SPY)  
5. **Optimization** – Uses `scipy.optimize` to build the efficient frontier and locate the maximum-Sharpe portfolio  

---

## 🧩 Tech Stack
- **Language:** Python 3.11  
- **Libraries:** `yfinance`, `pandas`, `numpy`, `matplotlib`, `scipy`  
- **Environment:** Conda / Jupyter Notebook  

---

## 📈 Example Output
| Portfolio | Ann. Return | Ann. Vol | Sharpe | Max Drawdown | Beta vs SPY |
|------------|--------------|-----------|---------|----------------|--------------|
| 60/40 (SPY/AGG) | 6.7 % | 10.2 % | 0.66 | −20.5 % | 0.56 |
| All-Equity | 11.0 % | 15.9 % | 0.69 | −32.8 % | 1.05 |
| Diversified Mix | 7.8 % | 11.8 % | 0.67 | −23.2 % | 0.71 |

*(Values depend on time frame and latest market data.)*

---

## 🧾 Project Structure
```
portfolio-diversification-dashboard/
│
├── stock_portfolio_dashboard.ipynb   # Main notebook  
├── README.md                        # Project overview  
├── requirements.txt                 # Dependencies  
├── portfolio_metrics_summary.csv    # (optional saved results)  
└── wealth_curves.csv                # (optional saved results)  
```

---

## 🏁 How to Run
1. **Clone the repo**
   ```bash
   git clone https://github.com/lukejbbrown/stock-portfolio-dashboard.git  
   cd stock-portfolio-dashboard
   ```
2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the notebook**
   - Open `stock_portfolio_dashboard.ipynb` in VS Code or Jupyter  
   - Run cells sequentially  

---

## 💡 Why It’s Useful
This project showcases practical **quantitative-finance and data-analysis** skills:
- Financial data engineering  
- Portfolio risk and return modeling  
- Python-based visualization and optimization  
- Reproducible analysis pipeline  

Great for demonstrating applied data skills for finance, analytics, or data-science roles.

---

## 👨‍💻 Author
**Luke Brown**  
📫 https://www.linkedin.com/in/luke-jesse-brown-43b42828b
💼 [https://github.com/lukejbbrown](https://github.com/lukejbbrown)

---

⭐ **If you found this useful, give it a star on GitHub!**
