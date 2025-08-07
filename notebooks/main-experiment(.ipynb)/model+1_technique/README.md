# [EN]

This folder contains experimental implementations where the baseline DNN model is **combined with one additional technique** at a time. The goal is to observe how each method contributes to improving model performance.

## 🔬 Techniques Applied

Each sub-experiment adds **one specific technique** to the baseline model:

- **Feature Selection with Kendall's Tau Correlation Coefficient**  
  To reduce irrelevant or redundant input features by selecting the most statistically correlated attributes.

- **Self-Attention Mechanism**  
  Incorporates an attention layer to help the model focus on more relevant parts of the input dynamically.

- **SMOTE for Imbalanced Data Handling**  
  Synthetic Minority Over-sampling Technique is applied to address class imbalance in the dataset.

- **Dimensionality Reduction with Autoencoders**  
  A pre-trained autoencoder is used to compress high-dimensional input into a more compact, information-rich representation.

## 🎯 Objective

The purpose of this experimentation is to evaluate:
- The impact of each technique when applied individually.
- Whether these enhancements outperform the standalone baseline DNN model.
- Which technique provides the most significant performance improvement.

---

[ID]

## Ringkasan

## 🔬 Teknik yang Digunakan

Setiap eksperimen dalam folder ini menambahkan **satu teknik spesifik** ke model baseline:

- **Seleksi Fitur dengan Korelasi Kendall (Kendall's Tau)**  
  Digunakan untuk mengurangi fitur yang tidak relevan dengan memilih atribut yang memiliki korelasi statistik paling kuat.

- **Mekanisme Self-Attention**  
  Menambahkan lapisan atensi untuk membantu model memfokuskan perhatian secara dinamis pada bagian input yang paling relevan.

- **Penanganan Data Tidak Seimbang dengan SMOTE**  
  Menggunakan *Synthetic Minority Over-sampling Technique* untuk mengatasi ketidakseimbangan kelas dalam dataset.

- **Reduksi Dimensi dengan Autoencoders**  
  Autoencoder yang telah dilatih digunakan untuk memadatkan input berdimensi tinggi menjadi representasi yang lebih ringkas namun tetap informatif.

## 🎯 Tujuan

Tujuan dari eksperimen ini adalah untuk mengevaluasi:
- Dampak dari setiap teknik saat diterapkan secara individual.
- Apakah teknik-teknik ini dapat mengungguli model baseline DNN yang berdiri sendiri.
- Teknik mana yang memberikan peningkatan performa paling signifikan.

