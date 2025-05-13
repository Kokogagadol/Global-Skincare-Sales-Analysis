# Analisis Penjualan dan Perilaku Konsumen Pada Toko Online Skincare
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
  pada tahapan awal kita perlu mengimport dataset yang akan dianalisis terlabih dahulu menggunakan library `pandas`.
  ```python
  # import library
  import numpy as np
  import pandas pd

  # load dataset
  data = pd.read_excel('/content/drive/MyDrive/Portfolio/Project 2 - Global Skincare/Global skincare and Beauty e-store_E-commerce Analysis_English.xlsx', sheet_name='data')
  data.head(3)
  ```
  output:
  
  ![Image](https://github.com/user-attachments/assets/48a0db5d-5e41-4878-99ee-31a31aa7e5b1)
 
* ### Data Assesing
  pada tahapan assesing data dilakuan beberapa pengecekan seperti data duplikat, data yang hilang, data tidak konsisten dan kesalahan tipe data. pengecekan dilakuan bertujuan agar mengetahui apa saja yang perlu diperbaiki atau dibersihkan di tahap data cleaning.
  
  ```python
  # 1. Check Data Duplicate
  print(f'Jumlah Data Duplicate : {data.duplicated().sum()}')
  
  # 2. Check Missing Value
  print(f'Jumlah Missing Value  : \n{data.isna().sum()}')
  ```
  Output:
  
  ![Image](https://github.com/user-attachments/assets/f358a09b-6dea-418e-a2bc-cbb2bb0e5280)
 
  ```python
  # 3. Chek Data Type
  data.info()
  ```
  Output:
  
  ![Image](https://github.com/user-attachments/assets/82c3d1e7-e91a-4614-be2a-41527350d538)
  
* ### Data Cleaning
  ```python
  # Menghapus Data Duplikat
  data.drop_duplicates(inplace=True)
  
  # Mengahapus Missing Value
  data.dropna(inplace=True)
  
  # Menambahkan Underscore '_' pada kolom yang memiliki dua kata
  data.rename(columns=lambda x:x.replace(" ","_"), inplace=True)
  ```

***
## 2. Exploratory Data Analysis
```python
data.describe()
```
Output:

Kode di atas akan menampilkan ringkasan dari data yang akan dianalisis dimana diketahui bahwa dataset menunjukan data transaksi dari bulan januari 2020 hingga Desember 2023 (4 tahun) dengan penjualan terbesar berada di angka $3940 sedangkan terkcilnya berada di angka $2, untuk jumlah pembelian terbanyak adalah 20 pcs dan pembelian terkcilnya yaitu 1 pcs, discount terbesar yang pernah diberikan adalah 85%. selain itu toko pernah mencatatakn profit terbesarnya di angka $1820 dan pernah mencatatkan profit minus di angka -$1746.


* Bagaimana Tren Penjualan dan Profit Bulanan Sepanjang Tahun?
  
* Produk atau kategori apa yang memiliki penjualan tertinggi?
  
* Negara atau wilayah mana yang memberikan kontribusi terbesar terhadap toal sales?
  
* Bagaimana perilaku pembelian berdasarkan segmentasi pelanggan (Consumer, Corporate, dll)?
  
* Apakah pelanggan dari segmen tertentu memberikan profit yang lebih besar dibanding yang lain?
  
* Apa dampak pemberian diskon terhadap profit?
  
* Apakah ada korelasi negatif antara diskon tinggi dan penurunan profit?
  
* Bagaimana distribusi penjualan berdasarkan negara, region, atau market?
  
* Wilyah mana yang memiliki potensi pasar terbesar untuk dikembangkan?
  
* Produk mana yang paling sering dipesan tetapi memiliki margin keuntungan rendah?
  
* Subkategori mana yang paling menguntungkan secara konsisten?
  

***
## 3. Data Visualization
***
## 4. Keisimpulan
***
## Interaktif Dashboard
***
## RFM Analysis
