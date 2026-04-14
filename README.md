# 📊 Job Market Intelligence System

**Author:** Nishant Tyagi

---

## 📌 Overview

This project analyzes job listings data to understand hiring trends, identify in-demand skills, and build a machine learning model to classify high-demand jobs.

The focus is on extracting insights from unstructured job descriptions and converting them into meaningful features.

---

## 🎯 Problem Statement

Many candidates struggle to identify which skills are actually required in the job market. This often leads to inefficient preparation and confusion in career direction.

This project aims to analyze job listings and uncover patterns in skill demand and hiring trends.

---

## 🛠️ Approach

### 🔹 1. Data Understanding

* Dataset contains job listings with title, company, location, and description
* No structured skill column present

---

### 🔹 2. Data Cleaning

* Renamed columns to lowercase
* Removed duplicates
* Cleaned text fields for consistency

---

### 🔹 3. Exploratory Data Analysis (EDA)

#### 📊 Top Job Roles

![Top Roles](outputs/Screenshot 2026-04-14 210833.png)

**Insight:**
Few technical roles dominate hiring demand.

---

#### 📊 Top Companies

![Top Companies](outputs/Screenshot 2026-04-14 210917.png)

**Insight:**
Hiring is concentrated among a limited number of companies.

---

#### 📊 Job Locations

![Locations](outputs/Screenshot 2026-04-14 210957.png)

**Insight:**
Jobs are concentrated in specific geographic regions.

---

#### 📊 Skill Demand

![Skills](outputs/Screenshot 2026-04-14 211053.png)

**Insight:**
SQL and Python are the most frequently required skills.

---

#### 📊 Industry Distribution

![Industries](outputs/Screenshot 2026-04-14 211124.png)

**Insight:**
Majority of roles belong to technology-related industries.

---

#### 📊 Employment Type

![Employment](outputs/Screenshot 2026-04-14 211219.png)

**Insight:**
Full-time roles dominate (~96% of listings).

---

---

## 🔥 Challenges & Learnings

### ❌ Missing Salary Data

* Initially assumed salary would be available
* Adjusted analysis to focus on skills and demand instead

---

### ❌ No Structured Skills Column

* Extracted skills from job descriptions using keyword matching

---

### ❌ Data Leakage Issue

* Used `skill_count` to define target and as a feature
* This caused 100% accuracy

👉 Fixed by removing dependent features

---

### ❌ Execution Order Issue

* Model was trained before defining the target
* Fixed by restructuring the workflow

---

---

## ⚙️ Feature Engineering

* Extracted key skills from job descriptions:

  * Python
  
  * Excel
  * Machine Learning
  * Data Analysis

* Created:

  * Binary skill indicators (presence/absence of each skill)
  * Derived features for modeling

---

## 🤖 Machine Learning Model

* Model: Logistic Regression
* Task: Binary classification (high-demand jobs)

---

### 📊 Model Evaluation

![Confusion Matrix](outputs/Screenshot 2026-04-14 211400.png)

---

## 📈 Results

* Achieved **~80% accuracy**
* Model performs well without overfitting

---

## 💡 Key Insights

* SQL and Python are the most demanded skills
* Skill combinations influence job demand
* Most roles are full-time
* Technology sector dominates hiring

---

## 🚀 Tech Stack

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn

---

## 📂 Project Structure

```
job-market-intelligence-system/
│
├── data/
├── notebooks/
├── outputs/
├── README.md
```

---

## 🔚 Conclusion

This project demonstrates how unstructured job data can be analyzed to extract meaningful insights and build predictive models.

It highlights the importance of:

* Proper feature engineering
* Avoiding data leakage
* Understanding real-world data limitations

---

## 📌 Future Improvements

* Add salary-based analysis
* Improve NLP techniques
* Build a deployment interface
