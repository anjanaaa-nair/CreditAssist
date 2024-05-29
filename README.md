# CreditAssist

## Project Overview

The Credit Card Classification project provides a web-based solution for predicting credit classification based on financial and personal attributes. It automates the credit assessment process using machine learning, offering quick insights into creditworthiness. By leveraging historical credit data, the project trains models such as Support Vector Machines (SVM), Random Forests (RF), Gradient Boosting (GB), and Logistic Regression (LR) to make predictions. Users input their information through a user-friendly interface, and the system generates predictions, aiding both lenders and borrowers in making informed decisions efficiently.

## Dataset Description

The dataset comprises 1000 samples, each containing various features related to individuals applying for credit. Here are some of the features:

1. CHK_ACCT: Checking account status, categorized into different levels such as "0DM" (no checking account), "less-200DM" (less than 200 DM balance), or "no-account" (no account exists).
2. Duration: Duration of the credit in months.
3. History: Credit history status, categorized into levels such as "critical", "duly-till-now", or "delay".
4. Purpose of credit: Purpose for which the credit is taken, such as "radio-tv", "education", "furniture", etc.
5. Credit Amount: Amount of credit in DM (Deutschmark).
6. Balance in Savings A/C: Balance in the savings account, categorized into different levels like "unknown", "less100DM", or "over1000DM".
7. Employment: Duration of employment, categorized into different levels such as "over-seven" (more than seven years), "four-years", etc.
8. Install_rate: Installment rate in percentage of disposable income.
9. Marital status: Marital status of the applicant, categorized into different levels such as "single-male", "female-divorced", "married-male", etc.
10. Co-applicant: Presence of a co-applicant, categorized as "none" or otherwise.
11. Present Resident: Duration of present residence, categorized into different levels such as "1" (less than one year) or "4" (more than four years).
12. Real Estate: Presence of real estate, categorized as "car", "building-society", etc.
13. Age: Age of the applicant.
14. Other installment: Presence of other installments, categorized as "none" or otherwise.
15. Residence: Type of residence, categorized as "own", "rent", etc.
16. Num_Credits: Number of existing credits at the bank.
17. Job: Job status of the applicant, categorized as "skilled", "unskilled-resident", "management", etc.
18. No. dependents: Number of dependents.
19. Phone: Availability of a phone, categorized as "yes" or "no".
20. Foreign: Foreign worker status, categorized as "yes" or "no".
21. Credit classification (Target Variable): Classification of credit risk, labeled as "good" or "bad".

## Data Preprocessing

The dataset used for training the classifier contains information about individuals' financial attributes and credit ratings. Before training the models, the data underwent preprocessing, including dropping irrelevant columns, handling missing values, encoding categorical variables, applying standard scaling to numerical features, and splitting the data into features and target variables.

## Model Training

Three base machine learning models were trained for this project: SVM Classifier, Random Forest Classifier, and Gradient Boosting Classifier. Additionally, a stacking ensemble technique was used to combine the predictions of these models and train a meta-model using Logistic Regression.

## Implementation Code

The Python code consists of two main files: `model.py` and `app.py`.
- `model.py` contains code for data preprocessing, model training, evaluation metrics calculation, and saving the trained models.
- `app.py` is a Flask web application that loads the trained models and scaler, defines routes for user input, predicts credit classification based on user input, and renders HTML templates for the user interface.

## Conclusion

In conclusion, the project achieved a remarkable accuracy score of 88.92% in predicting credit risk using a dataset of 1000 samples. Leveraging advanced machine learning techniques, the model provides valuable insights for financial institutions to make informed lending decisions. Deployed as a Flask web app, the model ensures easy accessibility and integration into existing workflows, enhancing credit risk management practices. This success highlights the potential for continued research and application in the field.

