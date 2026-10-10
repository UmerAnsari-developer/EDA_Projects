# Customer Churn Analysis (Telecom)

## Project Overview

Analysis of customer churn in a telecommunications company to identify at-risk customers and develop predictive insights for retention.

**Dataset:** Telco Customer Churn (7,043 customers, 21 features)

| File | Description |
|------|-------------|
| `Customer_Churn_Analysis.ipynb` | Full EDA notebook with 8 business Q&A |
| `Telco_Customer_Churn_Dataset.csv` | Source dataset |

---

## Key Findings

| Metric | Value |
|--------|-------|
| Overall Churn Rate | **26.5%** (1,869 of 7,043) |
| Annual Revenue at Risk | **~$1.5M** |
| Highest Risk Segment | Month-to-month + Electronic check (45%+ churn) |
| Critical Churn Window | First 6 months (53% churn rate) |
| Contract Impact | M2M 42.7% vs Two-year 2.8% |
| Payment Method | Electronic check 45.3% vs Auto-pay 15-17% |
| Internet Service | Fiber optic 41.9% vs DSL 19.0% |

---

## EDA Sections

1. Data Loading & Cleaning
2. Customer Demographics Analysis
3. Customer Tenure Analysis
4. Service Usage Analysis
5. Contract & Billing Analysis
6. Charges Analysis
7. Correlation Heatmap
8. Key Driver Analysis
9. Cohort Analysis
10. Business Questions & Answers (BQ1-BQ8)

---

## Business Questions Answered

| # | Question | Answer |
|---|----------|--------|
| BQ1 | Overall churn rate & financial impact? | 26.5%, ~$1.5M/year at risk |
| BQ2 | Highest risk segments? | M2M + Electronic check (45%+) |
| BQ3 | Critical churn window? | First 6 months (53% churn) |
| BQ4 | Contract type impact? | M2M 42.7% vs Two-year 2.8% |
| BQ5 | Do add-ons reduce churn? | Yes, 5-15pp reduction each |
| BQ6 | Pricing effect? | Churned pay ~$13/mo more |
| BQ7 | High-risk profile? | ~400 customers at 67% churn |
| BQ8 | Top 3 actions? | Contract migration + Auto-pay + Fiber bundle |

---

## Tech Stack

- Python (pandas, numpy, matplotlib, seaborn)
- Jupyter Notebook

---

## Usage

```bash
jupyter notebook Customer_Churn_Analysis.ipynb
```
