# 📊 Laporan Analisis dan Pengolahan Data Cereal Menggunakan KNIME

## BAB I  
### 1.1 Latar Belakang  
Analisis data diperlukan untuk memahami karakteristik nutrisi pada berbagai jenis sereal. Dengan memanfaatkan KNIME, proses data preparation, data cleaning, dan visualisasi dapat dilakukan lebih sistematis. Proyek ini bertujuan melakukan pengolahan data menggunakan node-node KNIME serta menghasilkan insight berupa hubungan nutrisi antar produk sereal.

### 1.2 Tujuan  
1. Melakukan preprocessing dataset sereal.  
2. Menganalisis pola dan hubungan antar fitur nutrisi.  
3. Menghasilkan visualisasi sebagai bentuk interpretasi data.  

---

## BAB II – Metodologi

### 2.1 Data dan Tools  
- Dataset : `Cereals.csv`  
- Software : KNIME Analytics Platform 5.8.0  
- Tipe analisis : Preprocessing, Exploratory Analysis, Visualization  

---

## BAB III – Tahapan Workflow KNIME

### 3.1 Node 1 – CSV Reader  
Membaca dataset sumber dengan format `.csv` dan memasukkannya ke workflow.

### 3.2 Node 2 – Column Auto Type Cast  
Mengubah tipe data otomatis (string → integer/float jika memungkinkan) agar operasi statistik berjalan lancar.

### 3.3 Node 3 – Column Filter  
Menentukan kolom mana yang akan digunakan/diabaikan sesuai kebutuhan analisis.

### 3.4 Node 4 – Missing Value  
Menangani nilai kosong/missing dengan metode imputasi (mean/median) sehingga dataset menjadi bersih.

### 3.5 Node 5 – Row Filter  
Menyaring baris berdasarkan kondisi tertentu, misal memilih baris dengan nilai nutrisi tertentu atau menghapus baris yang tidak relevan.

### 3.6 Node 6 – Normalizer  
Menormalkan data numerik agar skala antar fitur seragam (0–1), membantu analisis dan visualisasi lebih objektif.

### 3.7 Node 7 – Column Rename  
Mengubah nama kolom agar lebih ringkas dan mudah digunakan pada proses berikutnya.

### 3.8 Node 8 – Duplicate Row Filter  
Menghilangkan data duplikat berdasarkan seluruh kolom sehingga mencegah bias pada analisis.

### 3.9 Node 9 – Linear Correlation  
Menghitung korelasi antar variabel numerik dan menghasilkan skor hubungan antar fitur nutrisi.

### 3.10 Node 10 – GroupBy  
Melakukan agregasi data (mean, sum, count) untuk melihat ringkasan nutrisi dan statistik per kategori sereal.

### 3.11 Node 11 – Bar Chart  
Menampilkan grafik batang untuk membandingkan nilai nutrisi antar produk sereal.

### 3.12 Node 12 – Pie Chart  
Visualisasi proporsi kategori untuk melihat kontribusi tiap kelompok (misal rating atau brand tertentu).

### 3.13 Node 13 – Scatter Plot  
Menganalisis hubungan antar variabel, misalnya Kalori vs Gula untuk mengetahui pola kesehatan sereal.

### 3.14 Node 14 – Histogram  
Menampilkan distribusi nilai fitur numerik seperti sugar, calories, fat. Berguna untuk melihat penyebaran data.

### 3.15 Node 15 – Data/Report Output  
Output akhir berupa tabel atau laporan visual untuk dokumentasi dan interpretasi hasil.

---

## BAB IV – Hasil dan Insight

### 4.1 Temuan Analisis
- Setelah cleaning, dataset bebas missing value dan duplikat.  
- Normalisasi membuat fitur nutrisi lebih mudah dibandingkan.  
- Korelasi menunjukkan hubungan signifikan antar nutrisi tertentu.  
- Scatter plot mengindikasikan semakin besar gula ➜ semakin tinggi kalori.  
- Histogram menunjukkan distribusi nutrisi tidak merata, beberapa sereal sangat tinggi gula.  

### 4.2 Interpretasi  
Sereal dengan nutrisi seimbang (protein & fiber tinggi, gula rendah) lebih sehat. Sedangkan sereal dengan kandungan gula tinggi dapat memiliki kalori lebih besar. Informasi ini penting untuk rekomendasi nutrisi.

---

## BAB V – Kesimpulan
Workflow KNIME berhasil menerapkan rangkaian preprocessing dan visualisasi. Data dapat dianalisis secara eksploratif untuk menemukan pola nutrisi antar sereal.  
Project dapat dikembangkan dengan metode lanjutan seperti:

- Clustering sereal berdasarkan komposisi gizi  
- Klasifikasi sereal sehat & tidak sehat  
- Recommendation system untuk pilihan sarapan  


