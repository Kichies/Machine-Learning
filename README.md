# 🛍️ K-Means Clustering: Mall Customer Segmentation

Proyek ini adalah pengerjaan Latihan Mandiri dari modul Praktikum Machine Learning Pertemuan 11. Tujuannya adalah mengimplementasikan algoritma K-Means pada dataset baru secara mandiri untuk melihat pola segmentasi.

## 📝 Deskripsi Proyek
Dataset yang digunakan adalah **Mall Customer Segmentation Data** yang diperoleh dari Kaggle. Model ini dibangun untuk mengelompokkan pelanggan mall ke dalam beberapa segmen berdasarkan dua fitur utama:
* **Annual Income (Pendapatan Tahunan):** Penghasilan pelanggan per tahun dalam satuan ribu dolar.
* **Spending Score (Skor Belanja):** Skor (1-100) yang diberikan oleh pihak mall berdasarkan perilaku pengeluaran pelanggan.

## ⚙️ Tahapan Pemrosesan
1. **Data Loading:** Membaca dataset `Mall_Customers.csv`.
2. **Feature Selection:** Mengambil kolom pendapatan (`Annual Income`) dan skor belanja (`Spending Score`) untuk proses *clustering*.
3. **Data Normalization:** Menggunakan `MinMaxScaler` untuk menyamakan skala fitur agar perhitungan jarak antar titik data lebih akurat.
4. **Pemodelan K-Means:** Melatih model K-Means dengan membaginya ke dalam **5 kluster** (titik optimal standar untuk dataset ini).
5. **Visualisasi:** Menampilkan hasil sebaran 5 kluster dan titik pusat (*centroid*) masing-masing kelompok menggunakan *scatter plot*.

## 📊 Hasil Clustering
Berdasarkan visualisasi data, algoritma K-Means berhasil mengelompokkan pelanggan menjadi 5 segmen perilaku yang berbeda:
1. **Pendapatan Tinggi & Skor Belanja Tinggi** (Target promosi premium)
2. **Pendapatan Tinggi & Skor Belanja Rendah** (Perlu strategi untuk menarik minat belanja)
3. **Pendapatan Menengah & Skor Belanja Menengah** (Pelanggan standar)
4. **Pendapatan Rendah & Skor Belanja Tinggi** (Pelanggan loyal tapi perlu dijaga agar tidak *overspending*)
5. **Pendapatan Rendah & Skor Belanja Rendah** (Bukan target pasar utama)
