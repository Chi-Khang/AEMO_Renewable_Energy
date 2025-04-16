# ⚡ Renewable Energy Integration & Electricity Pricing in Queensland (2019–2025)

This project investigates how **renewable energy integration** — especially **solar energy** — and **demand behavior** influence **electricity pricing** in Queensland, using data from the **National Electricity Market (NEM)** between **January 2019 and January 2025**.

---

## 🎯 Project Objective

- Quantifying the **impact of solar generation** on electricity prices.
- Understanding how **demand fluctuations** and **the integration fluctuations** contribute to **pricing volatility**.
- Exploring **seasonal**, **daily**, and **holiday patterns** in generation, demand and power generation.
- Building Dashboard for relationship and trend analysis.
- Building **statistical models** to analyze and predict price movements.

---

## 🧱 Data Sources

| Dataset                     | Description                                                |
|-----------------------------|------------------------------------------------------------|
| `DISPATCH_UNIT_SCADA`       | Actual generation data at the unit level (every 5 mins).   |
| `PERDEMAND`                 | Regional demand data at 5-min intervals.                   |
| `DISPATCHPRICE`             | Electricity price data (regional and dispatch-level).      |
| `NEM Registration`          | Info on registered market participants and generating units. |

---

## 🗂️ Notebooks Overview

| Notebook                                                                                     | Description                                                |
|----------------------------------------------------------------------------------------------|------------------------------------------------------------|
| `[1D_EDA]AllData_Processing_Exploration.ipynb`                                                | Load and preprocess raw NEM data.                          |
| `[2D_EDA]PowerGeneration_EnergySources_Analysis.ipynb`                                       | Explore renewable generation patterns over time.           |
| `[2D_EDA]Pricing&Demand_with_RenewableEnergySources_Integration_Analysis.ipynb`              | Correlate pricing with solar generation and demand.        |
| `[Modeling]Features_Engineering.ipynb`                                                       | Engineer temporal, demand, and solar-related features.     |
| `[Modeling]Models_Build.ipynb`                                                               | Develop models (GLM, Mixed Linear Models) to explain price dynamics. |
| `[Eval]ModelsEval_and_ResultsAnalysis.ipynb`                                                 | Analyze and validate model outputs.                        |
| `[Tableau_Dashboard]DateProcessing_for_Dashboards.ipynb`                                     | Prepare data for Tableau visual dashboards.                |
| `Common_Functions.ipynb`                                                                     | Shared utility functions used across notebooks.            |

---

## 🛠️ Tech Stack

- **Python**: `pandas`, `numpy`, `matplotlib`, `seaborn`, `plotly`, `statsmodels`, `sklearn`, `holidays`
- **Data Source**: NEM datasets (via CSV or SQLite)
- **Visualization**: Tableau & Plotly
- **Modeling**: GLM, Mixed Linear Models (MLM), time series analysis

---

## 📦 Setup

Install required Python packages:

```bash
pip install -r requirements.txt
