# Walmart Sales EDA

## Project Overview

Transaction-level analysis of Walmart sales (20 stores, 8 products, Jan–Sep 2024) covering store performance, promotion effectiveness, demand drivers, and forecast accuracy — closed with statistical inference and a stakeholder recommendations memo.

**Dataset:** `Walmart.csv` (5,000 transactions, 28 features)

| File | Description |
|------|-------------|
| `EDA_Walmart.ipynb` | Full EDA notebook (44 cells, 13 business questions) |
| `Walmart.csv` | Source dataset |
| `Bar_graph_plot_method.txt` | Plotting reference notes |

---

## Key Findings

| Metric | Value |
|--------|-------|
| Total Revenue | **15.26M** across 5,000 transactions |
| Bottom-Quartile Stores | **5** of 20 (stores 6, 4, 12, 18, 7) |
| Promotion Lift per Txn | +2.8% — **not significant** (Welch t-test, p = 0.21) |
| Weather Effect | **Not significant** (ANOVA, p = 0.10) |
| Stockout-Flagged Txns | **51.9%** of all transactions |
| Forecast Error (MAPE) | **59.9%** overall |
| Best-Selling Product | Fridge |
| Holiday Uplift Leader | Electronics (+0.4%) |

---

## Notebook Sections

1. Data Ingestion & Integrity
2. Sales Overview (volume, revenue, category pricing)
3. Store Performance Diagnostics (bottom-quartile rule)
4. Promotion Performance (reach + lift with significance test)
5. Demand Driver Analysis (holiday uplift, weather, loyalty)
6. Temporal Analysis (monthly trend, day-of-week)
7. Extended Diagnostics (stockout exposure, forecast MAPE, payment mix)
8. Statistical Inference (Welch t-test, one-way ANOVA)
9. Executive Summary
10. Recommendations Memo + Supporting Exhibits (4-panel figure)
11. Recommended Next-Phase Analyses

---

## Business Questions Answered

| # | Question | Answer |
|---|----------|--------|
| Q1 | Total sales volume & revenue? | 15.26M revenue, 5,000 txns |
| Q2 | Highest-priced categories? | Category-level avg unit price |
| Q3 | Underperforming stores? | 5 stores, bottom revenue quartile |
| Q4 | Promotion reach? | Share of promo-flagged txns |
| Q5 | Promo effectiveness? | +2.8% lift — statistically not significant |
| Q6 | Holiday demand uplift? | Electronics leads (+0.4%) |
| Q7 | Weather vs transaction value? | Gap not significant (p = 0.10) |
| Q8 | Loyalty tier spend? | Revenue per customer by tier |
| Q9 | Monthly revenue trend? | Chronologically ordered seasonality |
| Q10 | Best-selling products? | Fridge leads by volume |
| Q11 | Stockout exposure? | 52% flagged txns; order-level data needed |
| Q12 | Forecast accuracy? | MAPE 59.9% — needs rebuild |
| Q13 | Payment mix? | Revenue share by payment method |

---

## Tech Stack

- Python (pandas, numpy, matplotlib, seaborn, scipy)
- Jupyter Notebook

---

## Usage

```bash
jupyter notebook EDA_Walmart.ipynb
```
