# **Machine Learning Regression Model: Prediksi Harga Apartemen Daegu**

## Latar Belakang 
Apartemen merupakan salah satu jawaban atas kebutuhan hunian masyarakat modern akibat keterbatasan lahan permukiman dan padatnya aktivitas bisnis di kawasan perkotaan. Oleh karena itu, menarik untuk mengkaji harga apartemen yang dipengaruhi oleh berbagai faktor internal dan eksternal.

## Rumusan Masalah Bisnis 
Apartemen di daerah Daegu (Korea Selatan) menjadi salah satu pilihan tempat tinggal penduduk setempat akibat keterbatasan lahan dan tingginya kepadatan penduduk. Harga apartemen dipengaruhi oleh berbagai faktor internal seperti tipe apartemen, luas unit, dan usia bangunan, serta faktor eksternal seperti lokasi dan fasilitas di sekitarnya. Dalam praktiknya, pemilik apartemen atau perusahaan sering menetapkan harga berdasarkan pertimbangan pribadi, sehingga sulit untuk menyesuaikan dengan kondisi pasar. 
Penetapan harga yang terlalu tinggi dapat menyebabkan unit sulit terjual, sedangkan harga yang terlalu rendah dapat mengakibatkan kerugian finansial.
## Tujuan
Tujuan dari analisis ini adalah:

1. Menganalisis faktor internal dan eksternal utama yang memengaruhi harga apartemen di Daegu menggunakan data historis perumahan.
2. Membangun model machine learning berbasis regresi yang mampu memprediksi harga apartemen berdasarkan karakteristik properti dan fitur yang berkaitan dengan lokasi.
3. Meningkatkan akurasi penetapan harga dengan menyediakan estimasi harga yang objektif dan berbasis data sehingga mencerminkan kondisi pasar saat ini.

## Pendekatan Analitis
Metodologi *Data Science* yang digunakan dalam proyek untuk menjawab permasalahan bisnis sebagai berikut:
1. Data Understanding
    * Menggunakan data historis transaksi apartemen di Daegu yang mencakup harga sebagai variabel target serta berbagai fitur internal dan eksternal seperti luas unit, usia bangunan, lokasi, dan fasilitas di sekitar.
2. Exploratory Data Analysis (EDA)
    * Menganalisis distribusi data, korelasi, dan hubungan antara fitur dengan harga apartemen untuk mengidentifikasi faktor-faktor yang paling berpengaruh.

3. Data Preprocessing
   * Dataset di split menjadi data train dan test. Variabel kategorikal dikodekan, fitur numerik dinormalisasi atau diskalakan jika diperlukan.

4. Model Development
    * Membangun dan membandingkan beberapa model regresi, seperti Linear Regression sebagai baseline serta model yang lebih kompleks seperti Random Forest Regression atau Gradient Boosting Regression untuk menangkap hubungan non-linear.

5. Model Training and Validation
    * Membagi data menjadi data latih dan data uji atau menggunakan cross-validation untuk memastikan model dapat melakukan generalisasi dengan baik.

6. Model Selection and Optimization
    * Mengevaluasi kinerja model, melakukan tuning hyperparameter, dan memilih model terbaik berdasarkan hasil evaluasi.

7. Interpretation Model
    * Menjelaskan faktor-faktor apa saja dalam model yang mempengaruhi prediksi harga apartemen.

## Stakeholder
Pemangku kebijakan yang berpengaruh terhadap hasil dari prediksi apartemen diantaranya sebagai berikut:
* Investor/Pemilik Unit Apartemen
* Pembeli Apartemen
* Marketing Team.

## Metrics
Karena menggunakan model regresi, maka metrik evaluasi yang digunakan adalah:
1. Mean Absolute Error (MAE): Mengukur rata-rata selisih absolut antara harga prediksi dan harga aktual, sehingga mudah diinterpretasikan dalam satuan harga.
2. Root Mean Squared Error (RMSE): Memberikan penalti lebih besar pada kesalahan prediksi yang besar, sehingga cocok untuk meminimalkan kesalahan harga yang ekstrem.
3. R-squared (R²): Menunjukkan seberapa besar variasi harga apartemen dapat dijelaskan oleh model. Nilai yang lebih tinggi menunjukkan performa model yang lebih baik.
4. Mean Absolute Percentage Error (MAPE): Mengukur rata-rata kesalahan prediksi dalam bentuk persentase terhadap harga aktual, sehingga mudah dipahami sebagai tingkat kesalahan relatif model.
   
## 5 Point Business ML Goals
1. Problem : Terbatasnya lahan tidak sebanding dengan pertumbuhan penduduk sehingga muncullah apartemen sebagai solusi hunian di zaman modern ini.
2. Data : Menggunakan data historis transaksi apartemen di Daegu.
3. ML Objective : Membangun model regresi untuk memprediksi harga apartemen di Daegu berdasarkan faktor internal dan eksternal suatu unit.
4. Action : Menjadikan hasil prediksi sebagai referensi, dasar atau acuan dalam penetapan harga apartemen saat ingin melakukan transaksi.
5. Value : Meminimalisasi kekeliruan penetapan harga saat ingin menjual apartemen bagi pemilik unit. Adapun untuk pembeli apartemen, pembeli dapat mengetahui pasaran harga apartemen sebelum membeli suatu unit apartemen. Tim marketing dapat menyarankan unit dengan tepat sesuai kebutuhan dan budget yang dimiliki customer.

## Modul yang dibutuhkan untuk menjalankan program:
category_encoders >= 2.9.0
matplotlib >= 3.10.0
pandas >= 2.2.2
numpy >= 2.0.2
scikit-learn >= 1.6.1
seaborn >= 0.13.2
scipy => 1.16.3
sklearn-pandas >= 2.2.0
xgboost >= 3.1.2

Author : **Fatimah Azzahra, Gabriella Davintia, Tengku Arika Hazera**



