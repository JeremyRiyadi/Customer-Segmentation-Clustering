## 📁 Dataset Overview

Dataset ini berisi informasi terkait **transaksi pelanggan** dari sebuah perusahaan retail. Data mencakup informasi demografis pelanggan, perilaku pembelian, dan detail produk yang dibeli. Dataset ini digunakan untuk **unsupervised learning**, khususnya **customer segmentation (klasterisasi)**

### 📌 Fitur Utama:

* `Customer ID`, `Gender`, `Birth Date`, `Location`
* `Item Purchased`, `Category`, `Purchase Amount (USD)`
* `Size`, `Color`, `Season`, `Review Rating`
* `Subscription Status`, `Shipping Type`, `Discount Applied`, `Promo Code Used`
* `Previous Purchases`, `Preferred Payment Method`, `Frequency of Purchases`

---

## 🧹 Data Preprocessing

Langkah-langkah preprocessing yang dilakukan antara lain:

* Konversi `Birth Date` menjadi `Age`
* Encoding fitur kategorikal menggunakan One-Hot Encoding
* Menangani missing values
* Normalisasi data numerik (MinMaxScaler)
* Seleksi fitur yang relevan untuk klasterisasi

---

## 📊 Exploratory Data Analysis (EDA)

Beberapa analisis dan visualisasi yang dilakukan:

* Distribusi umur pelanggan
* Perbandingan jenis kelamin pelanggan
* Distribusi nilai pembelian (`Purchase Amount`)
* Korelasi antar fitur numerik
* Analisis hubungan antara status langganan dan frekuensi pembelian

---

## 🔍 Clustering Approach

### Metode:

* **K-Means Clustering**
* Penentuan jumlah klaster menggunakan:

  * **Elbow Method**
  * **Silhouette Score**

### Hasil:

* Optimal cluster ditemukan pada `k = X` (tergantung hasil silhouette atau elbow)
* Visualisasi hasil clustering dengan PCA (2D)
* Analisis karakteristik masing-masing klaster (misalnya: cluster A berisi pelanggan muda dengan pembelian tinggi, cluster B berisi pelanggan pasif dengan transaksi sedikit, dst.)

---

## 📈 Evaluation

* Visualisasi inertia dan silhouette score menunjukkan bahwa pembagian klaster cukup baik.
* Interpretasi tiap klaster berdasarkan:

  * Umur
  * Nilai belanja
  * Frekuensi pembelian
  * Preferensi metode pembayaran dan langganan

---

## 📌 Conclusion

* Clustering berhasil membagi pelanggan ke dalam beberapa segmen yang berbeda berdasarkan perilaku dan demografi.
* Hasil segmentasi dapat digunakan oleh tim marketing untuk strategi pemasaran yang lebih tertarget (misalnya targeting khusus untuk pelanggan dengan frekuensi tinggi atau nilai pembelian rendah tapi potensial).

---

## 📁 File

* `2A.tsv` - Dataset transaksi pelanggan
* `clustering.ipynb` - Notebook analisis dan clustering
* `README.md` - Dokumentasi ini
