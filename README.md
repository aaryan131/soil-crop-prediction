# 🌾 Soil Crop Prediction Using Logistic Regression

This project uses machine learning to help farmers identify the **most suitable crop** to grow based on basic soil measurements such as **Nitrogen (N)**, **Phosphorous (P)**, **Potassium (K)**, and **pH value**.

---

## 📁 Dataset

- File: `soil_measures.csv`
- Columns:
  - `N` - Nitrogen content ratio in the soil
  - `P` - Phosphorous content ratio
  - `K` - Potassium content ratio
  - `ph` - pH value of the soil
  - `crop` - Target label representing the recommended crop

---

## 🎯 Project Goal

The goal is to:
1. **Predict the crop** using logistic regression models.
2. **Identify the most predictive single feature** (N, P, K, or pH).
3. Help farmers prioritize which soil metric to measure when resources are limited.

---

## 🧠 Machine Learning Approach

- **Model**: Logistic Regression (`scikit-learn`)
- **Problem Type**: Multi-class classification
- **Evaluation Metric**: F1-score (weighted)
- **Process**:
  - Trained one model **per feature**
  - Compared F1 scores
  - Reported the feature with the best predictive power

---

## 🏆 Results

The best predictive feature was:

```python
best_predictive_feature = {'K': 0.74}  # Example output
