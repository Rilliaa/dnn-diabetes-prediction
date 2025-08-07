[EN]

## 🧩 Baseline Experiment – Seed and Architecture Exploration

This step contains the **baseline experiment** that serves as the foundation for selecting the optimal deep neural network (DNN) configuration for seed classification tasks.

## 🧪 Purpose

The goal of this baseline experiment is to establish a reliable starting point for model development by conducting two key explorations:

1. **Seed Exploration**  
   The first phase involves testing various random seeds using a fixed, suggested DNN architecture. This step aims to identify the seed that consistently produces the best model performance.

2. **Architecture Exploration**  
   Once the best-performing seed is identified, it will be used to evaluate multiple architectural variations. This allows for a fair comparison and selection of the most effective model architecture.

By separating the influence of randomness (seed) and structural design (architecture), this two-step exploration ensures that the final model is built on a solid, data-driven baseline.

## ⚙️ Process Overview

1. **Step 1 – Seed Exploration**  
   - Uses the suggested DNN structure as illustrated in the `suggested_dnn-arch_pattern.png`:  
     `Input(21) → Hidden1(64) → Hidden2(32) → Hidden3(16) → Output(3)`
   - Tests a range of random seeds.
   - Identifies the seed that achieves the most consistent and optimal performance.

2. **Step 2 – Architecture Exploration**  
   - Uses the best seed from Step 1.
   - Compares a set of predefined DNN architectures as illustrated in the `dnn_exploration_patterns`.
   - Determines whether the originally suggested architecture is already optimal, or if improvements can be made.

---

[ID]

## 🧩 Eksperimen Baseline – Eksplorasi Seed dan Arsitektur

Langkah ini memuat **eksperimen baseline** yang berfungsi sebagai fondasi awal dalam proses pemilihan konfigurasi jaringan saraf tiruan (DNN) yang optimal untuk tugas klasifikasi benih.

## 🧪 Tujuan

Tujuan dari eksperimen baseline ini adalah untuk membangun titik awal yang kuat dan dapat diandalkan dalam pengembangan model, melalui dua tahapan eksplorasi utama:

1. **Eksplorasi Seed**  
   Tahapan pertama dilakukan dengan menguji berbagai nilai seed acak menggunakan arsitektur DNN yang telah disarankan. Langkah ini bertujuan untuk mengidentifikasi seed yang secara konsisten menghasilkan performa model terbaik.

2. **Eksplorasi Arsitektur**  
   Setelah seed terbaik diperoleh, eksplorasi dilanjutkan dengan mengevaluasi berbagai variasi arsitektur jaringan. Ini memungkinkan perbandingan yang adil dan pemilihan arsitektur model yang paling efektif.

Dengan memisahkan pengaruh dari elemen acak (*seed*) dan desain struktural (*arsitektur*), pendekatan dua tahap ini memastikan bahwa model akhir dibangun berdasarkan baseline yang solid dan berbasis data.

## ⚙️ Gambaran Proses

1. **Langkah 1 – Eksplorasi Seed**  
   - Menggunakan struktur DNN yang disarankan, seperti pada gambar `suggested_dnn-arch_pattern.png`:  
     `Input(21) → Hidden1(64) → Hidden2(32) → Hidden3(16) → Output(3)`
   - Menguji berbagai nilai seed.
   - Mengidentifikasi seed yang memberikan hasil performa paling optimal dan konsisten.

2. **Langkah 2 – Eksplorasi Arsitektur**  
   - Menggunakan seed terbaik dari Langkah 1.
   - Membandingkan berbagai arsitektur DNN yang telah didefinisikan, seperti yang digambarkan dalam `dnn_exploration_patterns`.
   - Menentukan apakah arsitektur awal yang disarankan sudah optimal, atau masih bisa ditingkatkan.


