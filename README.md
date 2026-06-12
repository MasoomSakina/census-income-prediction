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

### 3. Exploratory Data Analysis (EDA)
To understand data distributions before modeling, the following visual checks were implemented:
1. **Target Class Imbalance:** Checked the distribution of the income targets.
2. **Feature Distributions:** Evaluated the scale and skewness of continuous variables like `age` and `wage_per_hour`.
3. **Correlation Matrix Heatmap:** Assessed multi-frequency linear relationships across numeric features to check for collinearity.

---

## 📊 Visual Results

### Class Distribution
Below is the visual overview of the class distributions from our analysis:

![Class Distribution](visuals/class_distribution.png)

---

## 🏁 Project Status: COMPLETED ✅
The data preprocessing pipelines, exploratory visualizations, and initial diagnostics are optimized. The environment stands fully prepared to accept non-linear ensemble frameworks or specialized neural networks in subsequent assessments.