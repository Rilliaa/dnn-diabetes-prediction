[EN]
# DNN Model with 4 Techniques

This stage, **`model+4_techniques`**, represents the last  experimental configuration in this project.

## 📂 Optimization Flow

After preprocessing the dataset, the following sequence of techniques is applied:

1. **Kendall’s Correlation Coefficient (KCC)**  
   Used for feature selection based on a threshold of **mean absolute tau** value.
2. **Autoencoder (AE)**  
   Applied to reduce the dimensionality of the selected features. The AE architecture is based on the **best-performing setup** from previous dual-technique experiments.
3. **SMOTE**  
   Used to balance the class distribution of the reduced feature space before training.
4. **Self-Attention Layer**  
   Integrated into the DNN architecture to enhance feature interaction learning.

---

## 📝 Notes

- The Autoencoder used here is **predefined and pretrained** based on previous experimental results involving two techniques.
- This represents the **final and most optimized stage** of the project’s modeling pipeline.

---

[ID]

# Model DNN dengan Kombinasi 4 Teknik

Tahap ini, **`model+4_techniques`**, merupakan konfigurasi eksperimen paling lengkap dan akhir dari proyek ini.
## 📂 Alur Optimasi

Setelah proses **preprocessing**, langkah-langkah berikut diterapkan secara berurutan:

1. **Kendall’s Correlation Coefficient (KCC)**  
   Digunakan untuk seleksi fitur berdasarkan ambang batas **rata-rata nilai absolut tau**.
2. **Autoencoder (AE)**  
   Diterapkan untuk mereduksi dimensi dari fitur-fitur yang terpilih. Arsitektur AE mengacu pada **hasil terbaik** dari eksperimen dua teknik sebelumnya.
3. **SMOTE**  
   Digunakan untuk menyeimbangkan distribusi kelas dari fitur hasil reduksi sebelum pelatihan model.
4. **Self-Attention Layer**  
   Ditambahkan ke dalam arsitektur DNN untuk meningkatkan pembelajaran interaksi antar fitur.

---

## 📝 Catatan

- Autoencoder yang digunakan sudah **didefinisikan dan dilatih sebelumnya** berdasarkan eksperimen terbaik dari kombinasi dua teknik.
- Ini adalah tahap modeling yang **paling optimal dan menyeluruh** dalam proyek ini.

---
