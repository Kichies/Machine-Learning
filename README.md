# 📍 K-Means Clustering: GPS Trajectories

Proyek ini merupakan pengerjaan ulang modul Praktikum Machine Learning Pertemuan 11 mengenai implementasi algoritma K-Means Clustering.

## 📝 Deskripsi Proyek
Dataset yang digunakan berasal dari **UCI Machine Learning Repository** yaitu data perjalanan (*GPS trajectories*) yang dikumpulkan dari aplikasi Android Go!Track. Tujuan dari model ini adalah untuk mengelompokkan data perjalanan ke dalam beberapa kluster berdasarkan kemiripan jarak tempuh (*distance*) dan kecepatan (*speed*).

## ⚙️ Tahapan Pemrosesan
1. **Data Loading:** Membaca dataset `go_track_tracks.csv`.
2. **Feature Selection:** Menggunakan variabel `distance` dan `speed` untuk proses *clustering*, serta membuang kolom `linha` yang tidak diperlukan.
3. **Data Normalization:** Melakukan standarisasi skala data menggunakan `MinMaxScaler` agar jarak antar titik data pada algoritma K-Means lebih akurat.
4. **Pemodelan K-Means:** Menentukan jumlah kluster (K) sebanyak 3 kelompok dan melatih model menggunakan data yang sudah dinormalisasi.
5. **Visualisasi:** Menampilkan hasil *clustering* beserta titik *centroid* masing-masing kelompok menggunakan *scatter plot*.

## 📊 Hasil Clustering
Model berhasil mengelompokkan data perjalanan ke dalam 3 kluster yang berbeda. Titik merah (X) pada visualisasi merepresentasikan titik pusat (*centroid*) dari masing-masing kelompok, yang menunjukkan rata-rata jarak dan kecepatan pada kluster tersebut.

> **Catatan Koreksi Modul:** Evaluasi performa yang menggunakan `accuracy_score` dan `f1_score` (Supervised Learning) dihilangkan dalam implementasi ini karena K-Means merupakan algoritma *Unsupervised Learning* (tidak memiliki label asli untuk dikomparasi).
