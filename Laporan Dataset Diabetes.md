Nama  : Andi Daniella Mezauri <br/>
NIM   : 09011282328083 <br/>
Kelas : SK3B <br/>

<h1> LAPORAN SINGKAT HASIL DARI EKSPLORASI DAN ANALISIS DATA </h1>
<h2> 1. Definisi Eksplorasi Data </h2>
<p> Dalam analisis data, dataset terdiri dari baris yang mewakili sampel dan kolom yang mewakili variabel. Setiap baris adalah entitas individu, sementara kolom menunjukkan karakteristik atau fitur dari setiap sampel. Saat menganalisis dataset, penting untuk memahami jumlah baris dan kolom sebagai ukuran data serta mengidentifikasi nilai yang hilang (**missing values**), yang dapat memengaruhi hasil analisis jika tidak ditangani dengan baik. Selain itu, outliers, atau nilai yang sangat berbeda dari mayoritas data, juga perlu diperhatikan, karena mereka bisa mendistorsi hasil analisis. Mengelola nilai yang hilang dan outliers sangat penting untuk memastikan analisis data yang akurat dan representatif. </p>

<h3> 1.1. Nama Dataset </h3>
Judul Data : Diabetes Dataset <br/>
Link : https://github.com/AndiDaniella/Andi-Daniella_09011282328083_DataMining_SK3B/blob/1de11ccf7b4de974a9f282a3187b95574ce0f6df/Diabetes%20dataset.ipynb <br/>

<h3> 1.2. Deskripsi Isi Dataset </h3>
Berikut deskripsi singkat untuk setiap variabel yang disebutkan: <br/>
* Pregnancies: Jumlah kehamilan yang dialami oleh seorang wanita, sering kali dikaitkan dengan risiko diabetes gestasional. <br/>
* Glucose: Tingkat glukosa darah (gula darah) dalam tubuh, faktor utama untuk mendiagnosis diabetes.<br/>
* BloodPressure: Tekanan darah diastolik (dalam mmHg), penting untuk mengetahui risiko hipertensi terkait diabetes.<br/>
* SkinThickness: Ketebalan lipatan kulit (dalam mm), digunakan untuk mengukur lemak subkutan sebagai indikator obesitas.<br/>
* Insulin: Jumlah insulin dalam darah (μU/mL), hormon yang mengatur kadar gula darah dan terkait erat dengan resistensi insulin.<br/>
* BMI: Indeks Massa Tubuh, rasio antara berat badan dan tinggi badan yang digunakan untuk mengkategorikan obesitas atau kekurangan berat badan.<br/>
* DiabetesPedigreeFunction: Skor yang mewakili risiko genetik seseorang untuk mengembangkan diabetes berdasarkan riwayat keluarga.<br/>
* Age: Usia subjek, karena risiko diabetes sering meningkat seiring bertambahnya usia.<br/>
* Outcome: Diagnosis akhir, 0 untuk non-diabetes dan 1 untuk diabetes. <br/>
Masing-masing variabel ini digunakan untuk menganalisis hubungan dengan risiko diabetes. <br/>

<h3>1.3. Identifikasi Dataset</h3>
1. Jumlah baris data set : 768 <br/>
2. Jumlah kolom data set : 9 <br/>
3. Missing Value : 0, berdasarkan hasil  didapatkan bahwa dataset ini tidak ada missing value. <br/>


<h2>2. Analisis Statistik Data</h2>
Statistik seperti rata-rata, median, mode, standar deviasi, variansi, skewness, dan kurtosis digunakan untuk memahami distribusi dan karakteristik data numerik dalam dataset. Ini memberikan gambaran awal tentang data yang dianalisis. <br/>
Berikut penjelasan dari hasil analisis dataset berdasarkan statistik deskriptif:

