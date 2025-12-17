
# 📈 **Regression — Detailed README.md**

Video Walkthrough: (https://drive.google.com/file/d/1tjmtspt5lhiTuINL8JwLkT0aye8x8bm7/view?usp=sharing)

```markdown
# House Price Prediction — Regression using PyCaret

## Project Purpose
Accurate property valuation helps buyers, sellers, and real-estate agencies make informed decisions.  
This project uses **PyCaret Regression** to predict median housing prices in California.

## Objective
Build, evaluate, and deploy a regression model to estimate housing prices based on demographic & geographic inputs.

## Dataset
**California Housing Dataset**  
(Available in sklearn)

### Key Features
| Category | Features |
|---|---|
Location | longitude, latitude  
Neighborhood | median_income, population  
Housing Features | avg_rooms, avg_bedrooms, housing_median_age  
Target | `median_house_value` |

## Exploratory Observations
- Housing prices increase with **median income**
- Coastal areas are more expensive (lat/long impact)
- Some skewness in target variable (log transform optional)

## ⚙️ PyCaret Setup

```python
from pycaret.regression import *
reg = setup(data=df, target='median_house_value', session_id=123, normalize=True)

