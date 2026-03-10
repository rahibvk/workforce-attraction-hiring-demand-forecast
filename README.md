Workforce Attrition & Hiring Demand Forecast

Project Overview

This project analyzes employee attrition patterns and builds a predictive model to estimate future replacement hiring demand.
The goal is to help Talent Acquisition (TA) teams identify workforce segments with higher attrition risk and proactively plan recruiting efforts.

By combining exploratory data analysis and machine learning, this project demonstrates how predictive analytics can support workforce planning decisions.

---

Business Objective

Talent Acquisition teams often need to answer questions such as:

- Which departments are at higher attrition risk?
- Which employee groups are more likely to leave?
- Where might replacement hiring demand increase?
- Which job roles should recruiting prioritize first?

This project addresses these questions by analyzing attrition patterns and translating predicted attrition risk into estimated hiring demand.

---

Dataset

IBM HR Analytics Employee Attrition & Performance Dataset

This dataset contains fictional HR data with employee demographics, job information, satisfaction scores, and employment history.

Dataset includes features such as:

- Age
- Department
- Job Role
- Monthly Income
- Job Satisfaction
- Work-Life Balance
- Years at Company
- Overtime
- Attrition (target variable)

Total records: 1470 employees

---

Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

Project Workflow

1. Data Audit & Cleaning

- Inspected dataset structure
- Checked for missing values and duplicates
- Removed irrelevant identifier columns
- Created a binary target variable for attrition

2. Exploratory Data Analysis

Key attrition drivers were analyzed using visualizations:

- Attrition by department
- Attrition by overtime status
- Attrition by job role
- Attrition by job satisfaction
- Attrition by work-life balance
- Tenure comparison between employees who stayed vs left

3. Predictive Modeling

Two models were evaluated:

- Logistic Regression (baseline model)
- Random Forest (comparison model)

Logistic Regression performed better for this business use case.

4. Threshold Tuning

The default classification threshold (0.50) was lowered to 0.30 to improve recall and better identify employees at risk of attrition.

This adjustment improved the model's ability to detect potential attrition cases for workforce planning.

5. Workforce Planning Insights

Predicted attrition probabilities were aggregated to estimate:

- Replacement hiring demand by department
- Replacement hiring demand by job role

---

Key Findings

Department-Level Insights

- Research & Development has the highest predicted replacement hiring volume due to its large workforce size.
- Sales shows the highest relative attrition pressure.

High-Risk Job Roles

Roles with the highest predicted replacement demand include:

- Laboratory Technician
- Sales Executive
- Research Scientist
- Sales Representative

Attrition Drivers

Key factors associated with higher attrition risk include:

- Working overtime
- Low job satisfaction
- Poor work-life balance
- Shorter tenure at the company

---

Visual Insights

Attrition Rate by Department

"Attrition by Department" (images/attrition_by_department.png)

Attrition Rate by Overtime

"Attrition by Overtime" (images/attrition_by_overtime.png)

Attrition Rate by Job Role

"Attrition by Job Role" (images/attrition_by_job_role.png)

Estimated Replacement Hiring Demand by Department

"Hiring Demand by Department" (images/replacement_hiring_by_department.png)

Estimated Replacement Hiring Demand by Job Role

"Hiring Demand by Job Role" (images/replacement_hiring_by_job_role.png)

Model Performance Comparison

"Model Comparison" (images/model_comparison.png)

---

Final Model

The final selected model is:

Logistic Regression with a classification threshold of 0.30

This model provided the best balance of precision and recall for identifying employees at risk of attrition.

---

Business Value

This project demonstrates how predictive analytics can support Talent Acquisition teams by:

- Identifying workforce segments with higher attrition risk
- Estimating replacement hiring demand
- Prioritizing recruiting efforts for high-risk roles
- Supporting proactive workforce planning decisions

---

Repository Structure

workforce-attrition-hiring-demand-forecast
│
├── data
│   └── WA_Fn-UseC_-HR-Employee-Attrition.csv
│
├── notebooks
│   └── workforce_attrition_hiring_demand_forecast.ipynb
│
├── images
│   ├── attrition_by_department.png
│   ├── attrition_by_overtime.png
│   ├── attrition_by_job_role.png
│   ├── replacement_hiring_by_department.png
│   ├── replacement_hiring_by_job_role.png
│   └── model_comparison.png
│
└── README.md

---

Future Improvements

Possible extensions to this project include:

- Hyperparameter tuning for improved model performance
- Adding feature importance analysis
- Incorporating time-series workforce data
- Building an interactive dashboard for HR teams

---

Author

This project was created as part of a Talent Acquisition Analytics portfolio to demonstrate data analysis, predictive modeling, and workforce planning insights using Python.
