
---

##  README.md — Time Series Forecasting (Univariate)**


# Time Series Forecasting — Univariate (Airline Passengers)

##  Objective
Forecast monthly airline passengers using classical time series models.

##  Dataset
Airline Passengers dataset (monthly)

##  Tools
- PyCaret Time Series
- Pandas
- Matplotlib

##  Workflow
1. Load dataset & parse dates
2. Visualize trend & seasonal pattern
3. Initialize PyCaret TS setup
4. Train & compare models (ARIMA, ETS, Prophet)
5. Forecast future 12 months
6. Save model & forecast output

##  Best Model
Selected via `compare_models()`

##  Output Files
| File | Purpose |
|---|---|
| `ts_model.pkl` | Saved forecasting model |
| `forecast.csv` | Future predictions |

##  Predict
```python
from pycaret.time_series import load_model, predict_model
model = load_model("ts_model")
forecast = predict_model(model, fh=12)
forecast
