# MarketPulse — Analisi Comparativa Indici Azionari S&P 500 vs EURO STOXX 50

![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)
![Finance](https://img.shields.io/badge/Domain-Financial%20Analytics-green)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualisation-blue)

## Panoramica

Analisi comparativa della performance storica decennale di due indici azionari principali — **S&P 500** (mercato USA) e **EURO STOXX 50** (mercato europeo). Estrae insight su rendimenti, volatilità, stagionalità e eventi estremi. La logica core è incapsulata in un modulo Python; narrativa e grafici sono nel Jupyter Notebook.

Metodologie trasferibili a energy market analytics, risk management, financial reporting e qualsiasi contesto con dati di mercato time-series.

## Valore Enterprise

| Settore / Azienda | Rilevanza |
|-------------------|-----------|
| Energy (Enel, Terna) | Analisi price time-series applicabile a energy commodity |
| Banking & Insurance | Risk management, market performance reporting |
| IT Consulting (Accenture, NTT Data) | Financial analytics per clienti FSI |
| Data Reply | Python analytics pipeline su dati finanziari storici |

## Findings Principali

| Analisi | Risultato chiave |
|---------|-----------------|
| Performance decennale | S&P 500 outperforma EURO STOXX 50 su rendimento totale |
| Distribuzione rendimenti | Entrambi con skew negativo (drawdown > rally nella coda) |
| Giorni peggiori | Concentrati COVID-19 (marzo 2020) e shock rialzo tassi 2022 |
| Effetto giorno | Nessun effetto settimana statisticamente significativo ad alta frequenza |
| Volatilità estrema | I 5 giorni migliori seguono immediatamente i 5 peggiori — market timing impossibile |

## Analisi Condotte

| Analisi | Tecnica |
|---------|---------|
| Trend prezzi e volumi | Grafico storico normalizzato (base 100) |
| Distribuzione rendimenti | Istogramma + KDE — profilo di rischio e code |
| Performance mensile/annuale | Aggregazione periodi, heatmap stagionale |
| Effetto giorno della settimana | Media rendimento per weekday |
| Volatilità estrema | Top 5 best/worst trading days con contesto storico |

## Setup

```bash
git clone https://github.com/sylver86/13-performance-indici-azionari-python.git
cd 13-performance-indici-azionari-python
python -m venv venv && source venv/bin/activate
pip install -r requirements.txt
jupyter lab notebooks/main_analysis.ipynb
```

## Struttura Repository

```
13-performance-indici-azionari-python/
├── notebooks/
│   └── main_analysis.ipynb
├── data/
│   ├── sp500.csv
│   └── eurostoxx50.csv
├── src/
├── requirements.txt
└── README.md
```

## Stack Tecnologico

`Python 3.x` · `pandas` · `NumPy` · `Matplotlib` · `Seaborn` · `JupyterLab`

---

---

# MarketPulse — Comparative Analysis S&P 500 vs EURO STOXX 50 🇬🇧

![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)
![Finance](https://img.shields.io/badge/Domain-Financial%20Analytics-green)

## Overview

Comparative historical analysis of two major equity indices — **S&P 500** (US) and **EURO STOXX 50** (Europe) — over the last decade. Extracts insights on returns, volatility, seasonality, and extreme market events. Core logic in a Python module; analysis and charts in Jupyter Notebook.

## Key Findings

| Analysis | Key result |
|----------|-----------|
| 10-year performance | S&P 500 outperforms EURO STOXX 50 in total return |
| Returns distribution | Both show negative skew (drawdowns > rallies in tails) |
| Worst trading days | Concentrated around COVID-19 (March 2020) and 2022 rate shock |
| Weekday effect | No statistically significant weekday effect at daily frequency |
| Extreme volatility | Top 5 best days follow top 5 worst days — market timing is structurally impossible |

## Analyses

| Analysis | Technique |
|----------|-----------|
| Price & volume trends | Normalised historical chart (base 100) |
| Returns distribution | Histogram + KDE — risk profile and fat tails |
| Monthly / annual performance | Period aggregation, seasonal heatmap |
| Weekday effect | Average return per day of week |
| Extreme events | Top 5 best / worst trading days with historical context |

## Setup

```bash
git clone https://github.com/sylver86/13-performance-indici-azionari-python.git
cd 13-performance-indici-azionari-python
python -m venv venv && source venv/bin/activate
pip install -r requirements.txt
jupyter lab notebooks/main_analysis.ipynb
```

## Technologies

`Python 3.x` · `pandas` · `NumPy` · `Matplotlib` · `Seaborn` · `JupyterLab`
