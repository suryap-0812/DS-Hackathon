# Data Science Hackathon

This repository contains the Data Science solutions for **Question 6 (Q6)** and **Question 11 (Q11)**.

Both problems are implemented in a **single Jupyter Notebook / Google Colab notebook**. The notebook contains the complete workflow including data cleaning, exploratory data analysis, visualisation, statistical analysis, Linear Regression, model evaluation, key insights, and practical recommendations.

---

## Repository Structure

```text
DS-Hackathon/
│
├── DS_Day01.ipynb
│   └── Main Jupyter/Google Colab notebook
│       ├── Q6 — Banking
│       └── Q11 — HR Analytics
│
├── datasets/
│   ├── Q6/
│   │   └── DS_Day01_06_Banking_Inconsistent_Dataset_250.csv
│   │
│   └── Q11/
│       └── DS_Day01_11_HR_Salary_Inconsistent_Dataset.csv
│
└── README.md
Q6 — Banking
Does Income Really Determine Spending?
Industry

Banking and FinTech

Objective

The objective of this analysis is to investigate whether customer income is strongly associated with spending behaviour.

The analysis examines customer income, expenses, savings, credit-card spending, loans, age groups, and occupations to determine whether the assumption that higher-income customers automatically spend more is supported by the data.

Dataset

The Q6 dataset is located at:

datasets/Q6/DS_Day01_06_Banking_Inconsistent_Dataset_250.csv
Dataset Features
Feature	Description
Customer_ID	Unique customer identifier
Age_Group	Customer age category
Occupation	Customer occupation
Monthly_Income	Monthly income
Monthly_Expenses	Monthly expenditure
Savings	Monthly savings
Credit_Card_Spending	Monthly credit-card spending
Loan_Amount	Customer loan amount
Analysis Performed

The Q6 analysis includes:

Dataset inspection and validation
Missing-value detection and handling
Duplicate detection
Categorical-value standardisation
Numerical-value validation
Feature engineering
Savings ratio calculation
Expense-to-income ratio calculation
Income vs expenditure analysis
Salaried vs self-employed comparison
Age-group analysis
Unusual spending identification
Correlation analysis
Linear Regression
Model evaluation
Business insights
Practical action plan
Visualisations

The analysis includes four major visualisations:

Monthly Income vs Monthly Expenses
Average Savings Ratio by Occupation
Monthly Expenses — Salaried vs Self-employed
Distribution of Expense-to-Income Ratio
Machine Learning

Algorithm: Linear Regression

The primary objective of the model is to analyse the relationship between:

Monthly Income → Monthly Expenses

Model evaluation includes:

Mean Absolute Error (MAE)
Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
R² Score
Q11 — HR Analytics
Is the Company Paying People Fairly?
Industry

IT and HR Analytics

Objective

The objective of this analysis is to investigate employee compensation patterns and determine how salary varies across job roles, experience levels, education, locations, and performance.

The analysis focuses on identifying employees whose compensation differs substantially from employees with similar profiles rather than simply predicting salary.

Dataset

The Q11 dataset is located at:

datasets/Q11/DS_Day01_11_HR_Salary_Inconsistent_Dataset.csv
Dataset Features
Feature	Description
Employee_ID	Unique employee identifier
Designation	Employee's job role
Experience	Years of professional experience
Education	Highest education qualification
Location	Employee work location
Performance_Score	Employee performance rating
Salary	Annual employee salary
Salary_Increment	Salary increment percentage
Analysis Performed

The Q11 analysis includes:

Dataset inspection and validation
Missing-value detection and handling
Duplicate employee detection
Categorical-value standardisation
Numerical-value validation
Salary analysis across job roles
Salary growth with experience
Education-wise compensation analysis
Location-wise salary comparison
Performance vs salary increment analysis
Compensation anomaly detection
Expected salary estimation
Salary residual analysis
Linear Regression
Model evaluation
Key HR insights
Practical action plan
Compensation Analysis

The analysis calculates the difference between an employee's actual salary and the salary expected from the employee's observed characteristics.

Salary Residual =
Actual Salary − Expected Salary

Large positive or negative residuals are treated as potential compensation anomalies for further investigation.

A compensation anomaly does not automatically imply unfair treatment. It indicates that the employee's salary differs substantially from the model-based benchmark and should be investigated using additional HR information and company compensation policies.

Visualisations

The analysis includes four major visualisations:

Salary Distribution Across Job Roles
Salary Growth with Experience
Average Salary Across Locations
Performance Score vs Salary Increment
Machine Learning

Algorithm: Linear Regression

For Q11, Linear Regression is used as an analytical benchmark to examine salary relationships based on:

Designation
Experience
Education
Location
Performance Score

Model evaluation includes:

Mean Absolute Error (MAE)
Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
R² Score

The model is used as an analytical support tool rather than as the sole mechanism for determining employee compensation.

Notebook

Both Q6 and Q11 are implemented in:

DS_Day01.ipynb

There are no separate notebooks for Q6 and Q11.

The notebook is organised into separate sections for each question, allowing the datasets and analyses to be examined independently.

Data Quality

Both datasets are intentionally designed with inconsistencies to demonstrate the complete Data Science data-cleaning process.

The datasets contain examples of:

Missing values
Duplicate records
Inconsistent categorical formatting
Invalid categorical values
Invalid numerical values
Extreme observations
Behavioural anomalies
Compensation anomalies

These inconsistencies are identified and handled during the data-preprocessing stage of the notebook.

Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Jupyter Notebook
Google Colab
Machine Learning Workflow

The overall workflow followed for both questions is:

Raw Dataset
     │
     ▼
Data Inspection
     │
     ▼
Data Validation
     │
     ▼
Data Cleaning
     │
     ▼
Feature Engineering
     │
     ▼
Exploratory Data Analysis
     │
     ▼
Data Visualisation
     │
     ▼
Statistical Analysis
     │
     ▼
Linear Regression
     │
     ▼
Model Evaluation
     │
     ▼
Key Insights
     │
     ▼
Practical Action Plan
Expected Outputs

Each problem provides:

Cleaned dataset analysis
Descriptive statistics
4 visualisations
5–7 key insights
One trained Linear Regression model
Model evaluation results
Business/HR interpretation
Practical action plan
Project Files
Question	Domain	Dataset	Code
Q6	Banking & FinTech	datasets/Q6/DS_Day01_06_Banking_Inconsistent_Dataset_250.csv	DS_Day01.ipynb
Q11	IT & HR Analytics	datasets/Q11/DS_Day01_11_HR_Salary_Inconsistent_Dataset.csv	DS_Day01.ipynb
Conclusion

This project demonstrates the application of a complete Data Science workflow to two different business domains.

Q6 focuses on understanding customer spending behaviour and examining whether income is a meaningful predictor of expenditure.

Q11 focuses on analysing employee compensation patterns, salary growth, location differences, performance-linked increments, and potential compensation anomalies.

Both analyses combine data quality management, exploratory analysis, visualisation, statistical reasoning, and machine learning to convert raw data into actionable business insights.