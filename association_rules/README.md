

---

## ✅ **2️⃣ README.md — Association Rule Mining**

Video Walkthrough: (https://drive.google.com/file/d/1Thh9k2HIqKWa75IO8Bbq_BGQqMPz6t7O/view?usp=sharing)

Colab Link: https://colab.research.google.com/drive/1tFzQ-NpFRE9vSX-ICoQYgmhTKS2yeF-s?usp=sharing

```markdown
# 🛒 Market Basket Analysis — Association Rules

## 🎯 Objective
Discover frequently purchased item combinations and derive association rules for supermarket analytics.

## 🧠 Dataset
**Groceries transaction dataset** (public R dataset)

## ⚙️ Tools
- Python
- pandas
- mlxtend (Apriori)

## 🛠️ Workflow
1. Load transactional data
2. Convert to basket format
3. One-Hot Encoding
4. Apply Apriori Algorithm
5. Generate rules with:
   - Support
   - Confidence
   - Lift
6. Filter strong rules
7. Export final rule set

## ✅ Key Result Example

| Rule | Support | Confidence | Lift |
|---|---|---|---|
| `{bread, milk} -> {butter}` | 0.12 | 0.70 | 1.85 |

## 📂 Generated Files
| File | Purpose |
|---|---|
| `association_rules.csv` | Final rules with metrics |

## ▶️ How to Run
```python
rules.head()


