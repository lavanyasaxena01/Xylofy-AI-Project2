# Employee Attrition Prediction using Machine Learning

## Project Overview

Employee attrition is a major challenge for organizations as it leads to increased recruitment costs, training expenses, and productivity loss. This project aims to predict whether an employee is likely to leave the company using machine learning techniques and HR analytics.

Using the IBM HR Analytics Employee Attrition dataset, various employee-related factors such as salary, job role, work-life balance, overtime, and years at the company were analyzed to identify patterns associated with employee turnover.

---

## Objectives

* Analyze employee attrition patterns using exploratory data analysis (EDA).
* Preprocess HR data for machine learning.
* Build and compare multiple classification models.
* Identify the key factors influencing employee attrition.
* Generate actionable HR recommendations to improve employee retention.

---

## Dataset Information

* **Dataset:** IBM HR Analytics Employee Attrition Dataset
* **Source:** Kaggle
* **Total Records:** 1,470 Employees
* **Target Variable:** Attrition (Yes/No)

### Attrition Distribution

* Employees Stayed: 1,233
* Employees Left: 237
* Attrition Rate: ~16.12%

The dataset is imbalanced, with significantly more employees staying than leaving.

---

## Technologies Used

### Programming Language

* Python 3.x

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

### Development Environment

* Jupyter Notebook / Google Colab

---

## Project Workflow

### 1. Data Exploration

* Loaded and explored the dataset.
* Identified numerical and categorical features.
* Calculated attrition rate.
* Examined class distribution.

### 2. Data Preprocessing

* Removed irrelevant columns:

  * EmployeeNumber
  * EmployeeCount
  * Over18
  * StandardHours
* Converted Attrition into binary format (1/0).
* Applied One-Hot Encoding to categorical features.
* Standardized numerical features using StandardScaler.

### 3. Exploratory Data Analysis

Analyzed:

* Attrition by Department
* Attrition by Job Role
* Attrition vs Monthly Income
* Attrition vs Work-Life Balance
* Attrition vs Years at Company

### 4. Model Building

Three classification models were trained:

1. Logistic Regression
2. Random Forest Classifier
3. Gradient Boosting Classifier

Class imbalance was handled using:

```python
class_weight='balanced'
```

---

## Model Performance

| Model               | Accuracy | ROC-AUC |
| ------------------- | -------- | ------- |
| Logistic Regression | 75%      | 0.799   |
| Random Forest       | 83%      | 0.752   |
| Gradient Boosting   | 85%      | 0.794   |

### Best Overall Model

**Gradient Boosting Classifier**

* Highest Accuracy (~85%)
* Strong overall predictive performance

### Best Attrition Detection Model

**Logistic Regression**

* Highest Recall for identifying employees likely to leave
* Most interpretable for HR teams

---

## Visualizations

The following visualizations were created:

1. Attrition Rate by Department and Job Role
2. Monthly Income vs Attrition (Box Plot)
3. Confusion Matrix Heatmap
4. Top 10 Feature Importance Chart
5. ROC Curve Comparison (Bonus)

---

## Key Findings

* Employees with lower monthly income tend to leave more frequently.
* Attrition is higher among employees with fewer years at the company.
* Work-life balance shows a clear relationship with employee retention.
* Certain departments and job roles experience higher attrition rates.
* Salary alone does not explain employee turnover; multiple workplace factors contribute.

---

## Business Recommendations

### Recommendation 1

Focus retention efforts on employees in high-risk job roles and departments by conducting regular engagement and satisfaction surveys.

### Recommendation 2

Improve career development opportunities, mentorship programs, and work-life balance initiatives for employees during their early years at the company.

---

## Project Limitations

* The model relies on historical HR data and cannot capture all personal or external factors influencing employee decisions.
* Employee behavior can change over time, requiring periodic model retraining.
* Predictions should support HR decision-making rather than replace human judgment.

---

## Conclusion

This project demonstrates how machine learning can be applied to HR analytics to identify employees at risk of leaving the organization. By understanding the factors that drive attrition, companies can implement targeted retention strategies, improve employee satisfaction, and reduce turnover-related costs.

## Author

**Lavanya Saxena**

B.Tech – Artificial Intelligence & Data Science

Dr. Akhilesh Das Gupta Institute of Professional Studies (ADGIPS)

---
