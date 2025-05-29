# 🧠 Customer Segmentation Analysis
Analisis segmentasi pelanggan menggunakan data penjualan Superstore dan algoritma clustering (K-Means).

Proyek ini bertujuan untuk mengelompokkan pelanggan berdasarkan perilaku pembelian mereka dengan menggunakan metode K-Means Clustering. Proses ini melibatkan pembersihan data, rekayasa fitur, eksplorasi data, hingga pemodelan untuk menemukan pola yang dapat digunakan sebagai dasar strategi pemasaran.

## Struktur Proyek / Tree
```
Customer_Segmentation_Analysis.ipynb
│
├── Data Preparation
│   ├── Gathering Data
│   └── Data Cleansing
│
├── Feature Engineering
│   ├── Discount Amount
│   ├── Aggregasi per Customer
│   └── Recency Calculation
│
├── Exploratory Data Analysis
│   ├── Statistik Deskriptif
│   ├── Distribusi Numerik
│   └── Distribusi Kategorikal
│
├── Preprocessing
│   ├── One-Hot Encoding
│   └── Normalisasi (MinMaxScaler)
│
├── Modeling
│   ├── Elbow Method
│   └── KMeans Clustering
│
└── Visualization & Insights
    └── Cluster Interpretation
```
## Analisis Hasil 

### 🔍 Fitur yang Digunakan
Segmentasi pelanggan didasarkan pada beberapa fitur utama, yaitu:

- **Recency**: Jarak waktu sejak terakhir kali pelanggan melakukan pembelian.
- **Frequency**: Frekuensi pembelian yang dilakukan oleh pelanggan.
- **Monetary**: Total nilai pembelian yang dilakukan pelanggan.
- **Discount Amount**: Nilai hasil perkalian antara penjualan (*Sales*) dan diskon (*Discount*) yang diterima pelanggan.

Dengan fitur-fitur ini, model dapat mengidentifikasi kelompok pelanggan berdasarkan perilaku mereka, sehingga membantu pengambilan keputusan strategis seperti penawaran khusus, retensi pelanggan, dan pemasaran yang lebih terarah.



## Cara Instalasi / Requirements

Untuk menjalankan proyek ini secara lokal, Anda memerlukan:
```
pip install pandas numpy matplotlib seaborn scikit-learn

```

## 🗂 Dataset

- **📁 Nama File**: `Superstore.csv`
- **🌐 Sumber**: [Dicoding GitHub Dataset](https://github.com/dicodingacademy/dicoding_dataset/blob/main/superstore/Superstore.csv)
- **🧾 Deskripsi**:  
  Dataset ini berisi data transaksi penjualan retail dari sebuah Superstore yang mencakup berbagai informasi penting, seperti:
  - `Customer ID`: Identitas unik pelanggan  
  - `Order Date`, `Ship Date`: Tanggal pemesanan dan pengiriman  
  - `Segment`: Tipe pelanggan (Consumer, Corporate, Home Office)  
  - `Region`: Wilayah pemasaran  
  - `Category` & `Sub-Category`: Kategori dan subkategori produk  
  - `Sales`, `Profit`, `Discount`, `Quantity`: Detail transaksi penjualan  
  - `Order ID`: ID unik dari setiap transaksi  
  - `Postal Code`: Lokasi pengiriman  




















