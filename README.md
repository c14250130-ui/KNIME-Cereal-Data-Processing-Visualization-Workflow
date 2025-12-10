# 🥣 Cereal Dataset Analysis using KNIME

Project ini bertujuan untuk melakukan preprocessing dan visualisasi data dari dataset cereal menggunakan KNIME.  
Visualisasi dibuat untuk memahami hubungan nutrisi antar produk sereal, distribusi data, dan pola pada fitur nutrisi.

---

## 🔁 Workflow Overview

![Workflow](link-gambar-workflow)

### Node Flow

1. CSV Reader  
2. Column Filter  
3. Missing Value  
4. Normalizer  
5. Duplicate Row Filter  
6. Branch Visualisasi  
   - Linear Correlation → Heatmap  
   - Scatter Plot  
   - Histogram  
   - Box Plot  
   - Column Filter (categorical) → Pie Chart  
   - GroupBy → Bar Chart  

---

## 🔧 Data Processing Steps

| Step | Node | Fungsi |
|---|---|---|
|1|CSV Reader|Load data cereal (.csv)|
|2|Column Filter|Memilih kolom yang dibutuhkan|
|3|Missing Value|Menangani nilai kosong|
|4|Normalizer|Normalisasi fitur numerik|
|5|Duplicate Row Filter|Menghapus data duplikat|
|6|Linear Correlation|Menghitung korelasi antar fitur|
|7|Group By|Mengelompokkan data untuk Bar Chart|
|8|Visualization|Heatmap, Scatter, Histogram, Boxplot, Pie, Bar|

---

## 📊 Visualizations & Explanation

### 🔥 Heatmap (Correlation Matrix)
Melihat hubungan antar kolom numerik.  
Semakin kuat warna, semakin tinggi nilai korelasinya.

![Heatmap](link-gambar-heatmap)

---

### ✴ Scatter Plot
Untuk melihat hubungan dua variabel, misalnya sugar vs rating.

![Scatter](link-gambar-scatter)

---

### 📈 Histogram
Menampilkan distribusi nilai (contoh: sugar, calories, rating).

![Histogram](link-gambar-histogram)

---

### 📦 Box Plot
Menunjukkan persebaran data dan outlier.

![Boxplot](link-gambar-boxplot)

---

### 📊 Bar Chart (GroupBy)
Menampilkan nilai rata-rata nutrisi berdasarkan kategori (manufacturer/type).

![Bar Chart](link-gambar-barchart)

---

### 🥧 Pie Chart
Menunjukkan proporsi kategori — contoh distribusi tipe cereal.

![Pie Chart](link-gambar-piechart)

---

## 📌 Insight

- Kandungan **sugar dan carbo memiliki hubungan kuat**, ditunjukkan pada scatter & korelasi.
- Variasi nilai nutrisi cukup besar, terutama pada **calories, sugar, dan carbo**.
- Boxplot menunjukkan terdapat **outlier pada beberapa nutrisi**.
- Manufacturer/type tertentu punya rata-rata nutrisi yang berbeda (dari bar chart).
- Scatter plot memberi gambaran pola hubungan antar variabel.

---

## 📍 Kesimpulan

- Dataset cereal memiliki keragaman nutrisi yang cukup besar antar produk.
- Visualisasi membantu memahami pola nutrisi dan dapat digunakan untuk rekomendasi produk sehat.
- Workflow ini bisa dikembangkan untuk **clustering, prediction model, atau recommender** pada tahap selanjutnya.

---