### 2.1 Mean (Rata-rata)
- **Pregnancies**: Rata-rata jumlah kehamilan dari sampel adalah 3.85 kali.
- **Glucose**: Rata-rata kadar glukosa dari sampel adalah 120.89 mg/dL.
- **BloodPressure**: Rata-rata tekanan darah diastolik adalah 69.11 mmHg.
- **SkinThickness**: Ketebalan kulit rata-rata adalah 20.54 mm.
- **Insulin**: Rata-rata kadar insulin adalah 79.80 μU/mL.
- **BMI**: Rata-rata indeks massa tubuh (BMI) dari sampel adalah 31.99.
- **DiabetesPedigreeFunction**: Rata-rata fungsi silsilah diabetes adalah 0.47, menunjukkan risiko genetik sedang.
- **Age**: Rata-rata usia dari sampel adalah 33.24 tahun.
- **Outcome**: Rata-rata outcome atau hasil diagnosis adalah 0.35, menunjukkan sekitar 35% sampel menderita diabetes.

### 2.2 Median
- **Pregnancies**: Setengah dari sampel memiliki jumlah kehamilan di bawah 3 dan setengah lagi di atas 3 kehamilan.
- **Glucose**: Setengah dari sampel memiliki kadar glukosa di bawah 117 mg/dL dan setengahnya di atas 117 mg/dL.
- **BloodPressure**: Tekanan darah diastolik median adalah 72 mmHg.
- **SkinThickness**: Setengah dari sampel memiliki ketebalan kulit di bawah 23 mm dan setengah lainnya di atas 23 mm.
- **Insulin**: Setengah dari sampel memiliki kadar insulin di bawah 30.5 μU/mL dan setengah di atasnya.
- **BMI**: Setengah dari sampel memiliki BMI di bawah 32 dan setengahnya di atas 32.
- **DiabetesPedigreeFunction**: Setengah dari sampel memiliki fungsi silsilah diabetes di bawah 0.37 dan setengah lainnya di atas 0.37.
- **Age**: Setengah dari sampel berusia di bawah 29 tahun dan setengahnya di atas 29 tahun.
- **Outcome**: Setengah dari sampel tidak menderita diabetes (outcome = 0), sedangkan setengah lainnya menderita diabetes (outcome = 1).

### 2.3 Mode (Modus)
- **Pregnancies**: Jumlah kehamilan yang paling sering muncul adalah 1.
- **Glucose**: Kadar glukosa yang paling sering muncul adalah 99 mg/dL.
- **BloodPressure**: Tekanan darah yang paling sering muncul adalah 70 mmHg.
- **SkinThickness**: Ketebalan kulit yang paling sering muncul adalah 0 mm, menunjukkan banyak sampel yang mungkin memiliki data hilang atau ketebalan kulit yang tidak diukur.
- **Insulin**: Nilai insulin yang paling sering muncul adalah 0 μU/mL, menunjukkan data hilang atau kadar insulin tidak diukur pada banyak sampel.
- **BMI**: Indeks massa tubuh yang paling sering muncul adalah 32.
- **DiabetesPedigreeFunction**: Fungsi silsilah diabetes yang paling sering muncul adalah 0.254.
- **Age**: Usia yang paling sering muncul dalam sampel adalah 22 tahun.
- **Outcome**: Nilai outcome yang paling sering muncul adalah 0, menunjukkan banyak sampel tidak menderita diabetes.

### 2.4 Standar Deviasi
- **Pregnancies**: Variasi atau penyebaran jumlah kehamilan dalam sampel adalah 3.37.
- **Glucose**: Variasi kadar glukosa adalah 31.97 mg/dL.
- **BloodPressure**: Variasi tekanan darah diastolik dalam sampel adalah 19.36 mmHg.
- **SkinThickness**: Variasi ketebalan kulit adalah 15.95 mm.
- **Insulin**: Penyebaran kadar insulin dalam sampel sangat besar dengan standar deviasi 115.24 μU/mL.
- **BMI**: Variasi BMI dalam sampel adalah 7.88.
- **DiabetesPedigreeFunction**: Variasi fungsi silsilah diabetes dalam sampel adalah 0.33.
- **Age**: Variasi usia sampel adalah 11.76 tahun.
- **Outcome**: Variasi hasil diagnosis adalah 0.48.

