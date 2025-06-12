# 🛍️ Sales Analysis: Skincare & Beauty E-Commerce

## 📌 Deskripsi Proyek
Proyek ini bertujuan untuk menganalisis performa penjualan dari toko e-commerce global yang menjual produk skincare dan beauty. Melalui data transaksi historis, proyek ini mengeksplorasi tren penjualan, performa produk, efek diskon, dan memberikan insight untuk pengambilan keputusan bisnis.

## 🎯 Tujuan Analisis
- Mengidentifikasi tren penjualan berdasarkan waktu dan kategori produk.
- Menentukan produk/kategori paling laris dan paling menguntungkan.
- Menilai dampak diskon terhadap pendapatan dan profit.
- Memberikan rekomendasi berbasis data untuk meningkatkan performa penjualan.

## 🧾 Dataset
Dataset mencakup informasi:
- Produk (`Product`, `Category`, `Subcategory`)
- Transaksi (`Order_ID`, `Order_Date`, `Quantity`, `Discount`)
- Hasil keuangan (`Sales`, `Profit`)
- Wilayah pelanggan (`Country`, `City`, `Region`,`Market`, `Customer_ID`)

(Sumber: Dummy dataset dibuat untuk keperluan portofolio (Kaggle)

## 🛠️ Tools yang Digunakan
- Python (Pandas, Matplotlib, Seaborn)
- Google Colab / Jupyter Notebook
- Tableau (Dashboard)

## 🔍 Alur Analisis
1. Data Cleaning & Preparation
2. Exploratory Data Analysis (EDA)
3. Analisis Penjualan dan Diskon
4. Visualisasi Insight
5. Rekomendasi Bisnis

## 📊 Hasil Utama
- 📈 Penjualan menunjukkan peningkatan konsisten dari 2020 hingga 2023, mencapai **`$2.192.647`** di tahun terakhir, menandakan pertumbuhan bisnis yang baik. Namun, profit mengalami penurunan di tahun 2023 setelah kenaikan selama dua tahun sebelumnya.
  
  ![Image](https://github.com/user-attachments/assets/f026e0fa-581b-40b4-81c2-a73b9bd02f7f)

   Pola musiman yang kuat terlihat, dengan puncak penjualan di November-Desember dan titik terendah di Februari.
  
  ![Image](https://github.com/user-attachments/assets/6fd8e3aa-7561-4cbb-acfb-07cacde53c70)

  Analisis mendalam diperlukan untuk mengidentifikasi penyebab **penurunan profit di 2023**, termasuk dampak diskon dan performa produk. Optimalkan promosi di **Q4 (Oktober - Desember)** dengan **bundling dan kampanye digital**, serta dorong penjualan di awal tahun **(Januari-Februari)** dengan program loyalitas atau peluncuran produk baru.

- 🧴 Produk **Herbal Essences Bio** mencatat penjualan tertinggi **`$67.640`**, dan termasuk dalam kategori **Body Care**   yang dominan **`>$2.5 juta`**.
  
  ![Image](https://github.com/user-attachments/assets/57b9e77e-ec68-4dcb-99ec-9f49425eaae4)
  
  Namun, penjualan tinggi ini tidak sebanding dengan profit margin yang dihasilkan, mengindikasikan margin keuntungan per unit yang rendah.
  
  ![Image](https://github.com/user-attachments/assets/72b5ff4a-567b-4bfb-aa64-c0bfe30dcfea)
  
  Evaluasi struktur biaya dan strategi diskon untuk **Herbal Essences Bio** guna meningkatkan profitabilitas. Pertimbangkan untuk fokus pada produk dengan margin lebih tinggi dalam kategori **Body Care** atau menyesuaikan harga **Herbal Essences Bio**.

- Segmen **Corporate** memberikan kontribusi profit terbesar **(608.523)** meskipun jumlah order **(15.429)** lebih sedikit dari segmen **Consumer" (26.518 order)**. Segmen **Consumer** menghasilkan profit **`$365.378`**, sementara **Self- Employed** memberikan kontribusi profit terendah **`($91.512,7` dengan 9.343 order)**.
  
  ![Image](https://github.com/user-attachments/assets/0e7ac744-97f3-4249-b050-8f6a9852d072)

- 🔖 Terdapat hubungan negatif antara pemberian diskon dan profit yang dihasilkan. Diskon antara **0%-20%** menghasilkan profit positif, sementara diskon **40%-80%** menyebabkan penurunan profit signifikan, bahkan kerugian.
  
  ![Image](https://github.com/user-attachments/assets/80fed549-b089-433a-9c1e-1e0c42b569a0)

  Tinjau kembali strategi diskon secara keseluruhan dan batasi diskon besar-besaran yang dapat merugikan profitabilitas. Pertimbangkan alternatif promosi yang tidak terlalu bergantung pada diskon, seperti bundling atau hadiah dengan pembelian.
  
- Amerika Serikat mendominasi jumlah pembelian **(55.950 unit)**, jauh melampaui negara lain seperti Prancis **(15.969)** dan Australia **(15.937)**. **Asia Pacific** adalah market terbesar **(77.628 unit)**, diikuti oleh **Eropa (64.656) dan USCA (57.709)**.
  
  ![Image](https://github.com/user-attachments/assets/87b1672d-7602-46a4-87dd-390be3ffb953)

  Fokuskan upaya pemasaran di **Amerika Serikat** dan **wilayah Asia Pacific** untuk memaksimalkan penjualan. Pertimbangkan untuk menyesuaikan strategi pemasaran di negara-negara dengan penjualan lebih rendah untuk meningkatkan penetrasi pasar

- Meskipun total penjualan dan pembelian masih rendah, **Afrika Tengah** menunjukkan pertumbuhan penjualan yang signifikan **(60%)** dan profit margin yang lumayan **(28%)**. Ini menandakan potensi pasar yang perlu dikembangkan.

  ![Image](https://github.com/user-attachments/assets/be40990e-1448-4dd0-bfe7-ccc21cc5387b)
  
  Pertimbangkan untuk meluncurkan promosi yang berbeda untuk di wilayah tersebut guna mengomptimalkan potensi yang ada pada daerah tersebut.

## Kesimpulan
Secara Keseluruhan penjualan produk skincare dan kecantikan ini cukup baik dari segi penjualannya karena menunjukan tren yang positif hanya mungkin perlu untuk dikaji ulang tentang pemberian diskon karena dengan adanya pemberian diskon yang besar akan mempengaruhi profit yang dihasilkan. Perlu diperhatikan juga untuk ketegori pelanggan Self-Employeed seperti dengan memberikan promosi yang berbeda dengan kategori pelanggan lainnya. Di Sisi lain perlu juga dipertimbangkan tentang strategi pemasaran serta promosi untuk wilayah-wilayah yang tingkat penjualannya masih rendah serta wilayah yang memiliki potensi baik

## Dashboard
![Image](https://github.com/user-attachments/assets/451ab592-f712-42e4-a9b0-e34971296376)

Untuk melihat Dashboard interaktif klik 
[Lihat Dashboard](https//:public.tableau.com/](https://public.tableau.com/views/Dashbord_17496234661780/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link))

## ▶️ Cara Menjalankan
1. Clone repo ini.
2. Jalankan `sales_analysis.ipynb` di Jupyter/Colab.
3. Buka file dashboard Tableau untuk visual interaktif.

## 👤 Author
Koko  
Bandung, 2025

## 📄 License
Proyek ini dibuat untuk tujuan edukasi dan portofolio.
