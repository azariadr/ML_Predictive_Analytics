# Laporan Proyek Machine Learning - Azaria Dhea Rismaya

## Domain Proyek

**Proyek "Medical Insurance Premium Prediction"** berfokus pada industri asuransi kesehatan, sebuah sektor penting yang menyediakan perlindungan finansial terhadap risiko kesehatan bagi individu dan keluarga. Dalam konteks ini, perusahaan asuransi menawarkan layanan dengan menetapkan premi kepada pemegang polis.

Proyek ini bertujuan mengembangkan model prediktif untuk membantu perusahaan asuransi menghitung premi asuransi kesehatan dengan lebih presisi. Dengan mempertimbangkan berbagai faktor risiko, seperti usia, riwayat penyakit kronis, sejarah keluarga terkait penyakit serius, pengalaman menjalani operasi besar, serta data fisik seperti tinggi dan berat badan, model ini dapat menghasilkan estimasi premi yang lebih relevan dan sesuai dengan risiko yang dihadapi individu.

Model prediktif ini dirancang untuk memberikan estimasi premi yang lebih adil bagi calon pemegang polis. Dengan menganalisis faktor risiko secara menyeluruh, model ini dapat meminimalkan ketidakadilan dalam penentuan premi, sehingga jumlah premi yang dibayarkan mencerminkan risiko kesehatan yang sebenarnya.

Dengan memanfaatkan model ini, perusahaan asuransi dapat menetapkan premi berdasarkan risiko individu, membantu mereka mengelola potensi kerugian keuangan secara lebih efektif. Teknologi prediktif ini dapat mempercepat dan menyederhanakan proses penetapan premi, mengurangi waktu serta sumber daya yang dibutuhkan.

Calon pemegang polis akan menerima estimasi premi yang mencerminkan risiko kesehatan mereka secara lebih proporsional. Premi yang dihitung berdasarkan profil risiko individu memungkinkan pemegang polis mendapatkan perlindungan yang optimal sesuai dengan kebutuhan mereka, memberikan rasa aman dalam menghadapi potensi risiko kesehatan.

Secara keseluruhan, model prediktif yang dikembangkan dalam proyek ini memberikan manfaat signifikan bagi perusahaan asuransi dan calon pemegang polis. Perusahaan dapat mengelola risiko dan menentukan premi dengan lebih efisien, sementara calon pemegang polis mendapatkan premi yang lebih adil dan sesuai dengan kebutuhan mereka.

## Business Understanding

Proyek ini dirancang untuk mendukung perusahaan asuransi kesehatan dengan karakteristik bisnis berikut:
1. Perusahaan memiliki fokus kuat pada optimalisasi penggunaan data untuk meningkatkan pengambilan keputusan. Mereka menyadari pentingnya analisis prediktif dan teknologi machine learning dalam menghitung premi asuransi berdasarkan risiko individu.
2. Dengan akses ke data pelanggan yang luas dan terperinci, termasuk informasi usia, riwayat medis, operasi sebelumnya, alergi, riwayat penyakit keluarga, serta data fisik seperti tinggi dan berat badan, perusahaan dapat memanfaatkan data ini sebagai sumber utama untuk mengembangkan model prediktif yang akurat.
3. Perusahaan berkomitmen untuk meningkatkan daya saing di pasar asuransi kesehatan dengan menggunakan teknologi prediktif untuk menetapkan premi yang lebih akurat dan menawarkan produk asuransi yang kompetitif.

Proyek ini dirancang untuk membantu perusahaan mencapai tujuan bisnisnya dengan cara berikut:
1. Model prediktif memungkinkan perusahaan menghitung premi asuransi dengan lebih presisi, berdasarkan faktor risiko seperti usia, riwayat medis, operasi besar, dan data fisik lainnya. Keakuratan ini mendukung pengambilan keputusan berbasis data dan membantu perusahaan memitigasi risiko keuangan yang tak terduga.
2. Teknologi analisis prediktif dan machine learning memungkinkan proses otomatisasi dalam penetapan premi, mengurangi ketergantungan pada metode manual yang lebih lambat dan rentan kesalahan. Hal ini mempercepat proses kerja dan mengoptimalkan sumber daya perusahaan.
3. Model ini memberikan wawasan mendalam tentang pola risiko dan faktor-faktor yang memengaruhi premi asuransi kesehatan. Dengan wawasan ini, perusahaan dapat memahami kebutuhan pelanggan dengan lebih baik, mengidentifikasi tren pasar, serta membuat strategi bisnis yang lebih terinformasi.
4. Dengan menawarkan premi yang lebih akurat dan adil, perusahaan dapat menarik lebih banyak pelanggan dan memberikan produk yang kompetitif. Hal ini memperkuat posisi perusahaan di pasar, memperluas basis pelanggan, dan meningkatkan loyalitas mereka.

