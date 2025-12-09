# **LAPORAN ANALISIS DATA CEREAL MENGGUNAKAN KNIME**

## **1. Pendahuluan**

Proyek ini dilakukan untuk memenuhi tugas UAS dengan tujuan membangun workflow analisis dan pengolahan data pada dataset **Cereal** menggunakan KNIME.  
Tahapan meliputi *data cleaning, preprocessing, eksplorasi data, visualisasi, hingga pembuatan insight berbasis grafik*.  
Workflow dikerjakan end-to-end mulai dari input data hingga interpretasi hasil analisis.

---

## **2. Dataset**

Dataset berisi informasi nutrisi pada berbagai sereal, meliputi:

- Calories
- Protein
- Fat
- Sodium
- Fiber
- Carbohydrate
- Sugars
- Potassium
- Vitamins
- Rating

Dataset diimport menggunakan node **CSV Reader**.

---

## **3. KNIME Workflow**

Berikut alur utama proses pada KNIME:

1. **CSV Reader** — Mengimpor dataset.
2. **Column Auto Type Cast** — Menyesuaikan tipe data otomatis.
3. **Missing Value** — Mengatasi data kosong dengan imputasi.
4. **Column Filter** — Memilih kolom yang diperlukan.
5. **Duplicate Row Filter** — Menghapus data duplikat.
6. **Row Filter** — Menyaring data sesuai kebutuhan analisis.
7. **Normalizer** — Menormalkan data numerik.
8. **Column Rename** — Menjadikan nama kolom lebih ringkas.
9. **Linear Correlation** — Mengukur hubungan antar variabel numerik.
10. **GroupBy** — Menghasilkan statistik agregasi per kolom.
11. **Scatter Plot** — Melihat hubungan antar variabel.
12. **Bar Chart** — Membandingkan nilai nutrisi antar sereal.
13. **Pie Chart** — Visual proporsi kategori.
14. **Histogram** — Melihat penyebaran nilai nutrisi.
15. **Output Table / Report View** — Menampilkan hasil akhir.

---

## **4. Hasil & Insight**

### **4.1 Korelasi Nutrisi**
- Variabel **Sugars dan Calories memiliki korelasi cukup kuat**, menunjukkan bahwa sereal dengan gula tinggi cenderung memiliki kalori lebih besar.
- Variables nutrisi seperti **Fiber dan Protein berkontribusi terhadap rating sereal yang lebih baik**.

### **4.2 Visualisasi dan Temuan**
- **Histogram** memperlihatkan distribusi gula tidak merata, banyak sereal memiliki kadar gula tinggi.
- **Scatter Plot** menunjukkan pola positif antara kalori dan gula.
- **Pie Chart** menggambarkan penyebaran kategori rating sereal.
- **Bar Chart** membantu membandingkan nutrisi antar merk/seri.

Interpretasi:  
➡ Sereal rendah gula dan tinggi serat lebih direkomendasikan untuk konsumsi harian.  
➡ Kandungan gula menjadi indikator penting dalam menentukan kesehatan produk.

---

## **5. Kesimpulan**

Dari workflow KNIME yang dibangun, diperoleh hasil:

- Data berhasil dibersihkan dari missing value dan duplicate.
- Visualisasi memberikan gambaran pola nutrisi antar sereal.
- Hubungan antar variabel nutrisi dapat dianalisis melalui korelasi.
- Pemrosesan berbasis KNIME mempermudah analisis data secara modular dan terstruktur.

Proyek ini menunjukkan bahwa KNIME merupakan tools yang efektif untuk data cleaning, visual, dan analisis statistik ringan.

---

## **6. Dokumentasi Workflow & Output Visualisasi**

### 📂 Workflow KNIME
![Workflow](https://github.com/c14250130-ui/KNIME-Cereal-Data-Processing-Visualization-Workflow/blob/main/workflow.png)

### 📄 CSV Reader & Data Preview
![CSV Reader](https://raw.githubusercontent.com/c14250130-ui/KNIME-Cereal-Data-Processing-Visualization-Workflow/main/Screenshot%202025-12-09%20074019.png)

### 🔧 Missing Value & Cleaning
![Missing Value](https://raw.githubusercontent.com/c14250130-ui/KNIME-Cereal-Data-Processing-Visualization-Workflow/main/Screenshot%202025-12-09%20074105.png)

### 🔎 Correlation Matrix  
![Correlation Matrix](https://raw.githubusercontent.com/c14250130-ui/KNIME-Cereal-Data-Processing-Visualization-Workflow/main/Screenshot%202025-12-09%20074350.png)

### 📊 Histogram Distribusi Nutrisi 
![Histogram](https://raw.githubusercontent.com/c14250130-ui/KNIME-Cereal-Data-Processing-Visualization-Workflow/main/Screenshot%202025-12-09%20074443.png)

### 📈 Scatter Plot (Calories vs Sugar)
![Scatter Plot](https://raw.githubusercontent.com/c14250130-ui/KNIME-Cereal-Data-Processing-Visualization-Workflow/main/Screenshot%202025-12-09%20074433.png)

### 🧩 Pie Chart
![Pie Chart](https://raw.githubusercontent.com/c14250130-ui/KNIME-Cereal-Data-Processing-Visualization-Workflow/main/Screenshot%202025-12-09%20074422.png)

### 📊 Bar Chart
![Bar Chart](https://raw.githubusercontent.com/c14250130-ui/KNIME-Cereal-Data-Processing-Visualization-Workflow/main/Screenshot%202025-12-09%20074412.png)



