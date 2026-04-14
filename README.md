# 📊 Job Market Intelligence System

## 👨‍💻 Author

**Nishant Tyagi**

---

## 🚀 Project Overview

The **Job Market Intelligence System** analyzes real-world job posting data to uncover actionable insights about the job market.

This project focuses on identifying:

* In-demand skills
* Top hiring companies
* Job distribution trends
* High-demand job prediction using Machine Learning

---

## 🎯 Business Problem

Organizations and job seekers often lack clarity on:

* Which skills are currently in demand
* Where hiring is concentrated
* Which roles are growing fastest

This project solves these problems using **data-driven insights from job listings**.

---

## 📂 Dataset

* Source: Kaggle Job Dataset
* File Used: `job.csv`

---

## 🧹 Data Cleaning

* Standardized column names
* Removed duplicate records
* Cleaned and preprocessed text data

---

## ⚙️ Feature Engineering

Since the dataset lacked structured skill columns:

* Extracted skills from job descriptions using keyword matching:

  * Python
  * SQL
  * Excel
  * Machine Learning
  * Data Analysis

* Created new features:

  * `skill_count`
  * `desc_length`
  * Binary skill indicators (`has_python`, `has_sql`, etc.)
  * `high_demand` (target variable)

---

## 📊 Exploratory Data Analysis (EDA)

### 📌 Top Job Roles

![Top Roles](outputs/Screenshot%202026-04-14%20210833.png)

**Insight:**
Technical roles dominate the job market.

---

### 📌 Top Companies

![Top Companies](outputs/Screenshot%202026-04-14%20210917.png)

**Insight:**
Hiring is concentrated among a few major companies.

---

### 📌 Job Locations

![Locations](outputs/Screenshot%202026-04-14%20210957.png)

**Insight:**
Jobs are concentrated in specific geographic areas.

---

### 📌 Skill Demand

![Skills](outputs/Screenshot%202026-04-14%20211053.png)

**Insight:**
SQL and Python are the most in-demand skills.

---

### 📌 Industry Distribution

![Industry](outputs/Screenshot%202026-04-14%20211304.png)

**Insight:**
Most jobs belong to the IT and Technology sector.

---

### 📌 Employment Type

![Employment](outputs/Screenshot%202026-04-14%20211124.png)

**Insight:**
The majority of roles are full-time positions.

---

## 🤖 Machine Learning

### 🎯 Objective

Predict whether a job is **high demand** based on engineered features.

---

### 🧠 Model Used

* Logistic Regression

---

### 📊 Features Used

* Skill-based features
* Encoded categorical variables
* Text-derived features

---

### 📈 Model Performance

![Confusion Matrix](outputs/Screenshot%202026-04-14%20211327.png)

* Accuracy: **~0.8 – 1.0**

---

## 📉 Key Insights

* SQL and Python dominate job requirements
* Hiring is driven by major tech companies
* Full-time roles significantly outnumber internships
* Skill count strongly influences demand prediction

---

## 🧠 Challenges Faced

* Lack of structured skill data
* Handling unstructured text
* Feature extraction complexity

---

## 🔧 Improvements Made

* Extracted skills using keyword-based techniques
* Engineered meaningful features from raw text
* Improved prediction performance using feature engineering

---

## 🚀 Future Improvements

* Apply NLP techniques (TF-IDF, BERT)
* Deploy using Streamlit
* Integrate real-time job scraping

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn
* Jupyter Notebook

---

## ⭐ Conclusion

This project demonstrates:

* End-to-end data analysis workflow
* Real-world business problem solving
* Advanced feature engineering
* Practical machine learning implementation

---

## 🔗 Repository

👉 https://github.com/jollytyagi360-art/job-market-intelligence-system