Proyek ini mendukung perusahaan asuransi kesehatan dalam meningkatkan pengambilan keputusan berbasis data, meningkatkan efisiensi operasional, serta membangun keunggulan kompetitif. Dengan model prediktif ini, perusahaan dapat menawarkan produk asuransi yang lebih relevan dan kompetitif, sekaligus memberikan layanan terbaik bagi calon pemegang polis.

### Problem Statements

- Apa langkah-langkah yang dapat dilakukan untuk meningkatkan akurasi dalam penentuan premi asuransi kesehatan?  
- Bagaimana cara meningkatkan transparansi dalam penetapan premi asuransi kesehatan?  
- Apa strategi yang efektif untuk mengurangi risiko keuangan akibat penetapan premi yang tidak akurat?  

### Goals

- Mengembangkan model analisis prediktif
- Meningkatkan transparansi
- Mengurangi risiko keuangan

Beberapa metrik yang akan digunakan untuk menilai keberhasilan proyek meliputi:
- Akurasi prediksi
- Tingkat transparansi
- Pengurangan risiko keuangan
- Mean Squared Error (MSE)

## Data Understanding
Dataset proyek ini berisi data kesehatan dari hampir 1000 pelanggan yang diberikan secara sukarela. Dataset ini digunakan untuk membangun model prediktif yang memperkirakan biaya premi asuransi kesehatan tahunan dalam INR (₹). Dataset dapat diunduh di: Medical Insurance Premium Prediction (https://www.kaggle.com/datasets/tejashvi14/medical-insurance-premium-prediction/data).

Berikut informasi pada dataset :
- Berjumlah 986 sampel dengan 11 fitur bertipe int64.
- Lengkap (tidak ada missing value)
- Format CSV

### Variabel-variabel pada Medical Insurance Premium Prediction dataset adalah sebagai berikut:

- Age : Usia pelanggan
- Diabetes : Apakah pasien memiliki kadar gula darah yang tidak normal
- BloodPressureProblems : Apakah pasien memiliki tekanan darah yang tidak normal
- AnyTransplants : Apakah pelanggan pernah menjalani transplantasi organ utama  
- AnyChronicDiseases : Apakah pelanggan menderita penyakit kronis seperti asma, dll.  
- Height : Tinggi badan pelanggan  
- Weight : Berat badan pelanggan  
- KnownAllergies : Apakah pelanggan memiliki alergi yang diketahui  
- HistoryOfCancerInFamily : Apakah ada anggota keluarga sedarah pelanggan yang pernah menderita kanker  
- NumberOfMajorSurgeries : Jumlah operasi besar yang pernah dijalani oleh pelanggan
- PremiumPrice : Harga premium tahunan

### Exploratory Data Analysis (EDA)
Visualisasi outlier menggunakan box plot berguna untuk memvisualisasikan distribusi data dan mendeteksi outlier. Box plot untuk kolom 'Weight' dan 'NumberOfMajorSurgeries' dibuat untuk melihat apakah ada outlier pada kedua fitur tersebut. Outlier adalah data yang nilainya jauh berbeda dari data lainnya. Pada box plot, outlier ditunjukkan sebagai titik-titik di luar batas atas dan bawah box plot.
![Weight Outlier](https://github.com/user-attachments/assets/3c786cd9-0c29-4b5f-b32a-f2e02468ae4a)
![NumberOfMajorSurgeries Outlier](https://github.com/user-attachments/assets/5806497e-651a-44b6-985c-241fa7d1fd3d)

Selanjutnya, distribusi data pada fitur kategorikal divisualisasikan menggunakan bar plot. Tujuannya untuk melihat distribusi data pada setiap fitur kategorikal, misalnya berapa banyak orang yang memiliki diabetes, memiliki riwayat kanker dalam keluarga, dan sebagainya.
![Distribusi Data pada Fitur Kategorikal](https://github.com/user-attachments/assets/080947d8-45fe-4434-8815-9244e307f898)
Sedangkan, histogram digunakan untuk memvisualisasikan distribusi data pada fitur numerikal, seperti 'Age', 'Height', dan 'Weight'.
![Distribusi Data pada Fitur Numerikal](https://github.com/user-attachments/assets/c17267ca-ea42-4de7-900b-c2c085bc2417)

Untuk memahami pengaruh fitur kategorikal terhadap 'PremiumPrice', digunakan bar plot yang menampilkan 'PremiumPrice' untuk setiap kategori. Visualisasi ini membantu mengidentifikasi kategori-kategori yang cenderung memiliki harga premi lebih tinggi atau lebih rendah, misalnya orang dengan diabetes cenderung membayar premi lebih tinggi.
![Hubungan PremiumPrice dengan Fitur Kategorikal](https://github.com/user-attachments/assets/a2611cc6-516b-49c0-b33a-0845d3c92001)

Selain itu, hubungan antar fitur divisualisasikan menggunakan pair plot, yang menunjukkan korelasi dan pola hubungan antar fitur tersebut.
![Visualisasi Korelasi Antar Fitur](https://github.com/user-attachments/assets/ddbfa003-8fff-4b8c-b628-4f3afd5a8eb3)
Terakhir, untuk menganalisa keterkaitan antara semua fitur, digunakan correlation matrix dan visualisasi heatmap. Heatmap menunjukkan tingkat korelasi antar fitur, dengan warna yang lebih terang mengindikasikan korelasi yang lebih kuat. Analisis ini membantu dalam memahami keterkaitan antar fitur dalam dataset dan dapat memberikan wawasan yang berguna untuk pemilihan fitur dan pemodelan.
![Matriks korelasi PremiumPrice](https://github.com/user-attachments/assets/5c445ded-5922-4057-80f2-26400962f4d1)

## Data Preparation
Dari visualisasi boxplot, dapat dilihat bahwa terdapat outlier pada kolom 'Weight' dan 'NumberOfMajorSurgeries'. Outlier pada fitur 'Weight' kemudian diatasi menggunakan Z-score. Z-score mengukur seberapa jauh suatu data dari rata-rata dalam satuan standar deviasi. Data yang memiliki Z-score lebih besar dari 3 dianggap sebagai outlier dan dihapus dari dataset.

One Hot Encoding adalah teknik untuk mengonversi variabel kategorikal menjadi representasi numerik agar dapat digunakan dalam model machine learning. Hal ini penting karena sebagian besar algoritma machine learning hanya mendukung input berupa angka.  

Pandas menyediakan fungsi **pd.get_dummies()** untuk mempermudah proses One Hot Encoding. Fungsi ini akan membuat kolom-kolom baru untuk setiap nilai unik dalam fitur kategorikal. Nilai pada kolom akan diatur menjadi 1 jika sesuai dengan nilai kategori tertentu, dan 0 jika tidak.

Setelah fitur kategorikal diubah menjadi bentuk numerik menggunakan one-hot encoding, fitur kategorikal awal yang belum di-encode perlu dihapus. Hal ini dilakukan untuk menghindari redundansi data dan meningkatkan efisiensi model. Dengan menghapus fitur kategorikal awal, DataFrame hanya akan berisi fitur-fitur numerik, termasuk fitur kategorikal yang telah di-encode. Hal ini membuat data siap untuk digunakan dalam proses training model.

Selain itu, membagi dataset menjadi data training dan data testing adalah langkah penting dalam pengembangan model machine learning. Pembagian ini dilakukan untuk mengevaluasi performa model pada data yang belum pernah dilihat sebelumnya dan untuk mencegah overfitting.  

Data training digunakan untuk melatih model, sedangkan data testing digunakan untuk mengukur seberapa baik model memprediksi data baru. Dengan memisahkan data ini, kita dapat mengukur kemampuan model untuk menggeneralisasi pada data yang belum dikenali.  

Rasio 80:20 sering digunakan untuk membagi dataset, di mana 80% data digunakan untuk pelatihan dan 20% sisanya untuk pengujian. Rasio ini dianggap seimbang karena memberikan cukup data untuk melatih model sekaligus menguji performanya. Namun, rasio tersebut dapat disesuaikan sesuai dengan kebutuhan proyek dan karakteristik dataset.

Langkah scaling fitur numerik bertujuan untuk menyamakan rentang nilai dari fitur-fitur numerik dalam dataset. Hal ini dilakukan untuk mencegah fitur dengan rentang nilai yang lebih besar mendominasi fitur dengan rentang nilai yang lebih kecil selama proses pelatihan model. Selain itu, scaling juga dapat meningkatkan kinerja dan stabilitas algoritma machine learning.

Dalam kasus ini, digunakan metode scaling StandardScaler dari library sklearn.preprocessing. Metode ini bekerja dengan menggeser distribusi setiap fitur agar memiliki mean 0 dan standar deviasi 1. Rumus yang digunakan adalah:

z = (x - u) / s

di mana:

z adalah nilai yang telah di-scaling
x adalah nilai asli
u adalah mean dari fitur
s adalah standar deviasi dari fitur

Scaling diterapkan pada fitur numerik 'Age', 'Height', dan 'Weight' dalam dataset. Setelah scaling, fitur 'Age', 'Height', dan 'Weight' pada data training dan testing akan memiliki mean 0 dan standar deviasi 1. Hal ini memastikan bahwa fitur-fitur tersebut berada dalam rentang nilai yang sama dan tidak akan mendominasi satu sama lain selama proses pelatihan model.

## Modeling
Dalam proses pemodelan, proyek ini menggunakan algoritma **SVR (Support Vector Regression)** dan **Huber Regressor** berdasarkan hasil dari pustaka PyCaret. Kedua algoritma ini diterapkan untuk memprediksi premi asuransi kesehatan dengan mempertimbangkan faktor risiko yang relevan.

**Support Vector Regression (SVR):**  
SVR adalah varian dari Support Vector Machines (SVM) yang dirancang untuk masalah regresi. Tujuannya adalah menemukan fungsi regresi yang meminimalkan kesalahan prediksi sambil mempertahankan margin maksimum. SVR mencari hyperplane (bidang) yang memisahkan data dengan margin maksimum. Hyperplane ini digunakan sebagai fungsi prediktif, memungkinkan model menoleransi beberapa outlier di luar margin. SVR menyeimbangkan kesalahan prediksi dengan kompleksitas model. SVR mampu menangani data dengan noise atau outlier dan fleksibel dalam memilih fungsi kernel untuk memodelkan hubungan non-linear.  

**Huber Regressor:**  
Algoritma ini tahan terhadap outlier dengan menggabungkan metode Least Squares (LS) dan Least Absolute Deviations (LAD) menggunakan fungsi kerugian Huber. Huber Regressor menghitung residual (selisih antara prediksi dan nilai aktual). Jika residual kecil, digunakan fungsi LS (kuadrat residual). Namun, jika residual besar, digunakan LAD (nilai absolut residual). Pendekatan ini membuat model lebih robust terhadap outlier. Huber Regressor lebih stabil dibandingkan regresi linier biasa, terutama saat data memiliki outlier signifikan.  

**Tahapan Pemodelan:**  
1. Melatih model menggunakan data training dengan parameter default dari pustaka.  
2. Menguji performa model pada data training dan testing.  
3. Menggunakan metrik evaluasi seperti MSE, MAE, RMSE, dan R² untuk mengukur performa.  
4. Mengoptimalkan model dengan grid search atau hyperparameter tuning:  
   - **Huber Regressor:** Menguji parameter `epsilon` : [1.0, 1.5, 2.0], `alpha` : [0.0001, 0.001, 0.01], dan `max_iter` : [100, 200, 300]. Parameter terbaik adalah `{'alpha': 0.01, 'epsilon': 2.0, 'max_iter': 100}`.  
   - **SVR:** Menguji parameter `kernel` : [`linear`, `rbf`], `C` : [0.1, 1, 10], dan `epsilon` : [0.1, 0.2, 0.3]. Parameter terbaik adalah `{'C': 10, 'epsilon': 0.3, 'kernel': 'linear'}`.

**Kelebihan dan Kekurangan Algoritma:**  
1. **Huber Regressor:**  
   - **Kelebihan:** Stabil terhadap outlier, menghasilkan prediksi yang konsisten.  
   - **Kekurangan:** Pemilihan nilai parameter delta membutuhkan pengujian manual.  
2. **SVR:**  
   - **Kelebihan:** Dapat menangani hubungan non-linear dengan fungsi kernel.  
   - **Kekurangan:** Sangat sensitif terhadap skala data, sehingga perlu normalisasi data.  

**Kesimpulan:**  
Huber Regressor lebih unggul dibandingkan SVR dalam proyek ini, terutama karena ketahanannya terhadap outlier. Untuk meningkatkan performa, tuning hyperparameter perlu diterapkan selama evaluasi model.  

## Evaluation
Metrik evaluasi yang digunakan dalam proyek ini adalah **Mean Squared Error (MSE)**, yang digunakan untuk mengukur sejauh mana perbedaan antara nilai prediksi dan nilai aktual dalam masalah regresi.

**MSE** menghitung rata-rata kuadrat selisih antara nilai prediksi dan nilai aktual. Semakin kecil nilai MSE, semakin baik model dalam memberikan prediksi yang akurat. Langkah-langkah untuk menghitung MSE adalah sebagai berikut:

1. Memiliki dataset yang berisi pasangan nilai aktual (y) dan prediksi (ŷ) untuk sejumlah contoh.
2. Menghitung selisih antara nilai aktual dan prediksi untuk setiap contoh.
3. Mengkuadratkan setiap selisih agar semua error memiliki kontribusi positif, terlepas dari apakah prediksi lebih rendah atau lebih tinggi dari nilai sebenarnya.
4. Menghitung rata-rata dari kuadrat selisih dengan menjumlahkan seluruh kuadrat dan membaginya dengan jumlah contoh.

Rumus MSE:
MSE = (1/n) * Σ(yᵢ - ŷᵢ)²
di mana:
- Σ adalah penjumlahan,
- y adalah nilai aktual,
- ŷ adalah nilai prediksi,
- n adalah jumlah contoh dalam dataset.

**Hasil Evaluasi:**  
- **Huber Regressor:**  
  - MSE pada data training: ~18,480,005.17
  - MSE pada data testing: ~25,177,095.35
  - Kesalahan lebih tinggi pada data testing, menunjukkan adanya overfitting.  
- **SVR:**  
  - MSE pada data training: ~39,541,221.08
  - MSE pada data testing: ~42,200,364.02
  - Tingkat kesalahan lebih tinggi pada data testing, juga menunjukkan overfitting.  

**Hasil Evaluasi Model Setelah Hyperparameter Tuning:**

| Model  | Train MSE  | Test MSE   | Train Eval | Test Eval |
|--------|------------|------------|------------|-----------|
| Huber  | 18,480,005.17 | 25,177,095.35 | 18,069,346.97 | 24,133,879.74 |
| SVR    | 39,541,221.08 | 42,200,364.02 | 21,675,142.50 | 26,666,895.77 |

![Hasil Evaluasi Akhir](https://github.com/user-attachments/assets/f9032e44-0a13-49e7-9ed3-cdda53de2297)

**Grafik Evaluasi Model**  

MSE merupakan metrik evaluasi umum untuk masalah regresi karena mengukur perbedaan antara prediksi dan nilai aktual secara keseluruhan dan memberi bobot lebih pada perbedaan besar. Namun, MSE juga sensitif terhadap outlier, di mana nilai ekstrem dapat memengaruhi MSE secara signifikan. Oleh karena itu, metrik alternatif seperti Mean Absolute Error (MAE) sering digunakan untuk memberikan gambaran kinerja model yang lebih lengkap.

**Kesimpulan Berdasarkan Evaluasi MSE:**
- **MSE pada Data Training:**  
  Model Huber memiliki MSE yang lebih rendah (18,480,005.17) dibandingkan dengan SVR (39,541,221.08), yang menunjukkan bahwa Huber lebih akurat dalam memprediksi pada data training.

- **MSE pada Data Testing:**  
  Model Huber juga memiliki MSE lebih rendah pada data testing (25,177,095.35) dibandingkan dengan SVR (42,200,364.02), yang menunjukkan bahwa Huber lebih baik dalam melakukan prediksi pada data yang belum pernah dilihat sebelumnya.

- **Evaluation Score pada Data Training:**  
  Model Huber juga memberikan evaluasi score yang lebih rendah pada data training (18,069,346.97) dibandingkan dengan SVR (21,675,142.50), menunjukkan kinerja yang lebih baik.

- **Evaluation Score pada Data Testing:**  
  Model Huber juga memberikan evaluasi score yang lebih rendah pada data testing (24,133,879.74) dibandingkan dengan SVR (26,666,895.77), menunjukkan kinerja yang lebih baik.

Berdasarkan hasil ini, model Huber lebih unggul daripada SVR dalam memprediksi premi asuransi kesehatan, karena memiliki MSE yang lebih rendah dan evaluasi score yang lebih baik pada data testing. Oleh karena itu, model Huber dianggap lebih optimal dalam proyek ini untuk perkiraan premi asuransi kesehatan dengan tingkat akurasi yang lebih tinggi.
