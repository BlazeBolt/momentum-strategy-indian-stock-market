# 📈 Momentum Strategy on Indian Stock Market (BSE Sensex)

This project implements and backtests a momentum-based equity trading strategy on **BSE Sensex** stocks using **Python**, **yFinance**, and **SQL (SQLite)**. It demonstrates how real-time stock data can be transformed into actionable trading signals using historical price momentum and backtested using industry-standard techniques.

## 🚀 Overview

- 💹 Downloads real-time historical price data from Yahoo Finance (`yfinance`)  
- 🗃️ Stores time-series data in a **SQL (SQLite)** database  
- 📊 Calculates **rolling momentum** for each stock based on historical returns  
- 🔁 Selects the top N stocks by momentum and simulates **monthly rebalancing**  
- 📈 Tracks and visualizes **cumulative returns** of the momentum portfolio  

---

## 🧠 Strategy Logic

> **Momentum Trading Strategy**  
Select the top-performing stocks over a past window (formation period, e.g. 3 months), invest in them for a fixed holding period (e.g. 1 month), and repeat.

- **Formation Period:** 63 trading days (~3 months)  
- **Holding Period:** 21 trading days (~1 month)  
- **Rebalancing Frequency:** Monthly  
- **Stock Universe:** BSE Sensex sample tickers  

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| `Python` | Core programming language |
| `yfinance` | Downloading historical stock data |
| `SQLite` | Storing and querying price data |
| `pandas`, `numpy` | Data manipulation |
| `matplotlib` | Visualizing strategy returns |
| `SQLAlchemy` | SQL connection from Python |

---

## 📦 Requirements

Install the dependencies:

```bash
pip install yfinance pandas numpy matplotlib sqlalchemy
