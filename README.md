# 📊 Analisis Data Cereal Dataset Menggunakan KNIME

Repository ini berisi workflow KNIME untuk melakukan proses **Data Preparation**, **Data Processing**, dan **Visualisasi Data** pada dataset *Cereals.csv*.  
Tujuan utama project ini adalah mempraktikkan tahapan analisis data mulai dari membaca dataset, pembersihan data, transformasi, hingga visualisasi insight menggunakan KNIME.

---

## 🗂 Dataset
Dataset yang digunakan: **Cereals.csv**  
Berisi informasi mengenai berbagai jenis sereal beserta nilai gizi seperti Kalori, Protein, Lemak, Gula, Sodium, dan lainnya.

---

## 🔧 Tools yang digunakan
- **KNIME Analytics Platform** versi 5.8.0
- Node–node untuk data cleaning, preparation, statistical analysis & visualization

---

## 🏗 Workflow KNIME

Tahapan node yang digunakan (15+ node):

| No | Node | Fungsi |
|---|-------------------------|--------------------------------------------|
|1| CSV Reader | Membaca dataset |
|2| Column Auto Type Cast | Menyesuaikan tipe data otomatis |
|3| Column Filter | Memilih / buang kolom tertentu |
|4| Missing Value | Menangani data kosong (mean/median/mode) |
|5| Row Filter | Menyaring baris sesuai kriteria |
|6| Normalizer | Menormalkan nilai numerik |
|7| Column Rename | Merapikan nama kolom |
|8| Duplicate Row Filter | Menghapus data duplikat |
|9| Linear Correlation | Melihat korelasi antar fitur |
|10| GroupBy | Menghitung statistik agregat |
|11| Bar Chart | Visualisasi distribusi sereal |
|12| Pie Chart | Visualisasi proporsi kategori |
|13| Scatter Plot | Analisis hubungan antar variabel |
|14| Histogram | Distribusi fitur numerik |
|15| Data to Report / Export | Menyimpan hasil untuk laporan |

---

## 📈 Visualisasi yang dihasilkan

✔ Bar Chart — perbandingan nilai numerik antar sereal  
✔ Pie Chart — proporsi kategori (misal rating atau brand)  
✔ Scatter Plot — hubungan antar variabel nutrisi  
✔ Histogram — distribusi nilai pada fitur numerik  

Semua grafik digunakan untuk melihat pola, sebaran dan insight dari data.

---

## 🔍 Insight & Interpretasi

Berdasarkan hasil analisis:

- Tidak ditemukan missing value setelah dilakukan cleaning
- Normalisasi membantu membuat skala nutrisi lebih seragam
- Korelasi antar fitur membantu melihat hubungan seperti:
  - Kandungan gula cenderung berbanding lurus dengan kalori
  - Protein dan fiber berkontribusi pada sereal yang lebih sehat
- Scatter plot menunjukkan pola pengelompokan berdasarkan gizi
- Pie chart & bar chart membantu memahami distribusi nutrisi

---

## 📌 Kesimpulan

Workflow berhasil berjalan dengan baik dan menghasilkan insight berupa:

- Komposisi nutrisi antar sereal cukup bervariasi
- Fitur nutrisi tertentu saling berkaitan dan dapat dianalisis lebih lanjut
- Visualisasi membantu memahami data sebelum modeling

Workflow dapat dikembangkan lebih jauh dengan:

📍 Clustering (K-Means)  
📍 Classification (Decision Tree / Random Forest)  
📍 Feature Engineering lanjut  

---

## 📎 Cara Menjalankan

1. Buka **KNIME 5.8.0**
2. Import workflow
3. Jalankan node satu per satu atau klik **Execute All**
4. Buka view pada node visualisasi untuk melihat grafik


Silakan langsung **copy paste ke README.md** 🚀
Kalau kamu mau ditambah gambar workflow, badge GitHub, atau bagian tambahan lain tinggal bilang ya 😄
