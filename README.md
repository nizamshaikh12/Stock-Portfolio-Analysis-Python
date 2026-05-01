# Stock Portfolio Analysis & Data Manipulation — Python

**MSc Financial Technology — Programming for Financial Data Science**
*National College of Ireland, Dublin | Student ID: 24198170*

</div>

---

## Overview

This project demonstrates foundational Python programming skills applied to **real-world financial data**. It covers portfolio construction, risk-based valuation adjustments, multi-stock time series data manipulation and derived financial metrics using industry-standard libraries.

The notebook works with actual historical stock price data for **Apple (AAPL)**, **Microsoft (MSFT)**, **Netflix (NFLX)** and **Google (GOOG)** over a 3-month period (February–May 2023), covering 248 trading records across 8 price/volume fields.

---

## Objectives

- Construct and manipulate client portfolio dictionaries in Python
- Apply **risk-adjusted valuation logic** (high-risk vs low-risk asset discounts)
- Load, clean and transform real stock market CSV data using **Pandas**
- Standardise date formats and engineer new financial features
- Calculate **daily price change** (Close − Open) across all tickers
- Perform grouped multi-stock analysis and summary statistics

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

### Part 1 — Portfolio Construction & Risk Valuation
- Built a Python list of client portfolio dictionaries with fields: `Client_id`, `Asset_type`, `Value_usd`, `is_high_risk`
- Portfolios: **AAPL** ($254.43, high risk), **MSFT** ($509.23, high risk), **ETH** ($3,331.31, low risk)
- Applied conditional logic:
  - High-risk assets → **10% discount** applied (×0.90)
  - Low-risk assets → **5% discount** applied (×0.95)
- Output: recalculated portfolio values per client

### Part 2 — Stock Data Manipulation
- Loaded multi-stock CSV dataset using `pandas.read_csv()`
- Standardised date column from `DD/MM/YYYY` to `YYYY-MM-DD` using `pd.to_datetime()`
- Engineered `Daily_Change` column: `Close − Open` for each trading day
- Verified data shape, column types and null value checks
- Performed per-ticker filtering and grouped summary statistics

---

## Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Python 3** | Core programming language |
| **Pandas** | Data loading, cleaning, manipulation |
| **NumPy** | Numerical operations |
| **Jupyter Notebook** | Interactive development environment |
| **Microsoft Excel** | Initial data inspection & formatting |

---

## How to Run

1. Clone this repository or download the files
2. Open `Class-Assessment.ipynb` in **Jupyter Notebook** or **Google Colab**
3. Ensure `dataset.csv` is in the same folder as the notebook
4. Run all cells in order (Cell → Run All)

> **Requirements:** Python 3.x, pandas, numpy — install via `pip install pandas numpy`

---

## Author

**Mohd Nizam Nasir Shaikh**
