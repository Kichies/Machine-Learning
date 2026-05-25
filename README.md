# 📍 K-Means Clustering: GPS Trajectories

[cite_start]Proyek ini merupakan pengerjaan ulang modul Praktikum Machine Learning Pertemuan 11 mengenai implementasi algoritma K-Means Clustering[cite: 16, 18, 22].

## 📝 Deskripsi Proyek
[cite_start]Dataset yang digunakan berasal dari **UCI Machine Learning Repository** yaitu data perjalanan (*GPS trajectories*) yang dikumpulkan dari aplikasi Android Go!Track[cite: 43, 44]. [cite_start]Tujuan dari model ini adalah untuk mengelompokkan data perjalanan ke dalam beberapa kluster berdasarkan kemiripan jarak tempuh (*distance*) dan kecepatan (*speed*)[cite: 68, 70, 23].

## ⚙️ Tahapan Pemrosesan
1. [cite_start]**Data Loading:** Membaca dataset `go_track_tracks.csv`[cite: 59].
2. [cite_start]**Feature Selection:** Menggunakan variabel `distance` dan `speed` untuk proses *clustering*, serta membuang kolom `linha` yang tidak diperlukan[cite: 63, 68, 70].
3. [cite_start]**Data Normalization:** Melakukan standarisasi skala data menggunakan `MinMaxScaler` agar jarak antar titik data pada algoritma K-Means lebih akurat[cite: 95, 96, 97].
4. [cite_start]**Pemodelan K-Means:** Menentukan jumlah kluster (K) sebanyak 3 kelompok dan melatih model menggunakan data yang sudah dinormalisasi[cite: 25, 122, 124].
5. [cite_start]**Visualisasi:** Menampilkan hasil *clustering* beserta titik *centroid* masing-masing kelompok menggunakan *scatter plot*[cite: 149, 153, 160].

## 📊 Hasil Clustering
Model berhasil mengelompokkan data perjalanan ke dalam 3 kluster yang berbeda. [cite_start]Titik merah (X) pada visualisasi merepresentasikan titik pusat (*centroid*) dari masing-masing kelompok, yang menunjukkan rata-rata jarak dan kecepatan pada kluster tersebut[cite: 28].

> **Catatan Koreksi Modul:** Evaluasi performa yang menggunakan `accuracy_score` dan `f1_score` (Supervised Learning) dihilangkan dalam implementasi ini karena K-Means merupakan algoritma *Unsupervised Learning* (tidak memiliki label asli untuk dikomparasi).
