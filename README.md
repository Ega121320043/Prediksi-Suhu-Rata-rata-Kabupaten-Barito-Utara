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
### Model Regresi
Dalam rumus regresi yang diberikan:

Yi = a + bXi + ei

- Yi adalah suhu rata-rata pada bulan ke-i,
- Xi adalah bulan ke-i,
- a adalah intercept (konstanta),
- b adalah koefisien regresi (kemiringan), dan
- ei adalah kesalahan acak.

Dalam konteks ini:

- a mewakili titik perpotongan garis regresi dengan sumbu Y (intersep),
- b menunjukkan kemiringan garis regresi (slope), dan
- ei menggambarkan variabilitas yang tidak dapat dijelaskan oleh model.

Tujuan utama dari analisis regresi ini adalah untuk mengestimasi parameter a dan b yang optimal sehingga model dapat memberikan prediksi yang akurat terhadap suhu rata-rata bulanan berdasarkan bulan-bulan yang diamati. Dengan menggunakan model regresi linier, Anda dapat mengidentifikasi dan memahami tren jangka panjang dalam suhu rata-rata bulanan, yang dapat memberikan wawasan yang berharga dalam perencanaan dan pengambilan keputusan terkait dengan iklim dan lingkungan di Kabupaten Barito Utara.

### Model Random Forest Regression
Model Random Forest Regression merupakan sebuah metode prediksi yang menggunakan sejumlah pohon keputusan (decision trees) untuk melakukan regresi. Setiap pohon dalam model ini dibangun secara independen dan menghasilkan prediksi yang bersifat kontinu. Secara matematis, model Random Forest Regression dapat direpresentasikan sebagai berikut:

![image](https://github.com/Ega121320043/Prediksi-Suhu-Rata-rata-Kabupaten-Barito-Utara/assets/165037047/ae45cc3e-bc34-421f-98f5-144e49ccca80)

di mana Y(bar) adalah prediksi suhu rata-rata bulanan, N adalah jumlah pohon dalam model, dan Yi adalah prediksi suhu rata-rata bulanan yang dihasilkan oleh pohon ke-i.

Metode ini menggabungkan prediksi dari setiap pohon keputusan untuk menghasilkan prediksi akhir. Proses pembangunan model ini melibatkan pemilihan secara acak dari fitur-fitur yang akan digunakan dalam pembangunan setiap pohon, serta pemilihan secara acak dari sampel data yang akan digunakan dalam pelatihan setiap pohon.

Model Random Forest Regression memiliki keunggulan dalam menangani masalah overfitting, karena masing-masing pohon dalam model ini dibangun secara independen dan kemudian dikombinasikan untuk menghasilkan prediksi yang lebih stabil dan akurat.

Dengan menggunakan metode Random Forest Regression, Anda dapat memprediksi suhu rata-rata bulanan di Kabupaten Barito Utara dengan lebih akurat dan dapat diandalkan, karena model ini mampu menangani pola-pola yang kompleks dan tidak linear dalam data suhu rata-rata bulanan.
## Evaluation
### Tabel Perbandingan Model Akhir:
![image](https://github.com/Ega121320043/Prediksi-Suhu-Rata-rata-Kabupaten-Barito-Utara/assets/165037047/2d7f2f89-88cb-4c7c-9d69-b8944df5821e)
Membuat prediksi terhadap data uji dan mengevaluasi kinerja model. Evaluasi dilakukan dengan menghitung sejumlah metrik evaluasi yang relevan, termasuk Mean Squared Error (MSE), Mean Absolute Error (MAE), dan Coefficient of Determination (R^2). Metrik-metrik tersebut digunakan untuk menilai seberapa baik model mampu memprediksi suhu rata-rata bulanan. Hasil evaluasi kemudian disajikan dalam bentuk tabel perbandingan model, yang memungkinkan analisis komparatif terhadap performa model Random Forest Regression dengan model-model lainnya.
### Tabel y_true dan y_pred
![image](https://github.com/Ega121320043/Prediksi-Suhu-Rata-rata-Kabupaten-Barito-Utara/assets/165037047/a85a0b5a-2157-4df8-abf6-5b88785b8fda)

Selain itu, nilai sebenarnya (y_true) dan nilai prediksi (y_pred) dari data uji juga disimpan dalam tabel terpisah untuk memudahkan analisis lebih lanjut. Grafik perbandingan model disiapkan untuk memvisualisasikan nilai MSE dan MAE dari model Random Forest Regression secara komparatif.

### Grafik Perbandingan Model 
![image](https://github.com/Ega121320043/Prediksi-Suhu-Rata-rata-Kabupaten-Barito-Utara/assets/165037047/9d461eb4-f935-4c27-8ccd-84dbae074054)

Terakhir, berdasarkan hasil evaluasi yang teliti, disimpulkan bahwa metode Random Forest Regression menunjukkan kinerja yang paling baik dalam memprediksi suhu rata-rata bulanan di Kabupaten Barito Utara. Kesimpulan ini didasarkan pada analisis mendalam terhadap metrik evaluasi yang relevan, memberikan wawasan yang berharga bagi perencanaan dan pengambilan keputusan terkait iklim dan lingkungan di wilayah tersebut.

## Refrensi
[1] Badan Pusat Statistik. (n.d.). Suhu Udara [Data]. Diakses dari https://barutkab.bps.go.id/indicator/151/89/1/suhu-udara.html

[2] Sarwono, A. E., & Handayani, A. (2021). Metode kuantitatif. Unisri Press.

[3] Fernandes, A. A. R. (2017). Metode statistika multivariat pemodelan persamaan struktural (sem) pendekatan warppls. Universitas Brawijaya Press.

[4] Novianty, D., dias Palasara, N., & Qomaruddin, M. (2021). Algoritma Regresi Linear pada Prediksi Permohonan Paten yang Terdaftar di Indonesia. JUSTIN (Jurnal Sistem Dan Teknologi Informasi), 9(2), 81-85.

[5] Ayuni, G. N., & Fitrianah, D. (2019). Penerapan metode Regresi Linear untuk prediksi penjualan properti pada PT XYZ. Jurnal telematika, 14(2), 79-86.

[6] Dama, H. R. A., Supianto, A. A., & Setiawan, N. Y. (2021). Analisis Penggunaan Model Regresi untuk Prediksi Penjualan Spare Part pada AHASS Nur Andhita Grogol. Jurnal Pengembangan Teknologi Informasi dan Ilmu Komputer, 5(12), 5591-5603.

[7] Lestari, E. S., Astuti, I., Informasi, T., Gunadarma, U., & Raya, J. M. (2022). Penerapan Random Forest Regression Untuk Memprediksi Harga Jual Rumah Dan Cosine Similarity Untuk Rekomendasi Rumah Pada Provinsi Jawa Barat. Jurnal Ilmiah FIFO, 14(2), 131.

[8] Huda, M. (2023). Penerapan metode Random Forest pada prediksi penilaian nilai aset KJPP SIG MALANG berbasis web (Doctoral dissertation, Universitas Islam Negeri Maulana Malik Ibrahim).

[9] Lumbanraja, F. R., Mudyaningsih, W., Hermanto, B., & Syarif, A. (2019, December). Implementasi Metode Random Forest untuk Prediksi Posisi Metilasi pada Sekuens Protein. In Prosiding Seminar Nasional Sains, Matematika, Informatika dan Aplikasinya (Vol. 5, No. 1).
