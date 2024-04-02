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
#### Kami mengidentifikasi dan menangani data yang hilang: 
Kami melakukan identifikasi data yang hilang atau missing values dalam dataset kami. Kami menghapus baris atau kolom yang memiliki missing values atau mengisi nilai yang hilang dengan metode imputasi.
#### Kami menghapus duplikat data: 
Kami mengidentifikasi dan menghapus duplikat data dari dataset kami. Hal ini dilakukan untuk memastikan bahwa data kami tidak mengandung duplikat yang dapat memengaruhi hasil analisis.
#### Kami memeriksa kesalahan atau inkonsistensi dalam entri data: 
Kami memeriksa dataset kami untuk mengidentifikasi kesalahan atau inkonsistensi dalam entri data, seperti kesalahan penulisan, format yang salah, atau outlier yang mencurigakan.
#### Kami melakukan normalisasi data: 
Kami melakukan normalisasi data jika diperlukan untuk memastikan konsistensi format dan rentang nilai antar variabel. Contohnya adalah mengonversi satuan pengukuran, standarisasi format tanggal, atau melakukan scaling untuk variabel numerik.
#### Kami menangani outlier: 
Kami mengidentifikasi dan menangani outlier yang mungkin ada dalam dataset kami. Hal ini dilakukan untuk memastikan bahwa outlier tidak memengaruhi hasil analisis statistik dan model prediktif kami.
#### Kami memvalidasi data referensial: 
Kami melakukan validasi data referensial atau data yang berkaitan dengan data utama kami. Kami memastikan bahwa data referensial tersebut valid dan konsisten.
#### Kami menangani kesalahan manusia: 
Kami mengidentifikasi dan memperbaiki kesalahan yang disebabkan oleh kesalahan manusia atau kesalahan input data.
#### Kami melakukan transformasi data: 
Jika diperlukan, kami melakukan transformasi data untuk memenuhi kebutuhan analisis kami. Ini termasuk penggabungan kolom, pemisahan kolom, atau ekstraksi fitur dari data yang ada.
#### Kami memvalidasi konsistensi data: 
Kami melakukan validasi konsistensi data untuk memastikan bahwa data kami sesuai dengan aturan bisnis atau domain pengetahuan yang relevan.

