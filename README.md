# 🧠 Logistic Regression on Breast Cancer Dataset (Manual vs Scikit-learn)

This project implements *Logistic Regression from scratch using NumPy, and compares the performance against **Scikit-learn’s LogisticRegression* on the *Breast Cancer Wisconsin Dataset*.

---

## 📌 Dataset

- *Source*: [Kaggle - Breast Cancer Wisconsin Dataset](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)
- Contains features like:
  - Mean radius, texture, perimeter, area, smoothness, etc.
  - Diagnosis: Malignant (M) or Benign (B)

---

## 🛠 What I Did

### ✅ Manual Implementation
- sigmoid(z)
- compute_cost() with L2 Regularization
- compute_gradient()
- gradient_descent() with train/test cost tracking
- Custom predict() function

### ✅ Data Preprocessing
- Removed irrelevant columns (Unnamed: 32, ID)
- Label encoded target (M → 1, B → 0)
- Standardized all features
- Train/Test split (80/20)

### ✅ Evaluation Metrics
- Accuracy
- Confusion Matrix
- Classification Report (Precision, Recall, F1-score)
- 📉 Cost vs Iteration Curve (Train vs Test)

---

## 🔁 Comparison: Manual vs Scikit-learn

| Model                  | Accuracy | Comments                       |
|------------------------|----------|--------------------------------|
| Manual Logistic Regression | ~98.25% | Slightly better generalization |
| Scikit-learn LogisticRegression | ~97.36% | Still very competitive         |

---

## 📈 Cost Curve

The cost function for both train and test sets was plotted over 1000 iterations, showing:
- Smooth convergence
- No overfitting
- Generalization stability

---

## 🚀 How to Run

1. *Clone this repository:*
   ```bash
   git clone https://github.com/AkashJadon-tech/LogisticRegression_Manual_vs_SKLearn.git
   cd LogisticRegression_Manual_vs_SKLearn

## 📦 Requirements

Make sure the following libraries are installed:

```bash
numpy
pandas
scikit-learn
matplotlib
seaborn
