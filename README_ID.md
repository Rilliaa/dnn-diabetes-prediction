# 🧠 Optimasi Deep Neural Network untuk Prediksi Status Diabetes

![Python](https://img.shields.io/badge/Python-3.9-blue.svg)
![Colab](https://img.shields.io/badge/Google%20Colab-Compatible-orange)
![Status](https://img.shields.io/badge/Thesis-Final-brightgreen)

Proyek ini merupakan tugas akhir (skripsi) sarjana saya yang berfokus pada optimalisasi model Deep Learning untuk memprediksi status diabetes (Normal, Pre-diabetes, Diabetes) berdasarkan data indikator kesehatan. Tujuan utamanya adalah meningkatkan performa model melalui berbagai teknik optimasi, termasuk seleksi fitur, reduksi dimensi, penyeimbangan data, dan mekanisme perhatian (self-attention).

---

## 📊 Ringkasan Dataset

- **Sumber**: [Kaggle – Diabetes Health Indicators Dataset](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset)
- **Jumlah Sampel**: 253.680 baris
- **Fitur**: 21 indikator kesehatan
- **Kelas Target**:
  - 0: Normal
  - 1: Pre-diabetes
  - 2: Diabetes

---

## 🧪 Alur Penelitian

Penelitian dilakukan dalam beberapa tahapan untuk mengevaluasi performa model Deep Neural Network (DNN) dengan berbagai teknik optimasi. Alurnya sebagai berikut:

### 🔹 Tahap 1: Perancangan Penelitian
- Menentukan masalah dan tujuan
- Mengumpulkan dataset
- Melakukan eksplorasi data (EDA)

### 🔹 Tahap 2: Pra-pemrosesan Data
- Memuat dataset (`Dataset.csv`)
- Pembersihan data
- Normalisasi fitur

### 🔹 Tahap 3: Pengembangan Model

Beberapa varian model DNN dikembangkan dan dibandingkan:

#### 🔸 1. Model Dasar (DNN Default)
- Pembagian data stratifikasi (train-test split)
- Melatih DNN tanpa optimasi
- Evaluasi dengan Precision, Recall, F1-Score, ROC-AUC

#### 🔸 2. DNN + Self-Attention
- Menambahkan layer self-attention setelah DNN dasar
- Pembagian data tetap sama
- Evaluasi performa

#### 🔸 3. DNN + Seleksi Fitur (KCC)
- Menerapkan Kendall’s Correlation Coefficient untuk seleksi fitur
- Train-test split pada fitur yang diseleksi
- Melatih dan evaluasi DNN

#### 🔸 4. DNN + SMOTE
- Menerapkan oversampling SMOTE pada data latih
- Melatih dan evaluasi DNN pada data seimbang

#### 🔸 5. DNN + Autoencoder
- Melatih Autoencoder untuk reduksi dimensi non-linear
- Mengekstrak fitur laten dari encoder
- Melatih dan evaluasi DNN dengan fitur yang dikompresi

---

### 🔹 Tahap 4: Kombinasi Teknik Optimasi

Untuk menilai dampak kumulatif, kombinasi teknik berikut diuji:

#### 🔸 DNN dengan 2 Teknik Optimasi
- DNN + KCC + Autoencoder  
- DNN + KCC + Self-Attention  
- DNN + KCC + SMOTE  
- DNN + Autoencoder + Self-Attention  
- DNN + Autoencoder + SMOTE  
- DNN + Self-Attention + SMOTE  

#### 🔸 DNN dengan 3 Teknik Optimasi
- DNN + KCC + Autoencoder + Self-Attention  
- DNN + KCC + Autoencoder + SMOTE  
- DNN + KCC + Self-Attention + SMOTE  
- DNN + Autoencoder + Self-Attention + SMOTE  

#### 🔸 DNN dengan 4 Teknik Optimasi (Model Akhir)
- DNN + KCC + Autoencoder + Self-Attention + SMOTE

---

### 🔹 Tahap 5: Evaluasi dan Interpretasi Akhir
- Semua model dievaluasi dengan metrik klasifikasi standar:
  - Precision
  - Recall
  - F1-Score
  - ROC-AUC

---

## 🛠️ Library yang Digunakan

- Python (Google Colab)
- Scikit-learn
- TensorFlow / Keras
- Imbalanced-learn
- Matplotlib & Seaborn

---

## 📌 Hasil Utama

Penelitian ini bertujuan mengembangkan model Deep Neural Network (DNN) yang dioptimalkan dengan kombinasi teknik seleksi fitur (Kendall’s Correlation Coefficient), reduksi dimensi (Autoencoders), penyeimbangan data (SMOTE), dan mekanisme perhatian (Self-Attention) untuk meningkatkan klasifikasi multikelas status diabetes (Normal, Pre-Diabetes, Diabetes).

Temuan utama sebagai berikut:

1. **Performa Dasar**  
   Model DNN default tanpa optimasi menghasilkan F1-Score sebesar **0.4162** sebagai titik acuan untuk perbandingan selanjutnya.

2. **Teknik Optimasi Individu**  
   - **SMOTE**: Meningkatkan **Recall** secara signifikan (hingga **0.4912**) namun menurunkan **Precision**, menunjukkan adanya trade-off.  
   - **Self-Attention**: Mencapai skor **ROC-AUC tertinggi** (**0.7863**), meningkatkan kemampuan pemisahan kelas meskipun dampaknya pada F1-Score terbatas.  
   - **Autoencoder**: Sedikit meningkatkan **Precision**, namun menurunkan performa metrik lain, menunjukkan bahwa fitur laten kurang optimal.  
   - **Seleksi Fitur KCC**: Meningkatkan efisiensi dan stabilitas model sambil menghindari overfitting, memungkinkan model fokus pada fitur paling relevan.

3. **Kombinasi Teknik Optimasi**  
   - Performa **kuantitatif terbaik** dicapai dengan kombinasi **KCC + SMOTE**, menghasilkan **F1-Score tertinggi sebesar 0.4425**, melampaui baseline di semua metrik utama.  
   - Meskipun kombinasi **KCC + SMOTE + Self-Attention** menghasilkan **rata-rata performa tertinggi** (**0.5235**), model **KCC + SMOTE** dipilih sebagai **model terbaik** karena keseimbangan performa, kesederhanaan, dan efisiensi komputasi.

4. **Insight Interpretabilitas**  
   - **KCC** secara efektif mengidentifikasi fitur yang paling berkorelasi dengan status diabetes, membantu pembelajaran yang lebih fokus.  
   - **SMOTE** secara konsisten meningkatkan Recall dengan memungkinkan model memahami pola kelas minoritas, meskipun Precision cenderung turun.  
   - **Autoencoder**, dalam konteks ini, kurang efektif—kemungkinan karena hilangnya informasi penting saat encoding dan kurang representatif untuk klasifikasi.

---

📄 _Repositori ini mencerminkan puncak dari penelitian skripsi saya di Universitas Muhammadiyah Riau._