## Visualisasi Data
### Analisis Univariat
![image](https://github.com/Ega121320043/Prediksi-Suhu-Rata-rata-Kabupaten-Barito-Utara/assets/165037047/44b22c83-a59d-485c-b1e5-d4082220542b)
![image](https://github.com/Ega121320043/Prediksi-Suhu-Rata-rata-Kabupaten-Barito-Utara/assets/165037047/a7567afe-5ffa-4bf4-9b5b-ca22862aadde)
![image](https://github.com/Ega121320043/Prediksi-Suhu-Rata-rata-Kabupaten-Barito-Utara/assets/165037047/dce7b96a-3aea-42d0-9d05-c97be4fdfbc6)
![image](https://github.com/Ega121320043/Prediksi-Suhu-Rata-rata-Kabupaten-Barito-Utara/assets/165037047/6baa14b4-9c2a-478a-b76b-4a7dcc38b994)
![image](https://github.com/Ega121320043/Prediksi-Suhu-Rata-rata-Kabupaten-Barito-Utara/assets/165037047/1a63b060-dcbf-4057-bccb-835c966479e3)
![image](https://github.com/Ega121320043/Prediksi-Suhu-Rata-rata-Kabupaten-Barito-Utara/assets/165037047/90f812a5-1c87-4aad-afd5-60869504da50)
![image](https://github.com/Ega121320043/Prediksi-Suhu-Rata-rata-Kabupaten-Barito-Utara/assets/165037047/b0e79392-58fc-4f9c-9ec3-5da2ba271702)
![image](https://github.com/Ega121320043/Prediksi-Suhu-Rata-rata-Kabupaten-Barito-Utara/assets/165037047/c482478f-85a5-4b47-b5f8-eee64a7f58c7)

Analisis univariat dari dataset suhu rata-rata bulanan Kabupaten Barito Utara dari tahun 2015 hingga 2022 memberikan pemahaman yang mendalam tentang distribusi variabel tunggal. Setiap histogram memvisualisasikan distribusi suhu untuk setiap bulan secara terpisah. Dari hasil analisis tersebut, terlihat bahwa distribusi suhu cenderung mengikuti pola normal, dengan puncak tertinggi terjadi sekitar nilai rata-rata, terutama pada bulan Mei dan Juni. Namun, terdapat variasi yang signifikan antara bulan-bulan, seperti terlihat pada distribusi yang sedikit condong ke kiri pada bulan Agustus, menunjukkan kemungkinan penurunan suhu rata-rata pada bulan tersebut.

### Analisis Multivariat 
#### Analisis Multivariat (Data Numerik)
![image](https://github.com/Ega121320043/Prediksi-Suhu-Rata-rata-Kabupaten-Barito-Utara/assets/165037047/4a4cf482-85c3-4bdd-863b-f4cdc58e11fe)

Analisis multivariat menggunakan matriks korelasi memberikan perspektif yang lebih luas tentang hubungan antar bulan. Melalui heatmap korelasi, terlihat tingkat korelasi antar bulan yang menyoroti pola musiman dan hubungan yang mungkin terjadi. Korelasi yang tinggi antara beberapa bulan menunjukkan adanya keterkaitan dalam perubahan suhu dari bulan ke bulan. Sebagai contoh, korelasi positif yang kuat antara suhu bulan-bulan yang berdekatan, seperti antara Juni dan Juli, menunjukkan adanya pola musiman yang konsisten dalam data suhu. Analisis multivariat ini melengkapi pemahaman yang diperoleh dari analisis univariat dengan memberikan gambaran yang lebih komprehensif tentang distribusi suhu bulanan dan hubungan antar bulan dalam rentang waktu yang diteliti.

#### Analisis Multivariat (Correlation Matrix)
Analisis multivariat pada data suhu rata-rata bulanan Kabupaten Barito Utara dilakukan dengan menyusun matriks korelasi. Matriks korelasi, sebagai alat analisis statistik, digunakan untuk mengevaluasi hubungan antara variabel numerik dalam dataset. Dalam konteks ini, matriks korelasi bertujuan untuk menentukan sejauh mana hubungan antara suhu rata-rata bulanan dari tahun 2015 hingga 2022. Koefisien korelasi yang dihasilkan, berkisar dari -1 hingga 1, menggambarkan tingkat hubungan linier antara variabel. Nilai 1 menunjukkan korelasi positif sempurna, -1 menunjukkan korelasi negatif sempurna, sementara nilai 0 menunjukkan tidak adanya hubungan linier. Dengan demikian, koefisien korelasi yang tinggi antara bulan-bulan menandakan keterkaitan yang kuat dalam hal suhu rata-rata. Analisis ini memberikan pemahaman yang dalam tentang pola atau tren suhu dari waktu ke waktu, yang pada gilirannya dapat memberikan wawasan berharga untuk perencanaan dan pengelolaan lingkungan serta kegiatan yang terkait dengan iklim di wilayah tersebut.

## Modeling
Dalam menjalankan analisis regresi terhadap data suhu rata-rata bulanan Kabupaten Barito Utara dari tahun 2015 hingga 2022, kami menggunakan model regresi linier. Model ini dimaksudkan untuk memahami dan memprediksi hubungan linier antara bulan-bulan dan suhu rata-rata yang diamati. Model regresi linier mengasumsikan bahwa terdapat hubungan linier yang stabil antara variabel independen (bulan) dan variabel dependen (suhu rata-rata), serta bahwa tidak ada asumsi terhadap distribusi data atau interaksi antar variabel. Secara matematis, model regresi linier diwakili oleh persamaan:

\[ Y_i = \beta_0 + \beta_1X_i + \varepsilon_i \]

di mana \( Y_i \) adalah suhu rata-rata pada bulan ke-\(i\), \( X_i \) adalah bulan ke-\(i\), \( \beta_0 \) adalah intercept (konstanta), \( \beta_1 \) adalah koefisien regresi (kemiringan), dan \( \varepsilon_i \) adalah kesalahan acak. Tujuan utama dari analisis regresi ini adalah untuk mengestimasi parameter \( \beta_0 \) dan \( \beta_1 \) yang optimal sehingga model dapat memberikan prediksi yang akurat terhadap suhu rata-rata bulanan berdasarkan bulan-bulan yang diamati. Penggunaan model regresi linier dalam konteks ini memungkinkan kita untuk mengidentifikasi dan memahami tren jangka panjang dalam suhu rata-rata bulanan, yang dapat memberikan wawasan yang berharga dalam perencanaan dan pengambilan keputusan terkait dengan iklim dan lingkungan di Kabupaten Barito Utara.
