# Credit-Risk-Modeling-and-Prediction-for-Portfolio-Optimization

## 📌 Project Overview

This project focuses on **credit risk modeling** using supervised machine learning techniques to predict the likelihood of borrower default. The dataset includes demographic and financial attributes such as income, age, debt ratio, and delinquency history. The main objective is to improve **risk interpretability** and **model performance** through structured feature engineering and robust evaluation metrics.

---

## ⚙️ Workflow

### 1. **Data Preprocessing**

* Handled missing values through imputation.
* Normalized continuous variables to stabilize model training.
* Balanced the dataset to address class imbalance between default vs non-default borrowers.

### 2. **Feature Engineering**

* **Delinquency Binning** → Converted raw delinquency counts into categorical bins (`0 = No delinquency`, `1 = Moderate delinquency`, `2 = High delinquency`) for interpretability by credit analysts.
* **Outlier Treatment** → Applied **IQR method** to cap extreme values in financial ratios (e.g., `DebtRatio`, `RevolvingUtilizationOfUnsecuredLines`).
* **Log Transformation** → Reduced skewness in highly skewed financial variables.
* **Age Grouping** → Segmented `age` into categorical brackets for better interpretability.

### 3. **Exploratory Data Analysis (EDA)**

* Distribution plots for income, age, debt ratio, and credit utilization.
* Correlation heatmaps to identify multicollinearity.
* Segmentation of default rates across key demographic and financial features.

### 4. **Modeling**

* Implemented supervised learning models (e.g., **Logistic Regression, Decision Trees, Random Forest**) to predict credit default.
* Compared performance across models to select the most robust classifier.

### 5. **Model Evaluation**

* **Precision** → To minimize false positives in risk flagging.
* **Recall** → To maximize detection of risky borrowers.
* **F1 Score** → Balanced trade-off between precision and recall.
* Evaluated metrics at multiple classification thresholds (0.3, 0.5, 0.7) to align with different business use cases.

---

## 🛠️ Tech Stack

* **Python**: pandas, numpy, scikit-learn
* **Visualization**: matplotlib, seaborn

---

## 📌 Key Insights

* Feature engineering (delinquency binning, IQR-based outlier treatment) improved interpretability and reduced noise in financial variables.
* Tree-based models provided strong predictive performance, while logistic regression gave interpretable coefficients for risk factors.
* Threshold tuning allows business teams to decide between conservative (high recall) or strict (high precision) default prediction strategies.

---

