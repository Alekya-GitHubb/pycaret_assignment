
---

##  README.md — Time Series Forecasting w/ Exogenous Variables**

Colab: (https://colab.research.google.com/drive/1AUtqhClM_jQEPr7ourNIlNe3VEdUlFUc?usp=sharing)

#  Time Series Forecasting with Exogenous Variables (SARIMAX)

##  Objective
Predict energy consumption using temperature as an external regressor.

##  Dataset
Energy demand + Weather temperature dataset

##  Tools
- PyCaret Time Series
- Pandas
- Statsmodels

##  Workflow
1. Load & merge time series and exogenous data
2. Visualize trends
3. Setup PyCaret TS with exogenous feature
4. Train SARIMAX / Prophet w/ regressors
5. Forecast future values
6. Save model

##  Model Outcome
Exogenous variable **improved forecast accuracy**

| Metric | Improvement |
|---|---|
| RMSE | ↓ better than univariate |

##  Files
| File | Purpose |
|---|---|
| `ts_exog_model.pkl` | Saved model |
| `exog_forecast.csv` | Forecasted values |

##  How to Run
```python
model = load_model("ts_exog_model")
forecast = predict_model(model, fh=30)
forecast






