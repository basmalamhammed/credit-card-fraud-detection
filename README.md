#  Credit Card Fraud Detection

A machine learning project to detect fraudulent credit card transactions using multiple classification models.

---

##  Dataset

- **Source**: Kaggle - Credit Card Fraud Detection
- **Size**: 198,365 transactions
- **Features**: V1–V28 (PCA-transformed), Amount, Time
- **Target**: Class (0 = Normal, 1 = Fraud)
- **Challenge**: Highly imbalanced data — only **0.19%** are fraud cases

---

##  What I Did

- Scaled `Amount` using `StandardScaler`
- Handled imbalanced data using `class_weight='balanced'` and `scale_pos_weight`
- Trained and compared **3 models**:
  - Logistic Regression
  - Random Forest
  - XGBoost ✅ *(Best)*
- Evaluated using **ROC-AUC, F1-Score, Precision, Recall**
- Visualized results using **Confusion Matrix**

---

##  Results

| Model | ROC-AUC | F1-Score (Fraud) |
|-------|---------|-----------------|
| Logistic Regression | 0.974 | 0.13 |
| Random Forest | 0.962 | 0.86 |
| **XGBoost**  | **0.978** | **0.87** |

> **XGBoost** achieved the best overall performance with the highest ROC-AUC and F1-Score.

---

##  Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Matplotlib, Seaborn
- Jupyter Notebook

---

##  Project Structure

```
├── Credit Card Fraud Detection.ipynb  # Main notebook
├── submission.csv                      # Kaggle submission file
└── README.md
```

---

##  How to Run

```bash
git clone https://github.com/basmalamhammed/credit-card-fraud-detection.git
cd credit-card-fraud-detection
jupyter notebook
```

---

*Open to feedback and suggestions for improvement!* 
