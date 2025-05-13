# Project 2: Analisis Penjualan dan Perilaku Pelanggan Pada Toko Online Skincare
Proyek ini bertujuan untuk menganalisis performa penjualan e-commerce dari toko skincare dan produk kecantikan global dengan memanfaatkan tiga tools utama: SQL untuk pengolahan data awal, Python untuk eksplorasi dan visualisasi data, serta Tableau untuk dashboard interaktif. Analisis ini diharapkan dapat memberikan insight terhadap penjulan, perilaku pelanggan dan performa produk. dataset yang digunakan merupakan dataset yang berasal dari situs Kaggle sehingga memungkinkan adanya keterbatasan dari analisis ini.

## Latar Belakang
Dalam dunia e-commerce yang kompetitif, perusahaan perlu memahami data transaksi penjualan mereka untuk mengambil keputusan strategis. Dengan menganalisis data penjualan dan perilaku pelanggan, bisnis dapat menentukan produk yang paling laris, saluran pemasaran terbaik, serta memaksimalkan keuntungan. Oleh karena itu, analisis ini penting untuk membantu manajemen meningkatkan strategi pemasaran dan pengelolaan inventaris.

## Pertanyaan Bisnis
### 📊 Analisis Penjualan
  * Bagaimana tren penjualan dan profit bulanan sepanjang tahun?
  * Produk atau kategori apa yang memiliki penjualan tertinggi?
  * Negara atau wilayah mana yang memberikan kontribusi terbesar terhadap total sales?
### 🧑‍🤝‍🧑 Segmentasi Pelanggan
  * Bagaimana perilaku pembelian berdasarkan segmentasi pelanggan (Consumer, Corporate, dll)?
  * Apakah pelanggan dari segmen tertentu memberikan profit yang lebih besar dibanding yang lain?
### 🏷️ Diskon dan Profitabilitas
  * Apa dampak pemberian diskon terhadap profit?
  * Apakah ada korelasi negatif antara diskon tinggi dan penurunan profit?
### 🌍 Analisis Geografis
  * Bagaimana distribusi penjualan berdasarkan negara, region, atau market?
  * Wilyah mana yang memiliki potensi pasar terbesar untuk dikembangkan?
### 📦 Kinerja Produk
  * Produk mana yang paling sering dipesan tetapi memiliki margin keuntungan rendah?
  * Subkategori mana yang paling menguntungkan secara konsisten?
## Deskripsi Dataset
* Nama Dataset      : `Global skincare and Beauty e-store_E-commerce Analysis_English.xlsx`
* Sumber            : Kaggle
* Jumlah data/baris : 51.291 baris
* Variabel          :
  
![image](https://github.com/user-attachments/assets/c5873582-51b7-4012-ab96-bfb8968e05a6)

## Format lainya bisa dilihat di:
* PDf           :
* Google Colab  :
* Tableau       : 

***
## 1. Data Wrangling
* ### Data Gathering
  
  ```python
  # import library
  import numpy as np
  import pandas pd

  # load dataset
  data = pd.read_excel(,sheet_name='data')
  data.head()
  ```
  pada tahapan awal kita perlu mengimport dataset yang akan dianalisis terlabih dahulu menggunakan library `pandas`.
  
  output:
  
* ### Data Assesing
  
  ```python
  # 1. Check Data Duplicate
  print(f'Jumlah Data Duplicate : {data.duplicated().sum()}
  
  # 2. Check Missing Value
  print(f'Jumlah Missing Value  : {data.isna().sum()}'
  
  # 3. Check Inconsitent Data
  
  # 4. Check Data Type
  ```
  pada tahapan assesing data dilakuan beberapa pengecekan seperti data duplikat, data yang hilang, data tidak konsisten dan kesalahan tipe data. pengecekan dilakuan bertujuan agar mengetahui apa saja yang perlu diperbaiki atau dibersihkan di tahap data cleaning.
  
* ### Data Cleaning


***
## 2. Exploratory Data Analysis
***
## 3. Data Visualization
***
## 4. Keisimpulan
***
## Interaktif Dashboard
***
## RFM Analysis
