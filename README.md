# Prosper Loan Data Analysis: What Drives Borrower APR?

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-1.5%2B-green)
![Seaborn](https://img.shields.io/badge/Seaborn-0.12%2B-orange)
![Udacity](https://img.shields.io/badge/Udacity-Data%20Analyst%20Nanodegree-success)

---

## Project Overview

This project is part of the **Udacity Data Analyst Nanodegree** and explores the **Prosper Loan Dataset** — a rich collection of peer-to-peer loan data from Prosper Marketplace. The goal is to **uncover the key factors influencing Borrower APR (Annual Percentage Rate)** and present actionable insights for lenders, borrowers, and platform operators.

Through **systematic Exploratory Data Analysis (EDA)** and a **polished Explanatory Analysis**, we answer:

> **What drives interest rates in P2P lending?**  
> How do credit risk, income, loan size, and term structure affect pricing?

---

## Key Findings

| Factor | Impact on Borrower APR |
|-------|------------------------|
| **Credit Grade / Prosper Rating** | **Strongest driver** — HR-rated borrowers pay ~2.5x more than AA |
| **Income Range** | Higher income → lower APR (up to 8% difference) |
| **Loan Amount** | Smaller loans (<$5K) → higher APR (fixed costs + risk) |
| **Loan Term** | 60-month loans slightly cheaper than 36-month for same amount |
| **Loan Status** | Charged-off loans had higher original APRs |

> **Insight**: Prosper uses **risk-based pricing**, where creditworthiness dominates, but loan structure plays a supporting role.

---

## Project Structure
prosper-loan-analysis/
│
├── Part_I_Exploration.ipynb          # Full EDA: Univariate, Bivariate, Multivariate
├── Part_II_Explanatory.ipynb         # Executive summary with polished visuals
│
├── data/
│   └── prosperLoanData.csv           # Original dataset (not pushed due to size)
│
├── images/                           # Exported plots (optional)
│
├── Part_I_exploration_template.html  # Exported EDA notebook (HTML)
├── Part_II_explanatory_template.html # Exported explanatory notebook (HTML)
│
├── requirements.txt                  # Python dependencies
└── README.md                         # You're here!


## Exploratory Data Analysis (Part I)

### Visualizations Included
| Type | Count |
|------|-------|
| **Univariate** | Histogram (APR), Count Plot (Credit Grade) |
| **Bivariate** | Scatterplot (Loan vs APR), Box Plot (APR by Grade), Bar Chart, Clustered Count Plot, Heatmap |
| **Multivariate** | Facet Grid, Plot Matrix, Encoded Scatter (color + size), Clustered Bar Chart |

> All visualizations include **clear titles, labels, annotations**, and **appropriate scales**.

### Framework: *Question → Visualization → Observation*
Example:

**Q**: How does credit grade affect APR?  
**V**: Box plot of BorrowerAPR by ProsperRating  
**O**: Median APR drops from 32% (HR) to 7% (AA) — clear risk pricing.

Explanatory Analysis (Part II)
A separate, presentation-ready notebook designed for stakeholders.

Overarching Question: What are the primary drivers of Borrower APR?
Context: Prosper’s P2P lending model, dataset overview
Polished Visuals: Reused and refined from EDA
Key Insights: Summarized with business implications
Conclusion: Risk-based pricing is effective; small loans remain costly
