# Employee Attrition Prediction using Machine Learning

## Project Overview

Employee attrition is a major challenge for organizations because it increases recruitment costs, training expenses, and productivity loss. This project aims to predict whether an employee is likely to leave the company using machine learning techniques and identify the key factors that influence employee attrition.

The project uses the IBM HR Analytics Employee Attrition dataset to analyze employee characteristics such as department, job role, salary, work-life balance, years at the company, overtime, and other HR-related attributes. Multiple classification models are developed and compared to determine the most effective approach for predicting employee attrition.

---

## Objectives

* Analyze employee attrition patterns using exploratory data analysis (EDA).
* Clean and preprocess HR data for machine learning.
* Build multiple classification models for attrition prediction.
* Compare model performance using different evaluation metrics.
* Identify the most important factors contributing to employee attrition.
* Provide HR recommendations based on the findings.

---

## Dataset Information

* **Dataset:** IBM HR Analytics Employee Attrition Dataset
* **Source:** Kaggle
* **Total Records:** 1,470 Employees
* **Target Variable:** Attrition (Yes/No)

### Dataset Overview

* Employees Stayed: **1,233**
* Employees Left: **237**
* Overall Attrition Rate: **16.12%**

The dataset is imbalanced because a significantly larger number of employees stayed with the company than left.

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

### 1. Data Loading and Exploration

* Loaded the IBM HR Analytics Employee Attrition dataset.
* Displayed the first few records of the dataset.
* Checked dataset dimensions and data types.
* Calculated employee attrition rate.
* Identified numerical and categorical features.
* Checked for missing values.
* Checked for duplicate records.
* Generated summary statistics for numerical features.

### 2. Data Preprocessing

* Removed irrelevant columns:

  * EmployeeNumber
  * EmployeeCount
  * Over18
  * StandardHours
* Converted the target variable (Attrition) into binary format.
* Applied One-Hot Encoding to categorical variables.
* Standardized numerical features using StandardScaler.

### 3. Exploratory Data Analysis

The following analyses were performed:

* Attrition Rate by Department
* Attrition Rate by Job Role
* Monthly Income vs Attrition
* Work-Life Balance vs Attrition
* Years at Company vs Attrition

These visualizations helped identify employee groups that are more likely to leave the organization.

---

## Machine Learning Models

Three classification models were trained and evaluated:

1. Logistic Regression
2. Random Forest Classifier
3. Gradient Boosting Classifier

To address class imbalance, class weights were applied where appropriate during model training.

---

## Model Evaluation

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC Score
* Confusion Matrix

### Model Performance

| Model                        | Accuracy | ROC-AUC |
| ---------------------------- | -------: | ------: |
| Logistic Regression          |      75% |   0.799 |
| Random Forest Classifier     |      83% |   0.752 |
| Gradient Boosting Classifier |      85% |   0.794 |

### Best Overall Model

Gradient Boosting Classifier achieved the highest overall accuracy (approximately 85%) and provided the most balanced performance across evaluation metrics.

Although Logistic Regression achieved slightly lower overall accuracy, it obtained the highest recall for identifying employees who were likely to leave. This makes it valuable in situations where detecting potential attrition is more important than maximizing overall accuracy.

---

## Visualizations

The project includes the following visualizations:

* Attrition Rate by Department
* Attrition Rate by Job Role
* Monthly Income vs Attrition (Box Plot)
* Work-Life Balance vs Attrition
* Years at Company vs Attrition
* Confusion Matrix
* Top 10 Feature Importance
* ROC Curve Comparison

---

## Key Findings

* Employee attrition is concentrated in specific departments and job roles rather than being evenly distributed across the organization.
* Employees with lower monthly income generally have a higher likelihood of leaving the company.
* Employees with fewer years at the company show higher attrition rates compared to long-serving employees.
* Better work-life balance is associated with improved employee retention.
* Employee attrition is influenced by multiple workplace factors, including salary, tenure, overtime, job role, and work-life balance.

---

## HR Recommendations

* Focus retention efforts on departments and job roles with higher employee attrition.
* Strengthen onboarding and mentorship programs for newly hired employees.
* Improve work-life balance through flexible work policies and employee wellness initiatives.
* Review compensation structures and career growth opportunities for employees in lower salary ranges.
* Conduct regular employee feedback surveys to identify workplace issues before employees decide to leave.

---

## Project Limitations

* The dataset is imbalanced, with significantly fewer attrition cases than non-attrition cases.
* External factors such as personal circumstances and economic conditions are not included in the dataset.
* The model should be used as a decision-support tool rather than replacing human judgment.

---

## Future Improvements

* Apply hyperparameter tuning to improve model performance.
* Use SMOTE or other oversampling techniques to better handle class imbalance.
* Experiment with advanced ensemble models such as XGBoost or LightGBM.
* Use SHAP or LIME for explainable AI and model interpretability.
* Deploy the trained model as a web application using Streamlit or Flask.

---

## Folder Structure

```text
Employee_Attrition_Project/

├── Employee_Attrition_Project2.ipynb
├── WA_Fn-UseC_-HR-Employee-Attrition.csv
├── README.md
├── summary.pdf
└── charts/
    ├── department_attrition.png
    ├── jobrole_attrition.png
    ├── monthly_income_boxplot.png
    ├── worklife_balance.png
    ├── years_at_company.png
    ├── confusion_matrix.png
    ├── feature_importance.png
    ├── Boxplot of numerical values.png
    └── roc_curve.png
```

---

## Conclusion

This project demonstrates how machine learning can be used to predict employee attrition and support data-driven HR decision-making. By comparing multiple classification models and analyzing employee characteristics, the project identifies important factors contributing to attrition and provides actionable recommendations to improve employee retention. The findings can help organizations develop proactive HR strategies, reduce employee turnover, and create a more stable and engaged workforce.

---

## Author

**Lavanya Saxena**

B.Tech – Artificial Intelligence & Data Science

Dr. Akhilesh Das Gupta Institute of Professional Studies (ADGIPS)
