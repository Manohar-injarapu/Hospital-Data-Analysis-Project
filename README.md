# Hospital-Data-Analysis-Project
Performed end-to-end hospital data analysis including data cleaning, feature engineering, EDA, statistical testing, and executive-level visualization to identify cost drivers, readmission risks, and operational inefficiencies


## Overview
This project focuses on **data ingestion, cleaning, transformation, feature engineering, and exploratory analysis** of a hospital dataset to enable reliable modeling and insightful decision-making.  
The workflow ensures data quality, consistency, and integrity at each stage — from raw ingestion to final analytics and reporting.

---

## 🔹 Data Ingestion & Validation
- Loaded hospital CSV dataset.
- Created raw and working copies of data for reproducibility.
- Inspected dataset shape and schema.
- Verified data types and memory usage.
- Checked for missing values and duplicate records.

---

## 🔹 Column Standardization
- Cleaned column names by trimming whitespace and converting to lowercase.
- Converted all names to `snake_case`.
- Removed special characters from field names.
- Ensured naming consistency across datasets.

---

## 🔹 Identifier Cleaning
- Identified and removed duplicate patient IDs.
- Removed duplicate patient encounter records.
- Validated uniqueness of encounters and IDs.

---

## 🔹 Age Data Cleaning
- Converted the **age** column to numeric type.
- Removed invalid or negative age values.
- Handled outliers (ages > 120) using IQR-based methods.
- Imputed missing age values.
- Validated medical plausibility of all age entries.

---

## 🔹 Gender Standardization
- Normalized gender values (e.g., 'M', 'F', 'Male', 'Female').
- Corrected typos and inconsistent labels.
- Handled missing or unknown gender categories.
- Validated gender distribution post-cleaning.

---

## 🔹 Categorical Data Cleaning
- Cleaned and standardized **condition**, **procedure**, and **outcome** names.
- Standardized **readmission status** and **patient satisfaction ratings**.
- Removed extra whitespace, special symbols, and inconsistent text formats.
- Applied **mode-based imputation** to fill missing categorical entries.
- Validated frequency distribution of each categorical variable.

---

## 🔹 Numeric Data Cleaning
- Converted **cost** column to numeric type.
- Removed negative or invalid cost entries.
- Detected and capped cost outliers.
- Validated **length of stay** calculations.
- Treated length-of-stay outliers via statistical thresholds.

---

## 🔹 Feature Engineering
- Created binary encodings for:
  - Readmission status
  - Patient outcome
  - Gender
- Created custom features:
  - Age group bins (e.g., child, adult, senior)
  - Cost tier categories (low, medium, high)
  - Length-of-stay categories
  - Cost per day metric
- Validated all derived features for logical accuracy.

---

## 🔹 Modeling Preparation
- Checked multicollinearity among features using correlation analysis.
- Handled skewed distributions with transformations.
- Selected modeling-ready feature set.
- Scaled numerical features as needed.
- Implemented safeguards against data leakage.
- Exported the final cleaned dataset for model training.

---

## 🔹 Exploratory Data Analysis (EDA)
- Performed univariate and bivariate analysis.
- Visualized age, cost, and length-of-stay distributions.
- Compared cost across demographics and conditions.
- Analyzed readmission risk patterns.
- Identified high-cost or high-risk patient segments.
- Summarized key operational and efficiency insights.

---

## 🔹 Statistical Analysis
- Conducted **t-tests** for cost differences between groups.
- Performed **chi-square tests** for categorical outcome associations.
- Validated assumptions of normality and independence.
- Interpreted hypothesis testing results with business relevance.

---

## 🔹 Data Visualization
- Created a comprehensive visualization suite:
  - Histograms, bar charts
  - Box and violin plots
  - Scatter plots and pair plots
- Designed executive-level visual summaries.

---
