# 📊 KNIME Data Processing & Visualization Workflow

Repository ini berisi workflow KNIME untuk melakukan data preprocessing, analisis, serta visualisasi menggunakan dataset **Cereals.csv**.  
Proyek ini fokus pada pembersihan data, transformasi, eksplorasi, dan interpretasi sederhana terhadap data cereal.

---

## 🚀 Workflow Overview

Tahapan dalam pipeline mencakup:

### 🔧 Data Preparation
1. **CSV Reader** – Import dataset
2. **Column Auto Type Cast** – Adjust tipe data otomatis
3. **Column Filter** – Menyaring kolom yang digunakan
4. **String Manipulation** – Membersihkan data teks
5. **Missing Value Handling** – Menangani nilai kosong
6. **Row Filter** – Memilah baris sesuai kebutuhan
7. **Normalizer** – Menstandarisasi nilai numerik
8. **Column Renamer** – Merapikan nama kolom
9. **Duplicate Row Filter** – Menghapus baris duplikat

### 📊 Data Analysis & Exploration
10. **Linear Correlation** – Mengukur hubungan antar variabel
11. **GroupBy** – Agregasi untuk analisis ringkas

### 📈 Visualisasi
12. **Bar Chart**
13. **Pie Chart**
14. **Scatter Plot**
15. **Histogram**  
(Visualisasi dapat ditambah sesuai kebutuhan analisis)

---

## 📄 Insight yang didapat

Berikut poin utama dari hasil eksplorasi:

- Dataset berhasil dibersihkan dari missing value & duplikat sehingga lebih siap dipakai.
- Normalisasi membantu menstandarisasi nilai numerik untuk visualisasi & analisis yang lebih akurat.
- Korelasi antar variabel dapat terlihat dengan jelas menggunakan **Linear Correlation node**.
- Visualisasi memberikan gambaran distribusi dan hubungan antar fitur sehingga memudahkan interpretasi.
- Chart menunjukkan perbandingan kategori & kecenderungan pola berdasarkan atribut data.

---

## 📁 Struktur File
