# 📊 Priority Customer Transaction Monitoring
Exploratory Data Analysis & Risk-Oriented Dashboard

## 🧭 Business Context
Segmen nasabah prioritas memiliki karakteristik transaksi bernilai besar yang secara alami berbeda dengan nasabah reguler. Bank perlu memastikan bahwa aktivitas transaksi bernilai tinggi pada segmen ini dapat dimonitor secara efektif untuk:
* meningkatkan pengawasan risiko
* mencegah potensi fraud
* meminimalkan false positive dalam sistem monitoring
* memahami karakteristik perilaku nasabah high-value

Project ini bertujuan untuk mengevaluasi apakah transaksi bernilai besar pada nasabah prioritas merupakan anomali atau perilaku yang masih wajar secara konteks finansial dan demografis.

## 🎯 Business Questions

Analisis difokuskan untuk menjawab enam pertanyaan utama berikut:
1. Siapa nasabah dengan total transaksi tertinggi?
2. Produk dan channel apa yang paling sering digunakan oleh nasabah prioritas?
3. Cabang atau wilayah mana dengan nilai transaksi terbesar?
4. Apakah terdapat transaksi outlier atau aktivitas yang tidak wajar secara statistik maupun perilaku?
5. Nasabah mana yang menunjukkan pola transaksi berisiko dan perlu dimonitor lebih lanjut?
6. Bagaimana profil demografi nasabah yang sering melakukan transaksi bernilai besar?


## 📂 Data Overview

- [Customer Dataset](dataset/customer.xlsx)
- [Transaction Dataset](dataset/transaction.xlsx)


Dataset yang digunakan mencakup:
- Data transaksi nasabah prioritas
- Informasi demografi (usia, gender, provinsi)
- Informasi finansial (rata-rata saldo, limit kredit)
- Metadata transaksi (produk, channel, cabang)

Data telah melalui proses:
- pembersihan data
- merge data

## 🔍 Analysis Approach

Pendekatan analisis dilakukan secara bertahap:
- Exploratory Data Analysis (EDA) untuk memahami distribusi dan pola transaksi
- Outlier detection berbasis statistik (IQR) untuk mendeteksi anomali ekstrem
- Analisis perilaku relatif, membandingkan aktivitas nasabah terhadap baseline populasi
- Utilisation analysis, menggunakan rasio transaksi terhadap saldo rata-rata
- Profiling demografis untuk validasi konteks perilaku transaksi

## 💡 Key Insights
- Aktivitas transaksi bernilai besar terkonsentrasi pada sebagian kecil nasabah prioritas dengan profil finansial yang matang.
- Tidak ditemukan anomali ekstrem secara statistik pada distribusi nilai transaksi.
- Terdapat subset nasabah dengan tingkat utilisasi dana yang tinggi.
- Nasabah dengan transaksi besar dan frekuensi tinggi umumnya berasal dari kelompok usia produktif hingga matang (30–59 tahun), dengan distribusi gender relatif seimbang dan sebaran geografis yang luas.

## 💼 Business Impact
Analisis menunjukkan bahwa transaksi bernilai besar pada segmen nasabah prioritas terkonsentrasi pada sebagian kecil nasabah dengan profil finansial matang, tersebar lintas wilayah, serta melibatkan berbagai produk dan kanal. Tidak ditemukan anomali ekstrem secara statistik, meskipun terdapat sebagian nasabah dengan utilisasi dana tinggi yang ditunjukkan oleh rasio transaksi terhadap saldo rata-rata di atas 1. Temuan ini menegaskan bahwa pola tersebut umumnya wajar, namun tetap memerlukan pengawasan risiko berbasis profil dan perilaku agar sistem monitoring lebih kontekstual dan minim false positive.

📊 Dashboard
Hasil analisis divisualisasikan dalam dashboard interaktif menggunakan Looker Studio untuk mendukung pemantauan risiko secara ringkas dan eksploratif.
<img width="2500" height="1876" alt="Dashboard" src="https://github.com/user-attachments/assets/6b3e34e2-0378-4832-8bbd-be94fa76367c" />


## 🧰 Tools & Technologies
- Python (pandas, numpy, matplotlib, seaborn)
- Google Looker Studio
- Jupyter Notebook

## 📌 Note
Project ini merupakan studi kasus analitik untuk keperluan pembelajaran dan portfolio. Seluruh data bersifat simulasi dan tidak merepresentasikan data nasabah sebenarnya.
