# Stock Portfolio Analysis & Data Manipulation — Python

**MSc Financial Technology — Programming for Financial Data Science**
*National College of Ireland, Dublin | Student ID: 24198170*

---

## Overview

This repository contains a collection of Jupyter notebooks covering foundational Python programming skills applied to **real-world financial and stock market data**. The work spans portfolio construction, risk-based valuation logic, control flow for trading decisions, stock data manipulation and portfolio performance visualisation using NumPy and Matplotlib.

Stocks covered across the notebooks include **Apple (AAPL)**, **Microsoft (MSFT)**, **Netflix (NFLX)**, **Google (GOOG)**, **Tesla (TSLA)**, **Amazon (AMZN)**, **NVIDIA (NVDA)**, **Intel (INTC)**, **Meta (META)**, **Adobe (ADBE)** and **Salesforce (CRM)**.

---

## Objectives

- Construct and manipulate client portfolio dictionaries in Python
- Apply **risk-adjusted valuation logic** (high-risk vs low-risk asset discounts)
- Use conditional logic (if/elif/else) and loops (for/while) for trading decisions
- Load, clean and transform real stock market CSV data using **Pandas**
- Standardise date formats and engineer new financial features
- Calculate **daily price change** (Close − Open) across all tickers
- Compute **portfolio performance metrics** including weighted returns and volatility
- Visualise portfolio data using bar charts, scatter plots and pie charts with **Matplotlib**

---

## Dataset

| Column | Description |
|--------|-------------|
| `Ticker` | Stock symbol (AAPL, MSFT, NFLX, GOOG) |
| `Date` | Trading date (reformatted to YYYY-MM-DD) |
| `Open` | Opening price (USD) |
| `High` | Intraday high price (USD) |
| `Low` | Intraday low price (USD) |
| `Close` | Closing price (USD) |
| `Adj Close` | Dividend/split-adjusted closing price |
| `Volume` | Number of shares traded |
| `Daily_Change` | Engineered feature: Close − Open |

**Period:** 07 Feb 2023 – 05 May 2023 | **Records:** 248 rows × 9 columns

---

## Key Tasks Completed

### Class Assessment — Portfolio Construction & Stock Data Manipulation
- Built a Python list of client portfolio dictionaries with fields: `Client_id`, `Asset_type`, `Value_usd`, `is_high_risk`
- Portfolios: **AAPL** ($254.43, high risk), **MSFT** ($509.23, high risk), **ETH** ($3,331.31, low risk)
- Applied conditional logic:
  - High-risk assets → **10% discount** applied (×0.90)
  - Low-risk assets → **5% discount** applied (×0.95)
- Loaded multi-stock CSV dataset using `pandas.read_csv()`
- Standardised date column from `DD/MM/YYYY` to `YYYY-MM-DD` using `pd.to_datetime()`
- Engineered `Daily_Change` column: `Close − Open` for each trading day
- Performed per-ticker filtering and grouped summary statistics

### Assignment 1 — Python Basics for Stock Trading Logic
- Created a stock price dictionary for 7 tickers: AAPL, GOOG, MSFT, NVDA, TSLA, INTC, META
- Applied **if/elif/else** logic to classify stock as overvalued, stable or a bargain based on price threshold
- Used a **for loop** to iterate through all tickers and print their current prices
- Implemented a **while loop** to simulate NVDA price incrementing by $5 until reaching a target of $250
- Demonstrated core Python control flow concepts in a financial context

### Lab 7 — Portfolio Performance Visualisation
- Defined a 10-stock portfolio: MSFT, GOOG, TSLA, AMZN, NVDA, NFLX, DIS, PYPL, ADBE, CRM
- Used **NumPy arrays** for annual returns (ranging from −10% to +50%) and volatility values
- Defined investment allocation weights across all 10 tickers totalling 100%
- Computed **weighted portfolio return** and **weighted portfolio volatility**
- Created a **bar chart** of annual returns per stock
- Created a **scatter plot** of volatility vs return for risk-return analysis
- Created a **pie chart** of portfolio allocation weights with MSFT slice exploded for emphasis

---

## Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Python 3** | Core programming language |
| **Pandas** | Data loading, cleaning, manipulation |
| **NumPy** | Numerical operations and array-based portfolio calculations |
| **Matplotlib** | Data visualisation — bar, scatter and pie charts |
| **Jupyter Notebook** | Interactive development environment |
| **Microsoft Excel** | Initial data inspection & formatting |

---

## How to Run

1. Clone this repository or download the files
2. Open any `.ipynb` file in **Jupyter Notebook** or **Google Colab**
3. For `Class-Assessment.ipynb`, ensure `dataset.csv` is in the same folder
4. Run all cells in order (Cell → Run All)

> **Requirements:** Python 3.x, pandas, numpy, matplotlib — install via `pip install pandas numpy matplotlib`

---

## Author

**Mohd Nizam Nasir Shaikh**

MSc Financial Technology — National College of Ireland, Dublin

LinkedIn: https://www.linkedin.com/in/nizam-shaikh-90b737199

GitHub: https://github.com/nizamshaikh12
