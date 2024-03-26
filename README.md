# Prediksi-Suhu-Rata-rata-Kabupaten-Barito-Utara
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Langkah 1: Memuat data
data = pd.read_csv('Suhu.csv')

# Langkah 2: Visualisasi distribusi data
plt.figure(figsize=(8, 6))
sns.histplot(data['Temperature'], kde=True, color='skyblue')
plt.title('Distribusi Suhu Rata-rata Bulanan')
plt.xlabel('Suhu (Celsius)')
plt.ylabel('Frekuensi')
plt.show()

# Langkah 3: Plot tren waktu
plt.figure(figsize=(10, 6))
sns.lineplot(data=data, x='Month', y='Temperature')
plt.title('Tren Suhu Rata-rata Bulanan (2015-2022)')
plt.xlabel('Tanggal')
plt.ylabel('Suhu (Celsius)')
plt.xticks(rotation=45)
plt.show()

# Langkah 4: Plot musimanitas
plt.figure(figsize=(10, 6))
sns.boxplot(data=data, x='Month', y='Temperature')
plt.title('Polanya Musiman Suhu Rata-rata Bulanan')
plt.xlabel('Bulan')
plt.ylabel('Suhu (Celsius)')
plt.xticks(rotation=45)
plt.show()

# Langkah 5: Korelasi dengan variabel lain (opsional)
# Jika ada variabel lain seperti 'Curah Hujan', Anda bisa gunakan pairplot atau heatmap korelasi

# Langkah 6: Visualisasi spasial (opsional)
# Jika data terhubung dengan koordinat geografis, Anda bisa gunakan library geopandas atau folium untuk membuat peta.

# Langkah 7: Interpretasi hasil
# Setelah membuat visualisasi, analisis hasilnya untuk mendapatkan pemahaman yang lebih baik tentang tren dan pola yang ada dalam data.
# Identifikasi apakah ada tren jangka panjang, musiman, atau pola korelasi dengan variabel lain yang dapat memengaruhi suhu rata-rata.
