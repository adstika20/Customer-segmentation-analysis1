# Customer Segmentation Analysis
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

## Overview
Visualisasi berikut ini menampilkan hasil segmentasi pelanggan menggunakan algoritma **K-Means Clustering**, yang membagi pelanggan ke dalam empat cluster berdasarkan pola perilaku dan karakteristik mereka. Tujuannya adalah untuk memahami distribusi pelanggan agar strategi pemasaran dapat disesuaikan secara tepat dan efektif.

![Customer Segmentation Clustering](https://github.com/adstika20/Customer-segmentation-analysis1/blob/main/K%20Means%20Clustering.png)

---
#### 1. **Cluster 2 – The Largest Segment (~240 customers)**
Cluster ini merupakan kelompok pelanggan paling besar yang dapat diidentifikasi sebagai pelanggan **pasif**. Mereka cenderung kurang aktif atau mungkin pelanggan baru yang belum menunjukkan loyalitas penuh. Jumlah besar ini membuka peluang evaluasi ulang untuk meningkatkan engagement, atau mungkin melakukan re-activation campaign agar mereka kembali aktif bertransaksi.

#### 2. **Cluster 0 – Loyal Customers (~220 customers)**
Pelanggan di cluster ini menunjukkan loyalitas yang kuat dan potensi tinggi untuk program-program eksklusif. Mereka adalah aset berharga yang dapat didorong untuk peningkatan lifetime value melalui program reward, membership eksklusif, dan penawaran khusus.

#### 3. **Cluster 1 – Discount-Sensitive Customers (~200 customers)**
Segmen ini terdiri dari pelanggan yang sangat responsif terhadap diskon dan promosi. Strategi pemasaran yang cocok adalah kampanye promosi bertarget, penawaran khusus dengan potongan harga, serta flash sales yang dapat meningkatkan frekuensi pembelian mereka.

#### 4. **Cluster 3 – Niche or At-Risk Customers (~125 customers)**
Cluster terkecil ini belum memiliki deskripsi yang jelas, tetapi bisa jadi mengandung pelanggan eksklusif dengan karakter unik, atau pelanggan yang berpotensi **churn** (berhenti bertransaksi). Pendekatan yang tepat adalah melakukan analisa lebih dalam untuk mengidentifikasi karakteristik dan membuat strategi retensi atau personalisasi layanan.

---

#### Strategic Implications

- **Tidak Semua Pelanggan Sama:** Distribusi yang tidak merata menuntut strategi yang **diferensiasi** sesuai karakteristik tiap cluster.
- **Efisiensi Sumber Daya Pemasaran:** Dengan memahami segmentasi ini, budget pemasaran dapat dialokasikan lebih tepat sasaran.
- **Peluang Pengembangan Produk dan Layanan:** Setiap cluster memberikan insight untuk pengembangan fitur atau produk yang lebih sesuai dengan kebutuhan masing-masing segmen.

---


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




