### 2.5 Variansi
- **Pregnancies**: Kuadrat dari standar deviasi menunjukkan variasi jumlah kehamilan sebesar 11.35.
- **Glucose**: Kuadrat dari standar deviasi menunjukkan variasi kadar glukosa sebesar 1022.25.
- **BloodPressure**: Variasi tekanan darah adalah 374.65.
- **SkinThickness**: Variasi ketebalan kulit adalah 254.47.
- **Insulin**: Variasi kadar insulin sangat tinggi, sebesar 13281.18.
- **BMI**: Variasi BMI adalah 62.16.
- **DiabetesPedigreeFunction**: Variasi fungsi silsilah diabetes adalah 0.11.
- **Age**: Variasi usia adalah 138.30.
- **Outcome**: Variasi hasil diagnosis adalah 0.23.

### 2.6 Skewness
- **Pregnancies**: Nilai skewness sebesar 0.90 menunjukkan distribusi jumlah kehamilan miring ke kanan (lebih banyak sampel dengan kehamilan rendah).
- **Glucose**: Skewness 0.17 menunjukkan distribusi glukosa sedikit miring ke kanan..
- **BloodPressure**: Skewness -1.84 menunjukkan distribusi tekanan darah diastolik sangat miring ke kiri (lebih banyak tekanan darah rendah).
- **SkinThickness**: Skewness 0.11 menunjukkan distribusi ketebalan kulit hampir simetris.
- **Insulin**: Skewness 2.27 menunjukkan distribusi insulin sangat miring ke kanan, menunjukkan banyak sampel dengan kadar insulin rendah.
- **BMI**: Skewness -0.43 menunjukkan distribusi BMI sedikit miring ke kiri.
- **DiabetesPedigreeFunction**: Skewness 1.92 menunjukkan distribusi sangat miring ke kanan, menunjukkan sebagian besar sampel memiliki skor rendah.
- **Age**: Skewness 1.13 menunjukkan distribusi usia miring ke kanan (lebih banyak sampel muda).
- **Outcome**: Skewness 0.64 menunjukkan distribusi outcome sedikit miring ke kanan.

### 2.7 Kurtosis
- **Pregnancies** dan variabel lainnya tidak diberikan data kurtosis rinci, namun kurtosis biasanya mengukur "ketajaman" atau puncak distribusi data.
<br/>
<h2>3. Korelasi Pada Dataset </h2>
<img src="https://github.com/user-attachments/assets/68a61800-0eb0-437a-8b8a-e20f699f7008" width=500/>

<h2>4. Visualisasi Data</h2>
<h3>4.1. Histogram</h3>
<img src="https://github.com/user-attachments/assets/586225e6-4e70-441f-a725-7a7a2e75f99b" width=500/>
  
<h3>4.2. Box Plot</h3>
<img src="https://github.com/user-attachments/assets/5fe05318-dc8c-48b3-85d6-b70c929f7f96" width=500/> 
<img src="https://github.com/user-attachments/assets/9d7e9536-db16-4704-b199-0a768fc3e72a" width=500/>
<img src="https://github.com/user-attachments/assets/b650fc7d-24cb-4712-91d2-f5955da8c89a" width=300/> 

<h3>4.3. Scatter Plot</h3>


<h2>5. Kesimpulan</h2>
<p> Berdasarkan analisis statistik deskriptif yang dilakukan, data menunjukkan bahwa variabel seperti Glucose, BloodPressure, dan Insulin memiliki rentang yang luas dengan deviasi standar dan varian yang tinggi, menandakan adanya variasi yang signifikan di antara nilai-nilai tersebut. Glucose memiliki rata-rata yang lebih tinggi dibandingkan dengan median, menunjukkan distribusi yang condong ke kanan, sementara BloodPressure dan Insulin menunjukkan distribusi yang cukup berbeda antara mean dan median. Selain itu, variabel seperti SkinThickness dan Insulin menunjukkan skewness yang tinggi, menunjukkan adanya kemungkinan outlier atau distribusi yang tidak simetris.</p>
<p> Kurtosis yang tinggi pada variabel Insulin dan BloodPressure mengindikasikan bahwa distribusi dari kedua variabel ini lebih tajam di pusatnya dibandingkan dengan distribusi normal, menandakan adanya banyak nilai ekstrem. Di sisi lain, variabel seperti Age dan Outcome menunjukkan distribusi yang lebih mendekati normal dengan kurtosis yang mendekati nol atau sedikit positif. Hasil ini memberikan wawasan penting dalam memahami karakteristik distribusi data, yang dapat mempengaruhi analisis lebih lanjut dan pengembangan model prediktif.</p>
