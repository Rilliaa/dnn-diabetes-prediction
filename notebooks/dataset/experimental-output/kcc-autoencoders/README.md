
# 🧠 KCC-Based Feature Selection – Autoencoder Outputs

## 🌐 [EN] – Description

This folder contains **9 processed datasets**, each representing the output of an autoencoder trained on features selected using **Kendall’s Correlation Coefficient (KCC)**. This experiment applies a statistical filter method to reduce feature redundancy by analyzing pairwise correlations using Kendall's Tau.

After calculating the Kendall Tau correlation matrix, we applied a threshold based on the **mean of absolute Tau values**, which led to the selection of **9 features** from the original dataset. Due to this dimensionality reduction, each autoencoder architecture was adjusted accordingly to match the new input size.

### 🔧 Architectural Configurations

Each dataset corresponds to one of the following autoencoder architectures:

| Model | Input | Encode1 | Encode2 | Latent | Decode1 | Decode2 | Output |
|-------|--------|----------|----------|--------|----------|----------|--------|
| A1    | 9      | 8        | 7        | 5      | 7        | 8        | 9      |
| A2    | 9      | 8        | 6        | 4      | 6        | 8        | 9      |
| A3    | 9      | 8        | 5        | 3      | 5        | 8        | 9      |
| B1    | 9      | 7        | 6        | 4      | 6        | 7        | 9      |
| B2    | 9      | 7        | 5        | 3      | 5        | 7        | 9      |
| B3    | 9      | 7        | 4        | 2      | 4        | 7        | 9      |
| C1    | 9      | 6        | 5        | 4      | 5        | 6        | 9      |
| C2    | 9      | 6        | 4        | 3      | 4        | 6        | 9      |
| C3    | 9      | 6        | 3        | 2      | 3        | 6        | 9      |

Each model is symmetrical and follows a compression-reconstruction pattern. The variation in latent dimension allows for evaluating the effect of compression strength on downstream DNN performance.

---

## 🇮🇩 [ID] – Deskripsi

Folder ini berisi **9 dataset hasil praproses**, yang masing-masing merupakan keluaran dari autoencoder yang dilatih menggunakan fitur-fitur yang telah dipilih dengan metode **Kendall’s Correlation Coefficient (KCC)**. Eksperimen ini menggunakan pendekatan statistik untuk menyaring fitur dengan cara mengukur korelasi antar fitur berdasarkan nilai Tau Kendall.

Setelah diperoleh matriks korelasi Tau, ambang batas ditentukan menggunakan **rata-rata dari nilai absolut Tau**, yang kemudian menghasilkan **9 fitur terpilih** dari dataset awal. Karena ukuran input berkurang, arsitektur autoencoder pun disesuaikan agar cocok dengan dimensi baru tersebut.

### 🔧 Konfigurasi Arsitektur

Setiap dataset mewakili salah satu dari arsitektur autoencoder berikut:

| Model | Input | Encode1 | Encode2 | Latent | Decode1 | Decode2 | Output |
|-------|--------|----------|----------|--------|----------|----------|--------|
| A1    | 9      | 8        | 7        | 5      | 7        | 8        | 9      |
| A2    | 9      | 8        | 6        | 4      | 6        | 8        | 9      |
| A3    | 9      | 8        | 5        | 3      | 5        | 8        | 9      |
| B1    | 9      | 7        | 6        | 4      | 6        | 7        | 9      |
| B2    | 9      | 7        | 5        | 3      | 5        | 7        | 9      |
| B3    | 9      | 7        | 4        | 2      | 4        | 7        | 9      |
| C1    | 9      | 6        | 5        | 4      | 5        | 6        | 9      |
| C2    | 9      | 6        | 4        | 3      | 4        | 6        | 9      |
| C3    | 9      | 6        | 3        | 2      | 3        | 6        | 9      |

Masing-masing arsitektur bersifat simetris dan mengikuti pola kompresi-rekonstruksi. Perbedaan pada dimensi laten digunakan untuk mengevaluasi pengaruh tingkat kompresi terhadap performa model DNN selanjutnya.

---

📂 **[Access the Dataset Folder](https://drive.google.com/drive/folders/1qnq86mfufNfAhEOC103wNAQiefxuS5xr?usp=sharing)**
