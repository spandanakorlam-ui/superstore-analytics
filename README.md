# 🛒 Superstore Retail Analytics — Business Intelligence & Sales Performance Analysis

> **A full-stack data analytics project** | Python • Power BI • Jupyter • Machine Learning

[![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)](https://python.org)
[![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?logo=powerbi)](https://powerbi.microsoft.com)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green?logo=pandas)](https://pandas.pydata.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-lightgrey)](LICENSE)

---

## 📌 Project Overview

This project delivers a **comprehensive Business Intelligence analysis** of a U.S. retail superstore's transactional data — uncovering profit leakages, identifying growth opportunities, and translating raw data into **$123K–$192K in actionable annual profit improvement** recommendations.

| Metric | Value |
|--------|-------|
| 📦 Dataset | Sample Superstore — 9,994 records |
| 📅 Time Period | 2014 – 2017 (4 years) |
| 💰 Total Revenue Analysed | $2,297,201 |
| 📈 Overall Profit Margin | 12.47% |
| 🎯 Projected Margin After Fixes | 16–18% |
| 🗺️ Coverage | 49 US States, 4 Regions |
| 👥 Unique Customers | 793 |

---

## 🚨 The Problem

Despite $2.3M in revenue over 4 years, the business runs at only **12.47% profit margin** — well below the 20–25% retail industry benchmark. The analysis identifies five root causes:

1. **Uncontrolled discounting** — 856 orders at 50%+ discount destroying $76,559 in profit
2. **Loss-making Furniture sub-categories** — Tables alone: –$17,725 net loss
3. **Central region underperformance** — 7.92% margin vs. West's 14.94%
4. **State-level losses** — Texas: –$25,729 | Pennsylvania: –$15,560
5. **Consumer segment over-discounting** — Lowest margin (11.55%) despite highest revenue share (50.6%)

---

## 💡 Key Findings

### Category Performance
| Category | Sales | Profit | Margin |
|----------|-------|--------|--------|
| Technology | $836,154 | $145,455 | **17.40%** ✅ |
| Office Supplies | $719,047 | $122,491 | **17.04%** ✅ |
| Furniture | $741,999 | $18,451 | **2.49%** ⚠️ |

### Discount vs. Profit — Critical Finding
| Discount Tier | Orders | Avg Margin | Status |
|---------------|--------|------------|--------|
| 0% | 4,798 | **29.51%** | 🟢 Optimal |
| 1–20% | 3,803 | **~11–17%** | 🟡 Acceptable |
| 21–30% | 227 | **–10.05%** | 🔴 Loss |
| 50%+ | 856 | **–119.20%** | 🔴 Critical |

### Regional Breakdown
| Region | Sales | Profit | Margin |
|--------|-------|--------|--------|
| West | $725,458 | $108,418 | 14.94% 🥇 |
| East | $678,781 | $91,523 | 13.48% 🥈 |
| South | $391,722 | $46,749 | 11.93% |
| Central | $501,240 | $39,706 | 7.92% ⚠️ |

---

## 🎯 Business Recommendations

| # | Recommendation | Priority | Est. Annual Impact |
|---|---------------|----------|--------------------|
| 1 | Cap discounts at 20% — CFO approval above | 🔴 CRITICAL | $50K–$80K |
| 2 | Restructure Furniture (exit Tables, grow Chairs) | 🔴 HIGH | $25K–$40K |
| 3 | Fix Central region & Texas/Pennsylvania losses | 🟡 HIGH | $20K–$35K |
| 4 | Double down on Technology (Copiers 37.2% margin) | 🟡 MEDIUM | $18K–$22K |
| 5 | Differentiated customer segment strategy | 🟢 MEDIUM | $10K–$15K |
| | **TOTAL PROJECTED IMPACT** | | **$123K–$192K/yr** |

---

## 🏗️ Project Structure

```
superstore-analytics/
│
├── 📊 Data
│   └── cleaned_superstore.csv          # Cleaned dataset (9,994 rows × 24 cols)
│
├── 📓 Analysis
│   └── Store_Analysis_notebook.ipynb   # Full EDA + ML + visualisations
│
├── 📊 Dashboard
│   └── Superstore_BI.pbix              # Interactive Power BI report (6 pages)
│
├── 📄 Documentation
│   ├── Full_Project_Report.docx        # 30+ page comprehensive report
│   ├── Problem_Statement.docx          # Formal problem definition
│   └── Superstore_Presentation.pptx   # 10-slide executive deck
│
└── README.md                           # This file
```

---

## 🛠️ Tech Stack

```
Language    : Python 3.x
Libraries   : Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
BI Tool     : Power BI Desktop
Notebook    : Jupyter
Data Format : CSV (cleaned), .pbix (dashboard)
```

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/[your-username]/superstore-analytics.git
cd superstore-analytics
```

### 2. Install Dependencies
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 3. Run the Analysis Notebook
```bash
jupyter notebook Store_Analysis_notebook.ipynb
```

### 4. Open Power BI Dashboard
1. Download and install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
2. Open `Superstore_BI.pbix`
3. On the `Home` ribbon → `Transform Data` → update the CSV file path to your local `cleaned_superstore.csv`
4. Click `Refresh` — all visuals update automatically

---

## 📊 Power BI Dashboard Pages

| Page | Content |
|------|---------|
| Executive Overview | KPI cards — Revenue, Profit, Margin, Orders (with YoY) |
| Category Deep Dive | Sub-category profit waterfall, margin heatmap |
| Regional Analysis | US state-level filled map, regional comparison |
| Customer Segmentation | Segment profitability scatter plot, RFM overview |
| Discount Analysis | Discount vs. profit scatter with trend line |
| Sales Trend | Monthly sales line chart with year-over-year overlay |

> **Interactive slicers**: Year · Region · Category · Segment
> **Conditional formatting**: Loss-making rows highlighted in red automatically

---

## 📈 Analysis Methodology (CRISP-DM)

```
1. Business Understanding   → Define problem, KPIs, success metrics
2. Data Understanding       → EDA, distributions, correlations, outlier detection
3. Data Preparation         → Cleaning, type conversion, feature engineering
4. Modelling                → Statistical analysis, regression, time-series forecasting
5. Evaluation               → Validate findings against business questions
6. Deployment               → Power BI dashboard + report + recommendations
```

---

## 🔍 Notebook Contents

The Jupyter notebook (`Store_Analysis_notebook.ipynb`) covers:

- [x] Data loading, schema inspection, and quality checks
- [x] Univariate & bivariate distribution analysis
- [x] Category and sub-category profitability deep dive
- [x] Regional and state-level performance mapping
- [x] Discount rate vs. profit regression analysis
- [x] Customer segment RFM scoring
- [x] Year-on-year and seasonal trend analysis
- [x] Sales forecasting model (time series)
- [x] Feature importance analysis

---

## 🏆 Key Skills Demonstrated

`Exploratory Data Analysis` · `Business Intelligence` · `Data Visualisation` · `Power BI` · `Python` · `Pandas` · `Statistical Analysis` · `Machine Learning` · `Time Series Forecasting` · `Executive Communication` · `Retail Analytics` · `CRISP-DM`

## 📊 Dashboard Preview

### Executive Overview
![Dashboard 1](dashboard1.png)

### Category Analysis
![Dashboard 2](dashboard2.png)

### Regional Analysis
![Dashboard 3](dashboard3.png)

---

## 📬 Contact

**[Spandana Korlam]**
- 🔗 LinkedIn: linkedin.com/in/spandana-korlam-aa532420a
- 💼 Portfolio: https://github.com/spandanakorlam-ui
- 📧 Email: spandanakorlam@gmail.com

---

## 📄 License

This project is for educational and portfolio purposes. The Superstore dataset is publicly available via Tableau Public and Kaggle.

---

> ⭐ If this project helped you, consider giving it a star — it helps others find it!
