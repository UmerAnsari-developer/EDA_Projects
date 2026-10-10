# EDA Projects

Portfolio of Exploratory Data Analysis projects. Each project is a self-contained folder with a fully executed Jupyter notebook, its source dataset, and a detailed project readme.

These notebooks go beyond generic chart-making: every analysis follows a consistent professional structure — **data integrity → segmentation → hypothesis testing → executive summary → recommendations with quantified impact**.

---

## Projects

| Project | Dataset | Domain | Focus |
|---------|---------|--------|-------|
| [Customer Churn Analysis](Customer_Churn_Analysis/) | Telco churn — 7,043 customers, 21 features | Telecom | Churn drivers, at-risk segments, retention actions |
| [Netflix Shows Analysis](Netflix_Shows_Analysis/) | Netflix catalogue — 8,807 titles, 12 features | Streaming | Catalogue composition, genres, geography, content age |
| [Walmart Sales EDA](Walmart_EDA/) | Walmart transactions — 5,000 txns, 28 features | Retail | Store performance, promotion effectiveness, forecast accuracy |

---

## Highlights

### Customer Churn Analysis
- Overall churn rate **26.5%** — approximately **$1.5M** in annual revenue at risk
- Highest-risk segment: month-to-month contracts with electronic check (**45%+** churn)
- Critical churn window: first **6 months** of tenure (53% churn rate)
- Top actions quantified: contract migration, auto-pay adoption, fiber bundling

### Netflix Shows Analysis
- Catalogue is **70% movies** (6,126) vs 30% TV shows (2,664)
- Peak acquisition year **2019** (1,999 titles added)
- Top origin market: **United States** (2,809 titles)
- Selective data cleansing retains **99.8%** of rows (missingness reported before and after)

### Walmart Sales EDA
- Total revenue **15.26M** across 5,000 transactions (Jan–Sep 2024)
- **5 of 20 stores** fall in the bottom revenue quartile
- Promotion lift of +2.8% per transaction shown to be **statistically not significant** (Welch t-test, p = 0.21) — claims are tested, not assumed
- Forecast error **MAPE 59.9%**; stockout flags on 52% of transactions
- Closes with a stakeholder-style **recommendations memo** backed by four supporting exhibits

---

## Methodology

Every notebook follows the same analytical discipline:

1. **Data Ingestion & Integrity** — completeness profile before any cleansing; documented imputation/deletion policy
2. **Segmented Analysis** — business questions answered with confound-aware comparisons (per-transaction metrics, uplift vs baseline, normalised per-customer spend)
3. **Statistical Inference** — hypothesis tests (Welch t-test, one-way ANOVA) with effect sizes where group comparisons drive conclusions
4. **Executive Summary** — headline metrics regenerated dynamically from the data to prevent reporting drift
5. **Recommendations Memo** — findings → actions → estimated financial impact, written for stakeholder decision-making

---

## Tech Stack

- **Python** — pandas, numpy, matplotlib, seaborn, scipy
- **Jupyter Notebook** — all outputs pre-executed and embedded

---

## Getting Started

**Requirements**

```bash
pip install pandas numpy matplotlib seaborn scipy jupyter
```

**Run a notebook**

```bash
git clone https://github.com/UmerAnsari-developer/EDA_Projects.git
cd EDA_Projects
jupyter notebook <Project_Folder>/<notebook>.ipynb
```

| Folder | Notebook |
|--------|----------|
| `Customer_Churn_Analysis/` | `Customer_Churn_Analysis.ipynb` |
| `Netflix_Shows_Analysis/` | `shows_analysis.ipynb` |
| `Walmart_EDA/` | `EDA_Walmart.ipynb` |

---

## Repository Structure

```
EDA_Projects/
├── Customer_Churn_Analysis/
│   ├── Customer_Churn_Analysis.ipynb
│   ├── Telco_Customer_Churn_Dataset.csv
│   └── readme.md
├── Netflix_Shows_Analysis/
│   ├── shows_analysis.ipynb
│   ├── netflix_titles.csv
│   └── readme.md
├── Walmart_EDA/
│   ├── EDA_Walmart.ipynb
│   ├── Walmart.csv
│   ├── Bar_graph_plot_method.txt
│   └── readme.md
└── readme.md
```

---

## Author

**[UmerAnsari-developer](https://github.com/UmerAnsari-developer)** — data analysis portfolio
