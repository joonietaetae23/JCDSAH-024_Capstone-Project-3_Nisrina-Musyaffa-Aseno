# Travel Insurance Claim Prediction

## 📌 Project Overview
Proyek ini bertujuan untuk membangun model *machine learning* yang mampu memprediksi kemungkinan seorang pemegang polis mengajukan klaim asuransi perjalanan. Model dikembangkan menggunakan data historis pelanggan asuransi perjalanan, mencakup perjalanan domestik dan internasional, guna mendukung pengelolaan risiko dan pengambilan keputusan bisnis yang lebih akurat.

---

## 🎯 Business Context
Seiring meningkatnya jumlah perjalanan domestik dan internasional, perusahaan asuransi perjalanan menghadapi risiko klaim yang semakin beragam. Tidak semua pemegang polis memiliki tingkat risiko yang sama, sehingga kesalahan dalam memprediksi klaim dapat berdampak pada:
- Penetapan premi yang kurang optimal  
- Meningkatnya biaya klaim yang tidak terantisipasi  
- Menurunnya profitabilitas dan efisiensi operasional  

Pemanfaatan data historis pelanggan diharapkan dapat membantu perusahaan dalam mengelola risiko klaim secara lebih efektif.

---

## 🧾 Dataset
Dataset berisi data historis pemegang polis asuransi perjalanan, antara lain:
- Tujuan perjalanan  
- Jenis dan cakupan produk asuransi  
- Durasi perjalanan  
- Karakteristik perjalanan dan pelanggan  
- Riwayat klaim asuransi  

---

## 🎯 Target Variable
Status klaim asuransi:
- **0** → Tidak mengajukan klaim  
- **1** → Mengajukan klaim  

Permasalahan ini dimodelkan sebagai **binary classification**.

---

## ❓ Problem Statement
Tidak semua pemegang polis memiliki tingkat risiko klaim yang sama. Klaim yang tidak terprediksi dengan baik dapat menyebabkan:
- Peningkatan biaya klaim yang tidak terantisipasi  
- Kesulitan dalam pengelolaan risiko  
- Penurunan profitabilitas perusahaan  

Oleh karena itu, diperlukan model prediktif yang mampu mengidentifikasi pemegang polis berisiko klaim secara lebih akurat.

---

## 🥅 Goals
- Mengembangkan model *machine learning* untuk memprediksi kemungkinan pengajuan klaim asuransi.
- Meminimalkan risiko klaim yang tidak teridentifikasi oleh model.
- Mengidentifikasi variabel-variabel utama yang memengaruhi klaim, seperti:
  - Durasi perjalanan  
  - Tujuan perjalanan  
  - Jenis produk asuransi  
- Memberikan *insight* untuk mendukung strategi penetapan premi, pengembangan produk, dan peningkatan kualitas layanan.

---

## 🔍 Analytic Approach
1. Melakukan **Exploratory Data Analysis (EDA)** untuk memahami pola dan karakteristik data.
2. Melakukan **data preprocessing**, termasuk penanganan *missing values*, *feature engineering*, encoding, dan scaling.
3. Membangun **model klasifikasi** untuk memprediksi kemungkinan pengajuan klaim.
4. Mengevaluasi model dengan mempertimbangkan dampak kesalahan prediksi terhadap bisnis.

---

## 📊 Evaluation Metrics
Evaluasi model difokuskan pada kesalahan prediksi yang memiliki dampak bisnis signifikan:

| Jenis Error | Definisi | Konsekuensi Bisnis |
|------------|----------|--------------------|
| **False Positive (Type I Error)** | Pelanggan tidak klaim tetapi diprediksi klaim | Intervensi atau perlakuan risiko yang tidak perlu |
| **False Negative (Type II Error)** | Pelanggan klaim tetapi diprediksi tidak klaim | Biaya klaim yang tidak terantisipasi (**paling berisiko**) |

Berdasarkan konsekuensi tersebut, fokus evaluasi diarahkan pada **meminimalkan False Negative**, sehingga model mampu mengidentifikasi pemegang polis yang berpotensi mengajukan klaim secara lebih akurat.

---
