[EN]

## Evaluation Results – DNN with Optimization Technique Combinations

This folder contains the **final evaluation results** of all experimental models using combinations of optimization techniques integrated into the DNN pipeline. The metrics recorded include:  
**Precision, Recall, F1-Score, ROC-AUC**, and the **Average of the four metrics (AVG 4)**.

| No  | Model                              | Precision | Recall  | F1-Score | ROC-AUC | Average   | Notes                                     | Experiments |
|-----|------------------------------------|-----------|---------|----------|---------|-----------|-------------------------------------------|-------------|
| 1   | DNN (Default)                      | 0.4608    | 0.4037  | 0.4162   | 0.7765  | 0.5143    | 64, 32, 16 (default architecture)         | 20          |
| 2   | DNN + SA                           | 0.4738    | 0.3883  | 0.3992   | 0.7863  | 0.5119    | -                                         | 1           |
| 3   | DNN + KCC                          | 0.4708    | 0.3930  | 0.4050   | 0.7829  | 0.5129    | -                                         | 1           |
| 4   | DNN + SMOTE                        | 0.4279    | 0.4912  | 0.4153   | 0.7184  | 0.5132    | -                                         | 1           |
| 5   | DNN + AE                           | 0.4639    | 0.3859  | 0.3957   | 0.7737  | 0.5048    | AE-B1                                     | 9           |
| 6   | DNN + KCC + AE                     | 0.4724    | 0.3727  | 0.3777   | 0.7579  | 0.4952    | KCCAEC2_S1                                | 10          |
| 7   | DNN + KCC + SA                     | 0.4768    | 0.3741  | 0.3798   | 0.7822  | 0.5032    | -                                         | 1           |
| 8   | DNN + KCC + SMOTE                  | 0.4368    | 0.4746  | 0.4425   | 0.7332  | 0.5218    | SMOTEKCC_S2                               | 2           |
| 9   | DNN + AE + SA                      | 0.4763    | 0.3702  | 0.3738   | 0.7764  | 0.4992    | Dataset from AE-B1                        | 1           |
| 10  | DNN + AE + SMOTE                   | 0.4284    | 0.4894  | 0.3986   | 0.7339  | 0.5126    | Dataset from AE-B1                        | 1           |
| 11  | DNN + SA + SMOTE                   | 0.4294    | 0.4892  | 0.4126   | 0.7172  | 0.5121    | -                                         | 1           |
| 12  | DNN + KCC + AE + SA                | 0.4731    | 0.3722  | 0.3769   | 0.7572  | 0.4949    | Dataset from KCCAEC2_S1                   | 1           |
| 13  | DNN + KCC + AE + SMOTE              | 0.4337    | 0.4831  | 0.4058   | 0.7448  | 0.5169    | Dataset from KCCAEC2_S1                   | 1           |
| 14  | DNN + KCC + SA + SMOTE              | 0.4392    | 0.4835  | 0.4413   | 0.7300  | 0.5235    | -                                         | 1           |
| 15  | DNN + AE + SA + SMOTE               | 0.4306    | 0.4899  | 0.4110   | 0.7312  | 0.5157    | Dataset from AE-B1                        | 1           |
| 16  | DNN + KCC + AE + SMOTE + SA         | 0.4380    | 0.4843  | 0.4067   | 0.7473  | 0.5191    | Dataset from KCCAEC2_S1                   | 1           |

|                                            Summary                                          |
| Metric                     | Precision | Recall  | F1-Score | ROC-AUC | Average (4 Metrics) |
|----------------------------|-----------|---------|----------|---------|---------------------|
| Average Across Models      | 0.4517    | 0.4346  | 0.4042   | 0.7532  | 0.5109              |
| Models Surpassing Default  | 7         | 8       | 2        | 3       | 5                   |


---

[ID]

## Hasil Evaluasi - DNN dengan kombinasi teknik optimasi

Folder ini berisi hasil evaluasi keseluruhan konfigurasi eksperimen yang telah di uji, dengan metrik utama Precision, Recall, F1-Score, ROC-AUC dan skor rata rata. 

| No  | Model                              | Precision | Recall  | F1-Score | ROC-AUC | Rata-Rata | Notes                             | Experiments |
|-----|------------------------------------|-----------|---------|----------|---------|-----------|-----------------------------------|-------------|
| 1   | DNN (Default)                      | 0.4608    | 0.4037  | 0.4162   | 0.7765  | 0.5143    | 64, 32, 16 (arsitektur default)   | 20          |
| 2   | DNN + SA                           | 0.4738    | 0.3883  | 0.3992   | 0.7863  | 0.5119    | -                                 | 1           |
| 3   | DNN + KCC                          | 0.4708    | 0.3930  | 0.4050   | 0.7829  | 0.5129    | -                                 | 1           |
| 4   | DNN + SMOTE                        | 0.4279    | 0.4912  | 0.4153   | 0.7184  | 0.5132    | -                                 | 1           |
| 5   | DNN + AE                           | 0.4639    | 0.3859  | 0.3957   | 0.7737  | 0.5048    | AE-B1                             | 9           |
| 6   | DNN + KCC + AE                     | 0.4724    | 0.3727  | 0.3777   | 0.7579  | 0.4952    | KCCAEC2_S1                        | 10          |
| 7   | DNN + KCC + SA                     | 0.4768    | 0.3741  | 0.3798   | 0.7822  | 0.5032    | -                                 | 1           |
| 8   | DNN + KCC + SMOTE                  | 0.4368    | 0.4746  | 0.4425   | 0.7332  | 0.5218    | SMOTEKCC_S2                       | 2           |
| 9   | DNN + AE + SA                      | 0.4763    | 0.3702  | 0.3738   | 0.7764  | 0.4992    | Dataset dari AE-B1                | 1           |
| 10  | DNN + AE + SMOTE                   | 0.4284    | 0.4894  | 0.3986   | 0.7339  | 0.5126    | Dataset dari AE-B1                | 1           |
| 11  | DNN + SA + SMOTE                   | 0.4294    | 0.4892  | 0.4126   | 0.7172  | 0.5121    | -                                 | 1           |
| 12  | DNN + KCC + AE + SA                | 0.4731    | 0.3722  | 0.3769   | 0.7572  | 0.4949    | Dataset dari KCCAEC2_S1           | 1           |
| 13  | DNN + KCC + AE + SMOTE              | 0.4337    | 0.4831  | 0.4058   | 0.7448  | 0.5169    | Dataset dari KCCAEC2_S1           | 1           |
| 14  | DNN + KCC + SA + SMOTE              | 0.4392    | 0.4835  | 0.4413   | 0.7300  | 0.5235    | -                                 | 1           |
| 15  | DNN + AE + SA + SMOTE               | 0.4306    | 0.4899  | 0.4110   | 0.7312  | 0.5157    | Dataset dari AE-B1                | 1           |
| 16  | DNN + KCC + AE + SMOTE + SA         | 0.4380    | 0.4843  | 0.4067   | 0.7473  | 0.5191    | Dataset dari KCCAEC2_S1           | 1           |

|                                         Kesimpulan                                          |
| Metril                     | Precision | Recall  | F1-Score | ROC-AUC | Average (4 Metrics) |
|----------------------------|-----------|---------|----------|---------|---------------------|
| Rata Rata seluruh Model    | 0.4517    | 0.4346  | 0.4042   | 0.7532  | 0.5109              |
| Model yang melewati Default| 7         | 8       | 2        | 3       | 5                   |

---
