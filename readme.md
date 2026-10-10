# EDA Projects

Exploratory Data Analysis projects with business insights and Power BI dashboards.

---

## Projects

### 1. Customer Churn Analysis (Telecom)

**Dataset:** Telco Customer Churn (7,043 customers, 21 features)

**Objective:** Analyze customer churn drivers and provide actionable retention strategies.

| File | Description |
|------|-------------|
| `Customer_Churn_Analysis.ipynb` | Full EDA notebook with 8 business questions & answers |
| `Telco_Customer_Churn_Dataset.csv` | Source dataset (7,043 rows) |

#### Key Findings

| Finding | Value |
|---------|-------|
| Overall Churn Rate | **26.5%** (1,869 of 7,043) |
| Annual Revenue at Risk | **~$1.5M** |
| Highest Risk Segment | Month-to-month + Electronic check (45%+ churn) |
| Critical Churn Window | First 6 months (53% churn rate) |
| Contract Impact | Month-to-month 42.7% vs Two-year 2.8% |
| Payment Method | Electronic check 45.3% vs Auto-pay 15-17% |
| Internet Service | Fiber optic 41.9% vs DSL 19.0% |

#### EDA Sections

1. **Data Loading & Cleaning** — Missing TotalCharges imputed (11 new customers)
2. **Customer Demographics** — Gender, Senior, Partner, Dependents analysis
3. **Tenure Analysis** — Distribution, survival curve, tenure groups
4. **Service Usage** — 9 service features vs churn
5. **Contract & Billing** — Key churn drivers (Contract, Payment, Paperless)
6. **Charges Analysis** — Monthly/Total charges vs churn
7. **Correlation Heatmap** — Feature correlations with churn
8. **Cohort Analysis** — Tenure × Contract churn matrix

#### Business Questions Answered

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

#### Recommended Actions

1. **Contract Migration** — Incentivize M2M → annual (10-15% discount)
2. **Auto-Pay Conversion** — Push e-check to auto-pay ($5/mo incentive)
3. **Fiber Value Bundle** — Bundle security add-ons with fiber plans
4. **New Customer Onboarding** — 90-day engagement program for 0-6 month customers

---

## Tech Stack

- Python (pandas, numpy, matplotlib, seaborn)
- Jupyter Notebook
- Power BI (dashboard companion in `guide.md`)

---

## Usage

```bash
# Clone the repo
git clone https://github.com/UmerAnsari-developer/EDA_Projects.git

# Open notebook in Jupyter
jupyter notebook Customer_Churn_Analysis.ipynb
```

---

## Author

**Umer Ansari** — [GitHub](https://github.com/UmerAnsari-developer)
