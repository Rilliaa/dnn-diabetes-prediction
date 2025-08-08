[EN]
# DNN Model with Dual Technique Combinations

This step, **`model+2_techniques`**, contains multiple experimental setups combining **Deep Neural Networks (DNNs)** with two enhancement techniques per model. Each configuration aims to improve the DNN's performance in handling imbalanced and complex data structures through hybrid modeling strategies.

## 📂 Contents Overview

Each  script inside this directory represents a specific combination of techniques applied in conjunction with DNN. The dual-technique strategies include:

- **Autoencoder + Kendall’s Correlation Coefficient (AE + KCC)**
- **Autoencoder + Self-Attention (AE + SA)**
- **Autoencoder + SMOTE (AE + SMOTE)**
- **Kendall’s Correlation Coefficient + Self-Attention (KCC + SA)**
- **Self-Attention + SMOTE (SA + SMOTE)**
- **Kendall’s Correlation Coefficient + SMOTE (KCC + SMOTE)**

---

## 🔄 Dual-Scenario Configurations

Some technique combinations are implemented in **two different scenarios** to examine the impact of **order of application**:

### 1. **KCC + AE**
- **Scenario 1**: Apply **Kendall’s Correlation Coefficient** first, followed by **Autoencoding**.
- **Scenario 2**: Apply **Autoencoding** first, followed by **KCC feature selection**.

### 2. **KCC + SMOTE**
- **Scenario 1**: Apply **Kendall’s Correlation Coefficient** before oversampling with **SMOTE**.
- **Scenario 2**: Apply **SMOTE** before performing **KCC-based feature selection**.

---

For detailed implementation or results, please refer to the respective folders or notebooks within this directory.

---
[ID]
# Model DNN dengan Kombinasi Dua Teknik

Langkah ini, **`model+2_techniques`**, berisi berbagai pengaturan eksperimen yang menggabungkan **Deep Neural Networks (DNN)** dengan dua teknik peningkatan pada setiap model. Setiap konfigurasi dirancang untuk meningkatkan performa DNN dalam menangani data yang tidak seimbang dan memiliki struktur kompleks melalui pendekatan pemodelan hibrida.

## 📂 Ringkasan Konten

Setiap skrip dalam direktori ini merepresentasikan kombinasi teknik tertentu yang diterapkan bersama DNN. Kombinasi dua teknik tersebut meliputi:

- **Autoencoder + Kendall’s Correlation Coefficient (AE + KCC)**
- **Autoencoder + Self-Attention (AE + SA)**
- **Autoencoder + SMOTE (AE + SMOTE)**
- **Kendall’s Correlation Coefficient + Self-Attention (KCC + SA)**
- **Self-Attention + SMOTE (SA + SMOTE)**
- **Kendall’s Correlation Coefficient + SMOTE (KCC + SMOTE)**

---

## 🔄 Konfigurasi Dua Skenario

Beberapa kombinasi teknik diterapkan dalam **dua skenario berbeda** untuk melihat dampak dari **urutan penerapan teknik**:

### 1. **KCC + AE**
- **Skenario 1**: Terapkan **Kendall’s Correlation Coefficient** terlebih dahulu, kemudian lakukan **Autoencoding**.
- **Skenario 2**: Terapkan **Autoencoding** terlebih dahulu, kemudian lakukan seleksi fitur menggunakan **KCC**.

### 2. **KCC + SMOTE**
- **Skenario 1**: Terapkan **Kendall’s Correlation Coefficient** sebelum melakukan oversampling dengan **SMOTE**.
- **Skenario 2**: Terapkan **SMOTE** terlebih dahulu, kemudian lakukan seleksi fitur berbasis **KCC**.

---

Untuk implementasi dan hasil lebih rinci, silakan merujuk pada folder atau notebook terkait yang terdapat dalam direktori ini.

