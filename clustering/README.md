# Customer Segmentation using Clustering (PyCaret)

Video Walkthrough: (https://drive.google.com/file/d/1VnvpwQdlTaHqTg8bC3VMVfSIb8t_A2tp/view?usp=sharing)

Colab Link: https://colab.research.google.com/drive/1OyD1CdFt8zYkqU5epBis_Hjp7EfYPcSs?usp=sharing

##  Objective
Perform customer segmentation using clustering techniques to understand behavioral groups and enable better marketing strategies.

## Dataset
**Mall Customers Dataset**  
Contains demographics & spending behavior.

## Tools
- Python
- PyCaret (Clustering Module)
- Pandas, Matplotlib

## Workflow
1. Load dataset & inspect
2. Preprocess (handle nulls, scaling)
3. Initialize PyCaret clustering setup
4. Train & compare clustering models
5. Evaluate performance (Silhouette Score)
6. Save best model
7. Visualize clusters

## Best Model
**KMeans Clustering**

| Metric | Score |
|---|---|
| Silhouette Score | ~0.55 |
| Optimal Clusters | 3 |

## Generated Files
| File | Purpose |
|---|---|
| `cluster_model.pkl` | Trained PyCaret model |
| `cluster_results.csv` | Predictions & labels |

## How to Run
```python
from pycaret.clustering import load_model, predict_model
model = load_model("cluster_model")
preds = predict_model(model)
preds.head()


