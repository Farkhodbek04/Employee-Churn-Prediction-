# 🔍 Employee Churn Prediction with Logistic Regression

This project is a machine learning pipeline that predicts whether an employee will **churn** (i.e., leave the company) based on various employment and personal features. Achieving a final accuracy of **96%**, this project demonstrates a complete ML workflow including data preprocessing, visualization, modeling, and evaluation.

---

## 📊 Dataset Overview

The dataset contains 1000 rows with the following features:

| Feature           | Description |
|-------------------|-------------|
| `Age`             | Age of the employee |
| `Gender`          | Gender (Male/Female) |
| `Tenure`          | Duration (in months) with the company |
| `MonthlyCharges`  | Monthly salary of the employee |
| `ContractType`    | Type of contract (e.g. Full-Time, Part-Time) |
| `InternetService` | Company internet access type |
| `TechSupport`     | Whether the employee receives IT support |
| `TotalCharges`    | Total compensation (monthly * tenure) |
| `Churn`           | Target variable – Yes or No |

---

## 🔁 Project Workflow

### 1. **Data Understanding**
- Columns are clearly defined.
- Explored data types, unique values, and value distributions.

### 2. **Data Cleaning**
- Handled missing values.
- Converted types where necessary (e.g., `TotalCharges` to float).
- Validated data consistency.

### 3. **Data Visualization**
- Visualized churn distribution, gender-wise churn, and other feature relationships.
- Used histograms, count plots, and correlation heatmaps via Seaborn and Matplotlib.

### 4. **Feature Engineering**
- One-hot encoded categorical variables.
- Created `TotalCharges` if not present.
- Scaled numerical features using `StandardScaler`.

### 5. **Model Training**
- Applied Logistic Regression using `scikit-learn`.
- Split dataset into **train/test (80/20)**.
- Achieved **accuracy: 96%** on test data.

### 6. **Evaluation**
- Confusion Matrix, Precision, Recall, F1 Score.
- Strong recall and precision indicate high predictive power for both classes.

---

## 🤖 Tools & Technologies

- **Python 3.12+**
- **Jupyter Notebook**
- **Pandas & NumPy**
- **Matplotlib & Seaborn**
- **Scikit-learn**

---

## 📈 Results Summary

| Metric         | Score |
|----------------|-------|
| Accuracy       | 96%   |
| Precision      | 96%   |
| Recall         | 100%  |
| F1-Score       | 98%   |

---

## 💡 Key Insights

- **Tenure and ContractType** are strong churn predictors.
- Logistic Regression performs well with proper preprocessing.
- Model generalizes well without overfitting.

---

## 🚀 How to Run

```bash
git clone https://github.com/Farkhodbek04/Employee-Churn-Prediction-.git
cd churn-prediction
jupyter notebook Churn_prediction.ipynb

