# Netflix Shows Analysis

## Project Overview

Catalogue analysis of the Netflix titles dataset (8,807 movies & TV shows) covering composition, acquisition timeline, geographic distribution, ratings, genres, and duration profiles.

**Dataset:** `netflix_titles.csv` (8,807 titles, 12 features)

| File | Description |
|------|-------------|
| `shows_analysis.ipynb` | EDA notebook (22 cells, 7 analysis sections) |
| `netflix_titles.csv` | Source dataset |

---

## Key Findings

| Metric | Value |
|--------|-------|
| Titles Analysed | **8,790** after cleansing (0.2% removed) |
| Movies vs TV Shows | **6,126 vs 2,664** (70% movies) |
| Peak Acquisition Year | **2019** (1,999 titles added) |
| Top Origin Market | **United States** (2,809 titles) |
| Median Content Age | **1 year** at time of adding |
| Median Movie Runtime | **98 minutes** |

---

## Notebook Sections

1. Data Ingestion & Integrity (missingness profile before cleansing)
2. Catalogue Composition (movies vs TV shows)
3. Catalogue Evolution Over Time (acquisitions by year and type, content age)
4. Geographic Distribution (top 10 origin markets)
5. Content Ratings (top 10, horizontal bar)
6. Genre Composition (multi-label explode, stacked Movie vs TV)
7. Duration Profiles (runtime histogram, seasons distribution)
8. Executive Summary
9. Recommended Next-Phase Analyses

---

## Data Quality Approach

- Missingness reported **before** any cleansing
- `director` / `cast` / `country` imputed as "Unknown" (missingness is informative)
- Rows dropped only where `rating`, `duration`, or `date_added` are absent (0.2% of rows)
- Duplicate `show_id` check performed

---

## Tech Stack

- Python (pandas, numpy, matplotlib, seaborn)
- Jupyter Notebook

---

## Usage

```bash
jupyter notebook shows_analysis.ipynb
```
