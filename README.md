# Prediksi Suhu Rata-rata Kabupaten Barito Utara
## Business Understanding
Tujuan dari proyek ini adalah untuk memprediksi suhu rata-rata di Kabupaten Barito Utara pada tahun 2023 berdasarkan data suhu rata-rata dari tahun 2015 hingga 2022. Prediksi suhu rata-rata yang akurat dapat membantu dalam perencanaan pertanian, pengelolaan sumber daya alam, dan pemahaman dampak perubahan iklim terhadap wilayah tersebut.
## Data Understanding
Data yang digunakan adalah dataset suhu rata-rata bulanan dari Kabupaten Barito Utara dari tahun 2015 hingga 2022. Dataset ini mencakup variabel suhu rata-rata bulanan dalam derajat Celsius. Selain itu, dataset juga dapat mencakup tanggal dan waktu pengukuran suhu.
## Data Preparation
### Pengumpulan Data
Data saya ambil dari BPS data berisikan rata rata suhu pada Kabupaten Barito Utara sejak tahun 2015 hingga tahun 2022, klik link berikut untuk melihat data yang saya gunakan 
[(Suhu Rata-rata Kabupaten Barito Utara 2015-2022).](Suhu.csv)

### Pembersihan Data
Kami mengidentifikasi dan menangani data yang hilang: Kami melakukan identifikasi data yang hilang atau missing values dalam dataset kami. Kami menghapus baris atau kolom yang memiliki missing values atau mengisi nilai yang hilang dengan metode imputasi.
Kami menghapus duplikat data: Kami mengidentifikasi dan menghapus duplikat data dari dataset kami. Hal ini dilakukan untuk memastikan bahwa data kami tidak mengandung duplikat yang dapat memengaruhi hasil analisis.
Kami memeriksa kesalahan atau inkonsistensi dalam entri data: Kami memeriksa dataset kami untuk mengidentifikasi kesalahan atau inkonsistensi dalam entri data, seperti kesalahan penulisan, format yang salah, atau outlier yang mencurigakan.
Kami melakukan normalisasi data: Kami melakukan normalisasi data jika diperlukan untuk memastikan konsistensi format dan rentang nilai antar variabel. Contohnya adalah mengonversi satuan pengukuran, standarisasi format tanggal, atau melakukan scaling untuk variabel numerik.
Kami menangani outlier: Kami mengidentifikasi dan menangani outlier yang mungkin ada dalam dataset kami. Hal ini dilakukan untuk memastikan bahwa outlier tidak memengaruhi hasil analisis statistik dan model prediktif kami.
Kami memvalidasi data referensial: Kami melakukan validasi data referensial atau data yang berkaitan dengan data utama kami. Kami memastikan bahwa data referensial tersebut valid dan konsisten.
Kami menangani kesalahan manusia: Kami mengidentifikasi dan memperbaiki kesalahan yang disebabkan oleh kesalahan manusia atau kesalahan input data.
Kami melakukan transformasi data: Jika diperlukan, kami melakukan transformasi data untuk memenuhi kebutuhan analisis kami. Ini termasuk penggabungan kolom, pemisahan kolom, atau ekstraksi fitur dari data yang ada.
Kami memvalidasi konsistensi data: Kami melakukan validasi konsistensi data untuk memastikan bahwa data kami sesuai dengan aturan bisnis atau domain pengetahuan yang relevan.
Kami mendokumentasikan proses: Kami mencatat langkah-langkah pembersihan data yang kami lakukan secara rinci, termasuk alasan di balik setiap tindakan yang kami ambil. Dokumentasi ini penting untuk memahami dan mereplikasi proses pembersihan data di masa mendatang.
