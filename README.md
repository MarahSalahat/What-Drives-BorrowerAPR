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
