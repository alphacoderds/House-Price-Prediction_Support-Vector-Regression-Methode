# House-Price-Prediction_Support-Vector-Regression-Methode
# 🏠 USA Housing Price Analysis

Notebook ini berisi **eksplorasi data** dan **pemodelan harga rumah** pada dataset USA Housing menggunakan Python.  
Proyek ini dibuat untuk tujuan **pembelajaran pribadi**.

## 📚 Deskripsi Proyek

- Membaca dataset `USA_Housing.csv` dan melakukan eksplorasi data awal.
- Pembersihan data & ekstraksi fitur alamat (state/region).
- Analisis deskriptif dan visualisasi distribusi variabel.
- Analisis hubungan (korelasi) antar variabel terhadap harga rumah.
- Membangun model prediksi harga rumah menggunakan **Support Vector Regressor (SVR)**.
- Hyperparameter tuning menggunakan GridSearchCV.

## 🛠️ Library yang Digunakan

- pandas, numpy
- matplotlib, seaborn, missingno
- scikit-learn (train_test_split, MinMaxScaler, SVR, GridSearchCV)
- scipy.stats

## 📝 Langkah Utama

1. **Import Library & Load Data**  
   Membaca file `USA_Housing.csv` dan menampilkan informasi awal dataset.

2. **Eksplorasi Data**  
   - Menampilkan head/tail data.
   - Informasi tipe data (`.info()`).
   - Statistik deskriptif (`.describe()`).

3. **Pembersihan & Transformasi**  
   - Ekstraksi kolom `Address` menjadi kode negara bagian.
   - Menghapus outlier.
   - Normalisasi fitur numerik dengan `MinMaxScaler`.

4. **Visualisasi**  
   - Histogram, boxplot, dan countplot untuk distribusi variabel.
   - Pairplot dan heatmap untuk korelasi antar variabel.
   - Plot bivariate untuk hubungan fitur terhadap harga rumah.

5. **Pemodelan & Evaluasi**  
   - Membagi data train & test.
   - Melatih model SVR (linear dan RBF kernel).
   - Hyperparameter tuning menggunakan GridSearchCV.
   - Evaluasi performa model dengan MAE, MSE, RMSE, dan R².
   - Visualisasi hasil prediksi (actual vs predicted).

## 🚀 Cara Menjalankan Notebook

1. Buka di Google Colab atau Jupyter Notebook.
2. Pastikan semua library sudah terinstal:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn missingno
