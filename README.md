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

🔍 1. Data Exploration

The dataset was initially explored using:

head()
tail()
info()
shape
columns
describe()

These operations were used to understand the dataset structure, number of observations, data types and statistical properties.

📦 5. Outlier Analysis
Outliers were analysed using boxplots and an IQR-based approach for numerical variables.
This step was performed to identify unusual values in the numerical features before further modelling preparation.

🤖 10. Machine Learning Algorithms

The project workflow includes the following Regression algorithms:

1. Linear Regression

A basic regression algorithm used as a baseline model.

2. Decision Tree Regressor

Uses decision-tree-based rules to predict the rental count.

3. Random Forest Regressor

An ensemble learning algorithm that combines multiple decision trees.

4. AdaBoost Regressor

A boosting-based regression algorithm included in the project workflow.

5. Gradient Boosting Regressor

Builds models sequentially to improve prediction performance.


🏆 12. Model Results

The evaluated models produced the following results:

Model	R² Score	MAE	MSE	RMSE
Linear Regression	0.4206	99.62	17045.29	130.56
Decision Tree	0.8809	36.06	3503.09	59.19
Random Forest	0.9389	26.75	1798.31	42.41
Gradient Boosting	0.8695	44.07	3840.27	61.97
🥇 Best Performing Model

Random Forest Regressor

Performance:

R² Score  : 0.9389
MAE       : 26.75
MSE       : 1798.31
RMSE      : 42.41

Random Forest achieved the highest R² score among the evaluated models and the lowest MAE and RMSE.

📊 13. Accuracy Percentage

For project presentation purposes, the R² score was expressed as a percentage:

Accuracy % = R² × 100

For Random Forest:

0.9389 × 100 = 93.89%

Therefore:

Random Forest R²-based percentage = 93.89%

Note: This is an R²-based percentage used for project presentation. It is not classification accuracy.

📉 14. Visualizations

The project includes graphs for analysing:

Feature correlations
Outliers
Model performance
R² comparison
MSE comparison
Hourly bike rental patterns

These visualizations help understand the dataset and compare the performance of different regression algorithms.

🛠️ Technologies Used
Python
Jupyter Notebook
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Machine Learning
Regression
📁 Project Structure
Bike-Sharing-Regression/
│
├── hour.csv
│
├── Bike_Sharing_Regression.ipynb
│
├── README.md
│
└── Bike_Sharing_Regression_Presentation.pptx
🚀 How to Run the Project
Step 1 – Clone the repository
git clone <your-repository-link>
Step 2 – Open the project

Open the project folder in:

Jupyter Notebook
JupyterLab
VS Code
Google Colab
Step 3 – Install required libraries
pip install pandas numpy matplotlib seaborn scikit-learn
Step 4 – Load the dataset

Make sure hour.csv is available in the same project directory.

Step 5 – Run the notebook

Open:

Bike_Sharing_Regression.ipynb

and execute the cells sequentially.

🎓 Learning Outcomes

Through this project, the following concepts were implemented:

Dataset exploration
Data cleaning
Missing-value checking
Duplicate checking
Correlation analysis
Feature engineering
Outlier analysis
Feature selection
Yeo-Johnson transformation
Standard scaling
Train/Test splitting
Regression algorithms
Model evaluation
Model comparison
Data visualization

