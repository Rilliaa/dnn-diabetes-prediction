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

The research was conducted in multiple stages to evaluate the performance of Deep Neural Network (DNN) models under various optimization techniques. The workflow is as follows:

### 🔹 Stage 1: Research Design
- Define problem and objectives
- Collect dataset
- Conduct exploratory data analysis (EDA)

### 🔹 Stage 2: Data Preprocessing
- Load dataset (`Dataset.csv`)
- Data cleaning
- Feature normalization

### 🔹 Stage 3: Model Development

Several variants of DNN models were developed and compared:

#### 🔸 1. Baseline Model (Default DNN)
- Stratified train-test split
- Train DNN without optimization
- Evaluate using Precision, Recall, F1-Score, ROC-AUC

#### 🔸 2. DNN + Self-Attention
- Add self-attention layer after base DNN
- Same train-test split
- Evaluate performance

#### 🔸 3. DNN + Feature Selection (KCC)
- Apply Kendall’s Correlation Coefficient to select features
- Train-test split on reduced features
- Train and evaluate DNN

#### 🔸 4. DNN + SMOTE
- Apply SMOTE oversampling on the training set
- Train and evaluate DNN on balanced data

#### 🔸 5. DNN + Autoencoders
- Train Autoencoder to perform nonlinear dimensionality reduction
- Extract latent features from encoder
- Train and evaluate DNN using compressed features

---

### 🔹 Stage 4: Optimization Combinations

To assess cumulative impact, the following combinations were tested:

#### 🔸 DNN with 2 Optimization Techniques
- DNN + KCC + Autoencoder
- DNN + KCC + Self-Attention
- DNN + KCC + SMOTE
- DNN + Autoencoder + Self-Attention
- DNN + Autoencoder + SMOTE
- DNN + Self-Attention + SMOTE

#### 🔸 DNN with 3 Optimization Techniques
- DNN + KCC + Autoencoder + Self-Attention
- DNN + KCC + Autoencoder + SMOTE
- DNN + KCC + Self-Attention + SMOTE
- DNN + Autoencoder + Self-Attention + SMOTE

#### 🔸 DNN with 4 Optimization Techniques (Final Model)
- DNN + KCC + Autoencoder + Self-Attention + SMOTE

---

### 🔹 Stage 5: Final Evaluation & Interpretation
- Evaluate all models using standard classification metrics:
  - Precision
  - Recall
  - F1-Score
  - ROC-AUC
---

## 🛠️ Libraries Used

- Python (Google Colab)
- Scikit-learn
- TensorFlow / Keras
- Imbalanced-learn 
- Matplotlib & Seaborn

---
## 📌 Key Results

This research aimed to develop a Deep Neural Network (DNN) model optimized using a combination of feature selection (Kendall’s Correlation Coefficient), dimensionality reduction (Autoencoders), data balancing (SMOTE), and attention mechanisms (Self-Attention), in order to improve multiclass classification of diabetes status (Normal, Pre-Diabetes, Diabetes).

The key findings are as follows:

1. **Baseline Performance**  
   The default DNN model without any optimization achieved an F1-Score of **0.4162**, serving as the reference point for further comparison.

2. **Individual Optimization Techniques**  
   - **SMOTE**: Significantly improved **Recall** (up to **0.4912**) but caused a drop in **Precision**, indicating a trade-off in learning from minority classes.  
   - **Self-Attention**: Achieved the highest **ROC-AUC score** (**0.7863**), enhancing class separability, though with limited impact on F1-Score.  
   - **Autoencoders**: Slightly improved **Precision**, but decreased performance in other metrics, suggesting that the latent features were suboptimal for classification.  
   - **KCC Feature Selection**: Improved model efficiency and stability while avoiding overfitting, helping the model to focus on the most relevant features.

3. **Combined Optimization Techniques**  
   - The best **quantitative performance** was achieved by combining **KCC + SMOTE**, which resulted in the highest **F1-Score of 0.4425**, outperforming the baseline in all major metrics.
   - Although the combination **KCC + SMOTE + Self-Attention** achieved the highest **average performance** (**0.5235**), the **KCC + SMOTE** model was selected as the **best model** due to its balance between performance, simplicity, and computational efficiency.

4. **Interpretability Insights**  
   - **KCC** effectively highlighted features most correlated with diabetes status, enabling more focused learning by the DNN.  
   - **SMOTE** consistently boosted Recall by allowing the model to better understand minority class patterns, although it risked reducing Precision.  
   - **Autoencoders**, in this context, were less effective—potentially due to the loss of critical information during encoding and less representative latent space for classification tasks.


