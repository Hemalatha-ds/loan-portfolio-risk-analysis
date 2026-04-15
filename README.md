# 📊 Loan Portfolio Risk & Delinquency Analysis

## 🔍 Project Overview

This project analyzes a simulated personal loan portfolio to evaluate credit risk, identify delinquency patterns, and support data-driven lending decisions. The analysis is built using Python, SQL, and Power BI, focusing on Days Past Due (DPD) as the key risk metric.

---

## 🎯 Business Objective

* Measure overall portfolio risk using default rate
* Identify high-risk customer segments
* Analyze delinquency distribution using DPD buckets
* Build an interactive dashboard for monitoring key risk indicators

---

## 📁 Dataset Description

The dataset is synthetically generated and consists of:

* **Customers Table**: customer_id, age, income, employment_type, credit_score

* **Loans Table**: loan_id, customer_id, loan_amount, interest_rate

* **Payments Table**: payment_id, loan_id, due_date, paid_date

* Total Loans: ~20,000

* Customers: ~15,000

---

## ⚙️ Methodology

### 🔹 1. Data Processing (Python)

* Data cleaning and preprocessing using Pandas and NumPy
* Handling missing values and formatting date columns

### 🔹 2. DPD Calculation (SQL)

* Calculated Days Past Due (DPD) using `julianday()`
* Handled both paid and unpaid loans
* Applied DPD capping at 365 days

### 🔹 3. Default Definition

* Defined default as **DPD ≥ 90 days**
* Calculated overall default rate

### 🔹 4. Feature Engineering

* Created:

  * Credit Score Bands
  * Income Bands
  * DPD Buckets (0, 1–30, 31–60, 61–90, 90+)

---

## 📊 Key Insights

* Overall Default Rate: **13.58%**
* Highest risk observed in **low credit score segment (<600)** (~19%)
* Higher defaults in **low-income group (Below 3L ~15.62%)**
* Self-employed borrowers show slightly higher default rates than salaried
* Maximum delinquency observed in **31–60 DPD bucket**, indicating early-stage risk concentration

---

## 📈 Dashboard Features (Power BI)

* KPI Cards:

  * Total Loans
  * Defaulted Loans
  * Default Rate %
  * Average Max DPD

* Visualizations:

  * Default Rate by Credit Score Band
  * Default Rate by Income Band
  * Default Rate by Employment Type
  * Loan Distribution by DPD Bucket

* Interactive Filters:

  * Credit Score
  * Income Band
  * Employment Type

---

## 🛠️ Tools & Technologies

* **Python**: Pandas, NumPy
* **SQL (SQLite)**: Data transformation and DPD calculation
* **Power BI**: Dashboard and visualization

---

## 🚀 Project Outcome

Developed a complete risk analytics solution that enables monitoring of loan portfolio health, identification of high-risk segments, and improved decision-making for lending strategies.

---

## 📌 Future Improvements

* Incorporate machine learning models for default prediction
* Add time-series analysis for trend forecasting
* Integrate real-world datasets for production-level analysis

---

## 📷 Dashboard Preview



---

## 📬 Contact

If you have any questions or suggestions, feel free to connect!

