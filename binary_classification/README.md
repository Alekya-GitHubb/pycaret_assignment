# PyCaret Assignment - Binary Classification
# Customer Churn Prediction — Binary Classification using PyCaret

Video Walkthrough: (https://drive.google.com/file/d/1zqvM44o0NNUNwd1Zjfy9yXxfTqMOCBn-/view?usp=sharing)

Colab Link: https://colab.research.google.com/drive/1RRJg9WQZYqUxxv2yauh_jKwhlc-qQG0-?usp=sharing

## Project Overview
Customer churn prediction is critical for telecom companies to retain high-value users by identifying customers likely to leave.  
This project builds a machine-learning pipeline using **PyCaret Classification** to classify customers as:

- `Churn = Yes` — likely to leave
- `Churn = No` — likely to stay

## Objective
Develop an automated binary classification model to predict churn probability and assist proactive retention strategies.

##  Dataset Used
**Telco Customer Churn Dataset**  
Contains information on customer demographics, services, billing & contract details.

### Key Columns
| Feature Type | Examples |
|---|---|
Demographics | gender, SeniorCitizen, tenure  
Subscription & Usage | InternetService, StreamingTV  
Contract / Billing | Contract, MonthlyCharges, PaymentMethod  
Target Variable | `Churn` (Yes/No) |

## Data Preprocessing Performed
- Checked for missing values
- Encoded categorical features automatically via PyCaret
- Outlier handling (default with model setup)
- Train-Test split handled internally by PyCaret

## PyCaret Setup Code

```python
from pycaret.classification import *
clf = setup(data=df, target='Churn', session_id=123, normalize=True, ignore_features=['customerID'])
