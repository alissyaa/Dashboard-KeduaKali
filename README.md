# KeduaKali — Data Science

**Coding Camp 2026 powered by DBS Foundation**
**Tim:** CC26-PSU226 | **Tema:** Sustainable & Responsible Consumption

---

## Anggota Tim (Data Science)

| ID Anggota | Nama | Peran |
|---|---|---|
| CDCC319D6X2692 | Alissya Humairah Martiasaputri | Data Science |
| CDCC319D6X2689 | Chyntia Claudia | Data Science |

---

## 📌 Tentang Proyek

**KeduaKali** adalah platform cerdas penyelamat makanan *leftover* yang menghubungkan restoran dengan konsumen secara real-time. Proyek ini dibangun di atas fondasi analisis data untuk menjawab krisis *food waste* di Indonesia — yang mencatat lonjakan surplus makanan siap saji sebesar **380%** hanya dalam satu tahun (2022→2023).

---

## 🗂️ Struktur Repository

```
├── notebooks/
│   └── Project_KeduaKali.ipynb   # Notebook utama
│   ├── KeduaKali_ABTesting_Final.ipynb # A/B Testing
├── dashboard/
│   └── dashboard.py                  # Streamlit dashboard
├── data/
│   ├── restaurant_sales_cleaned.csv
│   ├── global_food_wastage_dataset.csv
│   └── food_wastage_cleaned.csv
├── laporan/
│   └── Laporan Teknis KeduaKali.pdf  # Laporan teknis lengkap
└── README.md
└── logoKeduaKali.png   # Logo keduaKali
```

---

## 📂 Dataset

| Dataset | Ukuran | Kegunaan |
|---|---|---|
| `restaurant_sales_cleaned` | 10.000 baris, 13 kolom | Analisis penjualan & efektivitas promosi |
| `global_food_wastage_dataset` | 5.000 baris, 8 kolom | Tren kerugian ekonomi global (2018–2024) |
| `food_wastage_cleaned` | 1.782 baris, 11 kolom | Analisis efisiensi produksi per acara |

---

## 🔍 Temuan Utama

- **Prepared Food** menjadi kategori kerugian ekonomi terbesar secara global — total **17,87 juta USD** (2018–2024)
- Indonesia menempati **posisi keempat global** dalam rasio limbah per populasi
- Promosi terbukti secara statistik (Z-Test, α=0.05) meningkatkan konversi penjualan dan menekan sisa makanan — Kopitiam mencatat penurunan sisa hingga **90%** saat ada promosi
- Cuaca berpengaruh signifikan: Food Stall paling rentan saat hujan, Kopitiam saat cerah
- Setiap tipe restoran memiliki "musim surplus" yang berbeda — pendekatan *one-size-fits-all* tidak efektif

---

## 🤖 Model Machine Learning

- **LSTM Time-Series Forecasting** — prediksi volume surplus per tipe restoran
- **Content-Based Filtering** — sistem rekomendasi makanan surplus untuk konsumen

---

## 📈 Dashboard Streamlit

Dashboard interaktif mencakup:
- Visualisasi EDA dari ketiga dataset
- Prediksi surplus berbasis model LSTM
- Filter berdasarkan tipe restoran, cuaca, dan waktu sajian

---

## 🚀 Cara Menjalankan KeduaKali

### Prasyarat
Pastikan Python dan virtual environment (`.venv`) sudah tersedia pada project.

---

### 1. Menjalankan Dashboard Streamlit

```bash
# Aktifkan virtual environment
.venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Jalankan dashboard
streamlit run dashboard.py
```

Dashboard akan tersedia pada:
```text
http://localhost:8501
```

---

### Struktur Menjalankan Aplikasi

```bash
.venv\Scripts\activate
pip install -r requirements.txt
streamlit run dashboard.py
```

---

## 📄 Laporan Teknis

Laporan teknis komprehensif tersedia di folder `laporan/`, mencakup:
- Problem discovery & identifikasi 7 pertanyaan bisnis
- Data wrangling & cleaning ketiga dataset
- Exploratory Data Analysis (EDA) lengkap
- Pengujian A/B Testing dengan validasi statistik formal
- Kesimpulan & rekomendasi strategis

---

## 🛠️ Tech Stack

`Python` `Pandas` `NumPy` `Scikit-learn` `TensorFlow/Keras` `Statsmodels` `Matplotlib` `Seaborn` `Streamlit`
