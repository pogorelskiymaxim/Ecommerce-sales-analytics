# E-Commerce Sales Analytics

**Tools:** Python (Pandas, NumPy, Matplotlib, Seaborn, SciPy) · Google BigQuery · Tableau  
**Period analyzed:** Nov 2020 – Jan 2021

---

## Overview

End-to-end analysis of an e-commerce furniture store: 349,545 sessions, 33,538 purchases, $31.97M total revenue across 100+ countries.

Data was pulled from Google BigQuery, analyzed in Python, and visualized in an interactive Tableau dashboard.

---

## Key Metrics

| Metric | Value |
|---|---|
| Total Revenue | $31,971,731 |
| Total Sessions | 349,545 |
| Total Purchases | 33,538 |
| Conversion Rate | 9.6% |
| Average Order Value | $953 |

---

## What's Inside

The notebook covers a full analytics pipeline:

1. **Data extraction** — SQL query via BigQuery, JOIN across sessions, purchases, and user account tables
2. **EDA** — data types, nulls, duplicates, date range, session counts
3. **Data cleaning** — user type classification (Registered vs Guest), revenue calculation, feature engineering
4. **Business insights** — geography, product categories, device types, traffic channels, email engagement
5. **Sales dynamics** — daily trends, 7-day rolling average, breakdown by continent, channel, device
6. **Pivot tables** — Sessions by Channel × Device; Revenue by Category × Country; AOV by Device × Channel
7. **Correlation analysis** — Pearson r between sessions and revenue (r ≈ 0.85+), cross-continent and cross-channel correlations
8. **Statistical tests** — Mann-Whitney U, Kruskal-Wallis, Z-test, Chi-Square
9. **Tableau export** — enriched CSV with date dimensions and readable labels

---

## Key Findings

- **Americas** accounts for 55% of revenue ($17.7M), led by the US ($13.9M, 44% of total)
- **Organic Search** is the top traffic channel; **Desktop** drives the majority of purchases
- **Registered users** (8% of sessions) generate disproportionately higher revenue than guests — statistically confirmed (Mann-Whitney U, p < 0.001)
- **Sessions and revenue are strongly correlated** (Pearson r ≈ 0.85+, p < 0.001) — organic traffic growth directly predicts revenue growth
- **Device and traffic channel are statistically associated** (Chi-Square, p < 0.001)

---

## Files

| File | Description |
|---|---|
| `E-commerce Sales Analytics.ipynb` | Main analysis notebook |
| `ecommerce_tableau_final.csv` | Cleaned and enriched dataset for Tableau |

---

## Tableau Dashboard

[View interactive dashboard →](https://public.tableau.com/app/profile/maxim.pogorelskiy/vizzes)

---

## Contact

**Maxim Pogorelskiy** · [LinkedIn](http://www.linkedin.com/in/blizzardheart) · pogorelskiymaxim@gmail.com
