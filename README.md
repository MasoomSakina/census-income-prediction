# Semester Project: Census Income Prediction

## 📌 Project Overview
This project focuses on data loading, quality inspection, and binary classification using the Census Income dataset. The primary goal is to clean and prepare a 42-feature dataset to accurately predict whether an individual's income level exceeds $50K/year based on historical census characteristics.

### 👤 Author Information
- **Name:** Masoom Sakina
- **Program:** BS Data Science (Semester 6)
- **Task:** Data Loading, Inspection, and Classification

---

## 🛠️ Data Pipeline & Workflow

### 1. Data Loading & Metadata Inspection
- Programmatically extracted layout and column definitions from `census-income.names` to serve as a data dictionary.
- Initialized core data science libraries (`pandas` and `numpy`) for structured data manipulation.
- Mapped 42 explicitly defined feature names onto the raw training (`census-income.data`) and testing datasets to fix the missing headers.

### 2. Quality Assurance & Cleaning
- Identified and removed duplicate observations from both data splits to prevent modeling bias (3,229 rows from training; 883 rows from testing).
- Standardized character-based missing value placeholders (`'?'`) into numeric Python `NaN` formats.
- Handled high-sparsity features and applied statistical mode imputation to fill missing fields safely based on training distributions.

### 3. Exploratory Data Analysis (EDA) & Optimization
To understand data distributions and evaluate performance, multiple diagnostic visual checks were implemented across the pipeline.

---

## 📊 Visual Results

### 1. Exploratory Data Analysis Diagnostics
We analyzed the dataset structural health across four key layouts: target class imbalance distributions, continuous input skewness attributes, bivariate target associations, and feature collinearity check matrices.

![Exploratory Data Analysis Diagnostics](visuals/EDA%20charts.png)

### 2. Hyperparameter Tuning & Convergence
Shows the iterative optimization validation curve tracing ensemble parameter search performance.

![Ensemble Optimization Curve](visuals/Ensemble%20Optimization%20curve.png)

### 3. Model Evaluation Matrix
The final predictive performance checked against unseen test configurations using an optimized LightGBM matrix layout.

![Final Optimization LightGMB Matrix](visuals/Final%20Optimization%20LightGMB.png)

---

## 🏁 Project Status: COMPLETED ✅
The data preprocessing pipelines, exploratory visualizations, and initial diagnostics are optimized. The environment stands fully prepared to accept non-linear ensemble frameworks or specialized neural networks in subsequent assessments.
