
# Laporan Analisis Data Produksi Perikanan (2018-2022)

## 1. Pendahuluan

Analisis ini bertujuan untuk mengeksplorasi data produksi perikanan dari tahun 2018 hingga 2022 dan membangun model regresi untuk memprediksi produksi tahunan berdasarkan data historis.

## 2. Eksplorasi Data

Dataset yang digunakan memiliki 163 entri dengan berbagai jenis ikan yang diproduksi setiap bulan dari tahun 2018-2022. Beberapa kolom memiliki nilai yang hilang, terutama pada `Growth_Rate` dan `Produksi_Tahun_Lalu`.

## 3. Preprocessing Data

- **Imputasi Nilai Hilang:**
  - Nilai yang hilang pada `Growth_Rate` dan `Produksi_Tahun_Lalu` diisi dengan median untuk mengurangi bias akibat outlier.
- **Encoding:**
  - `jenis_ikan` dikonversi menjadi variabel numerik menggunakan `LabelEncoder`.
- **Normalisasi:**
  - Semua fitur numerik dinormalisasi menggunakan `StandardScaler` untuk meningkatkan performa model.

## 4. Pemodelan

### a) Model yang Digunakan

Tiga model regresi diterapkan untuk memprediksi produksi tahunan:

1. **Linear Regression**
2. **Random Forest Regressor**
3. **Gradient Boosting Regressor**

### b) Evaluasi Model

Model dievaluasi menggunakan `Mean Squared Error (MSE)` dan `R-squared (R²)`. Hasil awal menunjukkan bahwa **Gradient Boosting Regressor** memberikan akurasi terbaik dengan nilai R² tertinggi.

## 5. Kesimpulan

- Model Gradient Boosting memberikan hasil prediksi terbaik.
- Preprocessing data seperti imputasi, encoding, dan normalisasi meningkatkan performa model.
- Analisis lebih lanjut dapat dilakukan dengan menambahkan fitur tambahan atau mencoba model deep learning.
