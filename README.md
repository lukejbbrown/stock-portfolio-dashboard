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
- 100% Equity port
