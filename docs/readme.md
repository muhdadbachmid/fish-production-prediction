# README

## Analisis Data Produksi Perikanan (2018-2022)

### Deskripsi

Proyek ini melakukan eksplorasi dan analisis data produksi perikanan dari tahun 2018 hingga 2022. Analisis ini mencakup pemrosesan data, imputasi nilai yang hilang, encoding variabel kategori, normalisasi data, serta penerapan model regresi untuk prediksi produksi tahunan.

### Dataset

- Nama File: produksi2018\_2022.csv
- Kolom:
  - `jenis_ikan`: Nama jenis ikan
  - `Januari - Desember`: Produksi per bulan
  - `Tahun`: Tahun produksi
  - `Total_Produksi_Tahunan`: Jumlah produksi tahunan
  - `Growth_Rate`: Tingkat pertumbuhan produksi
  - `Produksi_Tahun_Lalu`: Produksi pada tahun sebelumnya
  - `jenis_ikan_encoded`: Hasil encoding kategori ikan

### Persyaratan

- Python 3.8+
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

### Langkah Analisis

1. **Eksplorasi Data:**

   - Melihat informasi dasar, statistik deskriptif, dan nilai yang hilang.

2. **Preprocessing:**

   - Mengisi nilai yang hilang dengan median.
   - Encoding variabel kategori (`jenis_ikan`).
   - Normalisasi fitur numerik menggunakan `StandardScaler`.

3. **Modeling:**

   - Menggunakan beberapa model regresi:
     - `LinearRegression`
     - `RandomForestRegressor`
     - `GradientBoostingRegressor`
   - Evaluasi model menggunakan `mean_squared_error` dan `r2_score`.

4. **Validasi Model:**

   - `KFold Cross Validation` dan `GridSearchCV` untuk optimasi parameter.

### Cara Menjalankan

1. Instal dependensi dengan:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
2. Jalankan skrip utama di Jupyter Notebook atau Python.
