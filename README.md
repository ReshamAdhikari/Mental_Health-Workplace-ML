# Mental_Health-Workplace-ML
ML model to predict employee mental health treatment:  Undergraduate Dissertation
Resham Adhikari | BSc Computer Science | University of East London | 2025

Overview

This project was developed as part of my undergraduate final dissertation.
It uses machine learning to predict whether an employee is likely to seek 
mental health treatment based on workplace and personal factors.

The goal is to help organisations identify early indicators of mental health 
risk among employees using data-driven analysis.

Dataset

Source: Mental Health in Tech Survey : [Kaggle](https://www.kaggle.com/datasets/osmi/mental-health-in-tech-survey)
Rows: around 1,200 employee survey responses
Target variable: `treatment` whether the employee sought mental health treatment (Yes/No)


## Features Used (14)

| Feature | Description |

 Age | Employee age (filtered 18–60)
 Gender | Cleaned and standardised 
 family_history | Family history of mental illness 
 work_interfere | How much mental health affects work 
 wellness_program | Whether employer offers wellness programme 
 benefits | Mental health benefits provided 
 supervisor | Comfort discussing with supervisor 
 care_options | Awareness of care options 
 leave | Ease of taking mental health leave 
 coworkers | Comfort discussing with coworkers 
 mental_health_consequence | Fear of consequences for disclosing 
 seek_help | Whether employer encourages seeking help 
 remote_work | Works remotely 
 obs_consequence | Observed consequences for others 


## Models Compared

| Model | Accuracy 
Random Forest | **~80%** ... best model
Logistic Regression | ~69% 
K-Nearest Neighbours | ~69% 


## Key Findings

- **Random Forest** achieved the highest accuracy of ~80%
- **Most influential features:** age, family history, work_interfere, care_options
- **Least influential:** remote_work
- Employees with a family history of mental illness were significantly 
  more likely to seek treatment
- Workplace support factors (supervisor, care_options, leave) had a 
  strong relationship with treatment-seeking behaviour


## What This Notebook Contains

- Data cleaning (missing values, gender normalisation, age filtering)
- Exploratory data analysis with visualisations
- Label encoding and feature scaling
- Training and comparing 3 ML models
- Classification report and confusion matrix
- Feature importance analysis
- 5-fold cross-validation

## How to Run

1. Clone this repository
2. Install dependencies
3. Add the dataset, download from Kaggle link above and name it `Mental health at workpalce.csv`
4. Run the notebook top to bottom

## Limitations

- Dataset is from a tech industry survey and may not generalise to all industries
- Model is not clinically validated
- 1,200 rows is a relatively small dataset for ML

## Tech Stack

Python · Pandas · Scikit-learn · Matplotlib · Seaborn · NumPy · Joblib
