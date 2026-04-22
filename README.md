# 🗳️ Election Data Analysis & Winner Prediction

## 📌 Project Overview

This project performs an end-to-end data analysis on Indian election data to understand the key factors influencing election outcomes and prepare the dataset for machine learning models.

It follows a structured data science pipeline including data cleaning, exploratory data analysis (EDA), feature engineering, and statistical visualization.

---

## 🎯 Objectives

* Analyze patterns behind winning candidates
* Understand impact of assets, age, criminal cases, and party
* Clean and transform raw data into model-ready format
* Prepare dataset for future machine learning models

---

## 📂 Dataset Information

* Total Records: **2263**
* Features: **19**
* After Cleaning: **2018 records**

### Key Features

* Demographics: AGE, GENDER, CATEGORY
* Political: PARTY, STATE, CONSTITUENCY
* Financial: ASSETS, LIABILITIES
* Performance: TOTAL VOTES, VOTE SHARE
* Target Variable: **WINNER (0 = No, 1 = Yes)**

---

## ⚙️ Tech Stack

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn

---

## 🔄 Workflow

### 1. Data Loading

* Dataset uploaded using Google Colab
* Loaded into Pandas DataFrame

### 2. Initial Inspection

* Checked shape, columns, data types
* Identified missing values
* Used describe() for statistics

### 3. Data Cleaning

* Removed newline characters from column names
* Standardized column names
* Removed NOTA entries
* Dropped unnecessary columns (NAME, SYMBOL)

### 4. Feature Engineering

* Converted CRIMINAL CASES to numeric
* Cleaned ASSETS and LIABILITIES (removed currency symbols)
* Converted to numerical values

### 5. Exploratory Data Analysis (EDA)

#### Target Variable

* Winners: 539
* Non-Winners: 1724
  → Shows class imbalance

#### Categorical Analysis

* Party vs Winning
* Gender vs Winning
* Category vs Winning

#### Numerical Analysis

* Age distribution
* Assets distribution
* Criminal cases distribution

---

## 📊 Advanced Analysis

* Log transformation applied to ASSETS
* Outliers (top 1%) removed
* KDE plots for distribution comparison
* ECDF for cumulative analysis
* Boxplots for comparison

---

## 📈 Correlation Analysis

* Heatmap used to analyze relationships
* Strong relation between:

  * TOTAL VOTES & WINNER
  * Vote Share & WINNER

---

## 📊 Data Pipeline

Raw Data
↓
Data Cleaning
↓
Feature Engineering
↓
EDA & Visualization
↓
Data Transformation
↓
Model Ready Dataset

---

## 🔍 Key Insights

* Higher assets → higher probability of winning
* Criminal cases do not prevent winning
* Most candidates are aged 40–60
* Vote share is the strongest indicator of winning
* Certain parties dominate election results

---

## ⚠️ Challenges

* Missing values in multiple columns
* Financial data in string format
* Highly skewed distributions
* Class imbalance problem

---

## 🚀 Future Work

* Apply ML Models:

  * Logistic Regression
  * Random Forest
  * XGBoost
* Handle imbalance using SMOTE
* Feature selection & optimization
* Build prediction system

---

## 📁 Project Structure

Election-Data-Analysis/
│
├── data/
│   └── election_data.csv
│
├── notebook/
│   └── analysis.ipynb
│
├── images/
│   └── plots
│
├── README.md
└── requirements.txt

---

## 🧾 Conclusion

This project demonstrates a complete data analysis pipeline from raw dataset to meaningful insights. It highlights how structured data analysis can uncover patterns in election outcomes and prepare data for predictive modeling.

---

## 👩‍💻 Author

Jayeeta Dey
B.Tech AI & Technology Student

---

## ⭐ Support

If you like this project, give it a star ⭐ on GitHub!
