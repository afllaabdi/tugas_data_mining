# tugas_data_mining
Indonesia Food Price Prediction (WFP Dataset)
Proyek ini bertujuan untuk menganalisis dan memprediksi harga komoditas pangan di berbagai pasar di Indonesia menggunakan data historis dari World Food Programme (WFP). Proyek ini mencakup alur kerja data science lengkap, mulai dari pembersihan data hingga evaluasi model menggunakan algoritma Random Forest.

-Dataset Overview
Dataset yang digunakan adalah wfp_food_prices_idn.csv yang berisi informasi:
Waktu: Tanggal pengambilan data (tahun dan bulan).
Lokasi: Provinsi (admin1), Kota/Kabupaten (admin2), dan Nama Pasar.
Komoditas: Kategori pangan (misal: sereal, daging) dan nama barang (misal: beras, telur).
Harga: Harga dalam mata uang lokal (IDR) dan USD.

-Alur Kerja (Pipeline)
1. Preprocessing & Data Cleaning
Menghapus baris metadata (header ganda).
Mengonversi tipe data date ke format datetime.
Menangani missing values dan data duplikat untuk memastikan integritas model.
Mengonversi kolom target price menjadi tipe numerik.

2. Feature Engineering & Selection
Ekstraksi Waktu: Mengambil fitur year dan month dari kolom tanggal.
Seleksi Fitur: Memilih fitur relevan seperti admin1, market, category, dan commodity sebagai prediktor.

4. Data Transformation
Label Encoding: Mengubah data kategorikal (nama pasar, lokasi, jenis barang) menjadi format numerik agar dapat diproses oleh algoritma Machine Learning.

5. Analisis & Visualisasi
Matriks Korelasi: Melihat hubungan antar fitur.
Distribusi Harga: Memahami persebaran harga komoditas.
Trend Analisis: Melihat fluktuasi rata-rata harga berdasarkan bulan.

5. Modeling & Evaluasi
Menggunakan algoritma Random Forest Regressor dengan pembagian data 80% pelatihan dan 20% pengujian.
Metrik Performa:
MAE (Mean Absolute Error): Mengukur rata-rata kesalahan absolut dalam prediksi harga.
R² Score: Mengukur sejauh mana model dapat menjelaskan varians data.

-Hasil Prediksi
Berdasarkan eksperimen terakhir, model menunjukkan performa yang sangat tinggi:
MAE: ~894.58 (Rata-rata selisih prediksi dengan harga asli).
R² Score: ~0.9958 (Akurasi model sangat mendekati sempurna).
