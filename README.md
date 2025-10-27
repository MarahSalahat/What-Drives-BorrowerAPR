# 📊 Prosper Loan Data Analysis

### **by Marah Salahat**

---

## 🧠 Project Overview

This project explores and explains the factors that influence **BorrowerAPR (Annual Percentage Rate)** in the **Prosper Loan dataset**.  
The dataset contains detailed information about loans issued through Prosper Marketplace, including borrower characteristics, loan terms, and credit ratings.

The project is divided into two main parts:

- **Part I – Exploratory Data Analysis (EDA)**
- **Part II – Explanatory Data Analysis (Presentation)**

---

## 🎯 Project Goal

The primary goal is to understand **what drives BorrowerAPR differences** among borrowers.  
By analyzing borrower demographics, credit ratings, income levels, and loan details, we identify patterns and relationships that influence the rates offered to borrowers.

---

## 🧩 Dataset Overview

The dataset includes **113,937 loan records** and **81 variables** covering:
- Borrower financial attributes  
- Loan characteristics (amount, term, date, status)  
- Credit and risk ratings  
- Income and employment information  

Key variables analyzed:
- `BorrowerAPR` — Annual Percentage Rate (target variable)
- `CreditGrade` / `ProsperRating (Alpha)` — Borrower credit risk rating
- `IncomeRange` — Borrower’s income level
- `LoanOriginalAmount` — Size of the issued loan
- `Term` — Duration in months
- `LoanStatus` — Current loan condition (Completed, Current, Defaulted, etc.)

---

## ⚙️ Tools and Libraries Used

| Tool | Purpose |
|------|----------|
| **Python (Pandas, NumPy)** | Data cleaning, wrangling, and manipulation |
| **Matplotlib & Seaborn** | Data visualization |
| **Jupyter Notebook** | Documentation and presentation of findings |
| **Warnings & datetime** | Data preprocessing and quality control |

---

## 🧼 Data Cleaning Summary

Before analysis, the dataset was thoroughly cleaned to ensure accuracy:
- Converted date fields (`LoanOriginationDate`, `ClosedDate`) to datetime format.
- Filled missing categorical data (`CreditGrade`, `IncomeRange`, `BorrowerState`) with meaningful labels such as “Not Disclosed”.
- Merged `CreditGrade` and `ProsperRating (Alpha)` intelligently (since Prosper changed its grading system in 2009).
- Derived a new feature `LoanDurationDays` to represent the time between origination and closure.
- Handled outliers in `BorrowerAPR`, `StatedMonthlyIncome`, and `LoanOriginalAmount`.

---

## 🔍 Part I – Exploratory Data Analysis (EDA)

### Objectives
1. Explore relationships between BorrowerAPR and borrower attributes.
2. Identify which features most strongly correlate with interest rates.
3. Use visual analysis to support key observations.

### Analysis Summary
- **Univariate Analysis** – Examined distribution of key features (APR, loan amount, income range).
- **Bivariate Analysis** – Explored how BorrowerAPR changes with CreditGrade, Income, Term, etc.
- **Multivariate Analysis** – Combined multiple variables to identify interactions (e.g., CreditGrade × Income × APR).

### Key Findings
1. **Credit Grade** is the strongest predictor of BorrowerAPR.
2. **Higher Income** borrowers consistently receive lower APRs.
3. **Loan Amount and Term** slightly affect APR — smaller and shorter loans have higher rates.
4. **Active loans (no ClosedDate)** generally have moderate APRs.

---

## 📈 Part II – Explanatory Data Analysis (Presentation)

### Focus Question
> What drives BorrowerAPR differences among borrowers?

### Key Insights
1. Borrower **creditworthiness (CreditGrade)** has the greatest influence on BorrowerAPR.  
   Lower grades correspond to much higher interest rates.
2. Borrowers with **higher income ranges** tend to receive lower APRs, suggesting income stability affects lender confidence.
3. **Loan characteristics** (amount and term) play a minor role but still show predictable trends — shorter, smaller loans usually carry higher APRs.

### Featured Visualizations
1. **BorrowerAPR by Credit Grade** – Shows clear downward trend with improving credit grade.  
2. **BorrowerAPR by Income Range** – Demonstrates inverse relationship between income and APR.  
3. **BorrowerAPR vs Loan Amount (colored by Term)** – Illustrates how loan structure influences rate.

---

## 🧾 Files Included

| File | Description |
|------|--------------|
| `Part_I_Exploration.ipynb` | Full exploratory analysis with data cleaning, visualizations, and observations |
| `Part_II_Explanatory.ipynb` | Polished presentation with executive summary and final insights |
| `README.md` | Project documentation |
| `Prosper_Loan_Data.csv` *(if available)* | Source dataset |

---

## 🧮 Example Visuals

#### BorrowerAPR by Credit Grade
AA → Lowest APR
HR → Highest APR

#### BorrowerAPR by Income Range
Higher income → Lower APRs (inverse relationship)

#### BorrowerAPR vs Loan Amount
Smaller, short-term loans tend to have higher APRs.


---

## 🏁 Conclusion

The analysis concludes that **BorrowerAPR is primarily driven by borrower credit risk**, represented by credit grades and Prosper ratings.  
Income level and loan characteristics have secondary but consistent effects.  
These findings align with real-world financial principles of **risk-based pricing**, where lenders adjust interest rates based on borrower reliability and repayment ability.

---

## 💡 Future Improvements
- Use regression modeling to predict BorrowerAPR more accurately.
- Include time-based analysis (loan origination year vs. APR trend).
- Integrate external economic data (interest rate benchmarks) for deeper context.

---

## 🙋‍♀️ Author
**Marah Salahat**  
Data Science Enthusiast | Computer Systems Engineer  
Specializing in Data Analysis, Visualization, and Machine Learning  
📧 Contact: *marah.salahat2001@gmail.com*

---

*This project was developed as part of a Data Analysis portfolio to demonstrate professional data cleaning, exploration, and visualization practices.*
