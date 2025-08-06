# 🧠 Optimizing Deep Neural Network for Diabetes Status Prediction

This project is my undergraduate thesis which focuses on optimizing Deep Learning models for predicting diabetes status (Normal, Pre-diabetes, Diabetes) based on health indicator data. The main objective is to improve model performance using various optimization techniques including feature selection, dimensionality reduction, data balancing, and attention mechanisms.

---

## 📊 Dataset Overview

- **Source**: [Kaggle – Diabetes Health Indicators Dataset](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset)
- **Samples**: 253,680 rows
- **Features**: 21 health-related indicators
- **Target Classes**:
  - 0: Normal
  - 1: Pre-diabetes
  - 2: Diabetes

---

## 🧪 Research Workflow

The project workflow includes the following key steps:

1. **Feature Selection** using Kendall’s Correlation Coefficient (KCC)
2. **Data Normalization** and **SMOTE Oversampling** for class imbalance
3. **Dimensionality Reduction** using Autoencoders (non-linear)
4. **Deep Neural Network (DNN)** architecture for multiclass classification
5. **Self-Attention Mechanism** added to enhance feature learning
6. **Evaluation** using Accuracy, Precision, Recall, F1-Score, ROC-AUC
7. **Model Interpretation** with SHAP (Shapley Additive Explanations)

---

## 🛠️ Technologies Used

- Python (Google Colab)
- Scikit-learn
- TensorFlow / Keras
- Imbalanced-learn (SMOTE)
- SHAP
- Matplotlib & Seaborn

---

## 📁 Project Structure

