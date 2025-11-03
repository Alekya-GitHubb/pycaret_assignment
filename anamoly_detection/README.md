
---

##  README.md — Anomaly Detection**

```markdown
#  Anomaly Detection (PyCaret)

##  Objective
Detect unusual patterns in transaction data using unsupervised anomaly detection.

##  Dataset
Credit card transactions dataset

##  Tools
- Python
- PyCaret (Anomaly Detection)

##  Workflow
1. Load dataset
2. Explore & clean data
3. Setup PyCaret anomaly module
4. Train models & compare
5. Select best model (Isolation Forest)
6. Label anomalies
7. Export results

##  Best Model
**Isolation Forest**

| Metric | Value |
|---|---|
| % Anomalies | ~2–3% |

##  Generated Files
| File | Description |
|---|---|
| `anomaly_model.pkl` | Trained model |
| `anomaly_predictions.csv` | Labeled data |

##  Run Inference
```python
from pycaret.anomaly import load_model, predict_model
model = load_model("anomaly_model")
preds = predict_model(model)
preds.head()
