# 🚲 Bike Sharing – Hours Calculation using Regression

## 📌 Project Overview

This project focuses on predicting the **hourly rental count of bikes** using Machine Learning Regression techniques.

The project uses the **Bike Sharing hourly dataset** from the UCI Machine Learning Repository. The target variable is `cnt`, which represents the total number of rental bikes for a particular hour.

The project explores the dataset, performs data preprocessing and feature selection, applies transformation and scaling techniques, and compares multiple regression algorithms to identify the best-performing model.

---

## 🎯 Project Objective

The main objective of this project is:

> **To predict the count of rental bikes for hourly observations using Regression Machine Learning algorithms.**

The project analyses different factors such as:

- Season
- Year
- Month
- Hour
- Holiday
- Weekday
- Working Day
- Weather Situation
- Temperature
- Feeling Temperature
- Humidity
- Windspeed

---

## 🎯 Target Variable

### `cnt`

`cnt` represents the **total number of rental bikes** for a particular hourly observation.

The project treats `cnt` as a **continuous numerical target**, making this a Regression problem.

---

## 📊 Dataset

### Dataset Name
**Bike Sharing Dataset – Hourly**

### Dataset Source

Fanaee-T, H. (2013). *Bike Sharing [Dataset].*  
UCI Machine Learning Repository.

### Dataset Link

https://doi.org/10.24432/C5W894

### Dataset Used

`hour.csv`

### Dataset Size

- **Rows:** 17,379
- **Columns:** 17
- **Time Period:** 2011–2012
- **Observation Type:** Hourly

---

## 🗂️ Original Dataset Features

| Feature | Description |
|---|---|
| `instant` | Record index |
| `dteday` | Date |
| `season` | Season |
| `yr` | Year |
| `mnth` | Month |
| `hr` | Hour |
| `holiday` | Holiday indicator |
| `weekday` | Day of the week |
| `workingday` | Working-day indicator |
| `weathersit` | Weather situation |
| `temp` | Normalized temperature |
| `atemp` | Normalized feeling temperature |
| `hum` | Normalized humidity |
| `windspeed` | Normalized wind speed |
| `casual` | Casual-user rental count |
| `registered` | Registered-user rental count |
| `cnt` | Total rental bike count |

---

# 🔄 Project Workflow

```text
Import
   ↓
Load hour.csv
   ↓
Head / Tail / Info / Shape / Describe
   ↓
Missing-Value Check
   ↓
Duplicate Check
   ↓
Correlation
   ↓
Rename Columns
   ↓
Date Processing
   ↓
Remove ID + casual + registered
   ↓
Outlier Analysis
   ↓
Feature Selection
   ↓
Yeo-Johnson Transformation
   ↓
Standard Scaling
   ↓
Train/Test Split
   ↓
Linear Regression
   ↓
Decision Tree Regressor
   ↓
Random Forest Regressor
   ↓
AdaBoost Regressor
   ↓
Gradient Boosting Regressor
   ↓
R² / MAE / MSE / RMSE
   ↓
Model Comparison
   ↓
Best Model
   ↓
Accuracy %
   ↓
Graphs
