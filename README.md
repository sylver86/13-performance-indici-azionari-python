# Stock Market Index Analysis — S&P 500 vs EURO STOXX 50

![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualisation-blue)
![Finance](https://img.shields.io/badge/Domain-Financial%20Analysis-green)

## Overview

Comparative analysis of the historical performance of two major equity indices over the last decade: **S&P 500** (US market) and **EURO STOXX 50** (European market).

Extracts actionable insights on returns, volatility, seasonality, and extreme market events. Core logic is encapsulated in a Python module; analysis narrative and charts are in a Jupyter Notebook.

---

## Key Analyses

| Analysis | What it answers |
|----------|----------------|
| Historical price & volume trends | Long-term trajectory and market regime changes |
| Daily returns distribution | Volatility profile and fat-tail risk |
| Monthly & annual performance | Seasonal patterns and year-over-year comparison |
| Weekday effect | Average return by day of week (Monday effect, etc.) |
| Top 5 best / worst trading days | Extreme market events and their context |

---

## Key Findings (from notebook)

- S&P 500 delivered stronger long-term total returns over the decade compared to EURO STOXX 50
- Both indices show negative skew in daily returns distribution (larger drawdowns than rallies)
- Worst trading days cluster around COVID-19 (March 2020) and 2022 rate-hike shock
- Best trading days immediately follow worst days — timing the market is structurally impossible
- No statistically significant weekday effect in either index at daily resolution

Full charts and per-year breakdowns available in `main_analysis.ipynb`.

---

## Setup

```bash
git clone https://github.com/sylver86/13-performance-indici-azionari-python.git
cd 13-performance-indici-azionari-python

python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

pip install -r requirements.txt
jupyter lab
```

Open `notebooks/main_analysis.ipynb` to run the full analysis.

---

## Data Source

Raw CSV files for S&P 500 and EURO STOXX 50 included in the `data/` directory (sourced from public financial data collections).

---

## Project Structure

```
13-performance-indici-azionari-python/
├── notebooks/
│   └── main_analysis.ipynb   # Full analysis and visualisations
├── data/
│   ├── sp500.csv
│   └── eurostoxx50.csv
├── requirements.txt
└── README.md
```

---

## Technologies

`Python 3.x` · `pandas` · `NumPy` · `Matplotlib` · `Seaborn` · `JupyterLab`
