# 📊 Excelerate Internship Project – SLU Opportunity Data Analysis

This repository contains the code and analysis I completed during my internship at **Excelerate**, focused on cleaning, transforming, and enriching a real-world dataset related to student opportunities. The internship encompassed of 4 weeks where each week a data oriented task was performed.

## 📁 Project Overview

The notebook demonstrates the **end-to-end data processing pipeline** applied to the **Saint Louis University Opportunity Wise dataset**, including:

## 🚀 Key Tasks Completed

### ✅ Data Cleaning
- Filled missing values in fields like `Institution Name` and `Apply Date`
- Coerced invalid date formats into `NaT` safely
- Standardized formats for:
  - Gender (`M`, `F`, `female` → `Male`, `Female`, etc.)
  - Strings (title case, stripped spaces)
  - Institutions (e.g., “St. Louis” → “Saint Louis”)

### ✅ Feature Engineering
- **Age** (calculated from `Date of Birth`)
- **Engagement Duration** = `Apply Date` − `Opportunity Start Date`
- **Time in Opportunity** = `Opportunity End Date` − `Opportunity Start Date`
- **Signup Month** and **Signup Year** (extracted from datetime)
- **Gender Binary Encoding**: `Male` = 1, `Female` = 0, `Other` = -1
- **MinMax Normalization** of numerical features

### ✅ Exploratory Data Analysis (EDA)
- Visualized distribution of key features such as age, engagement duration, and signup trends.
- Analyzed time-based patterns (e.g., signups by month/year).
- Identified correlations between user demographics and application timing.
- Detected outliers and inconsistencies using box plots and scatter plots.
- Assessed class imbalance and data quality for predictive readiness.
  
### ✅ Predictive Modeling

- Built supervised learning models to predict user drop-off or completion.
- Trained models using logistic regression and evaluated with precision, recall, F1-score, and AUC.
- Handled imbalanced data using stratified sampling and/or class weights.
- Performed feature selection and importance ranking using model coefficients.
- Validated model performance using cross-validation and confusion matrix.

### ✅ Recommendation System 

- Designed a simple rule-based recommendation system to suggest relevant opportunities to users based on their demographics and engagement patterns.
- Clustered users with similar behaviors using KMeans (optional: or used collaborative filtering if applicable).
- Created matching logic between student profiles and opportunity characteristics.
- Evaluated system precision by comparing historical outcomes and suggested matches.


## 🧰 Tech Stack

- **Python**
- **Jupyter Notebook**
- **Pandas**
- **NumPy**
- **scikit-learn** (for preprocessing)

---

## 📂 Files in This Repository

| File Name                             | Description                                      |
|--------------------------------------|--------------------------------------------------|
| `excelerate internship codfile.ipynb` | Main notebook with full data cleaning and feature engineering , ML mddel training and testing and building a simple recommendation system. |
| `README.md`                          | Project overview and documentation (this file)   |

---



## Acknowledgements

This work was completed as part of my internship at **Excelerate**, under guidance from the data team. Special thanks to the project mentors for their support.



