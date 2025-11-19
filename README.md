# 📝 Text Classification & Sentiment Analysis Project

Proyek ini bertujuan untuk membangun model klasifikasi teks menggunakan dua pendekatan utama, yaitu machine learning dan deep learning.Dataset terdiri dari 1500 data komentar YouTube yang mencakup data latih, data uji, serta dataset berlabel manual. Model yang dikembangkan mencakup SVM, Logistic Regression, Random Forest, dan LSTM.

---

## 📁 Struktur Folder

```
.
├── Dataset/
│   ├── Train.csv
│   ├── Test.csv
│   └── Label.xlsx
│
├── Laporan/
│   └── (file laporan proyek)
│
├── Modeling/
│   ├── lstm.ipynb               # Preprocessing + Model Deep Learning (LSTM)
│   └── preprocess_ml.ipynb      # Preprocessing + Machine Learning
│
└── README.md
```

---

## 📘 Deskripsi Proyek

Proyek ini melakukan klasifikasi teks untuk menentukan label tertentu berdasarkan isi teks. Pendekatan yang digunakan:

### *1. Machine Learning*
Menggunakan beberapa algoritma klasik:

- Support Vector Machine (SVM)
- Logistic Regression
- Random Forest

Dengan beberapa metode ekstraksi fitur:

- *Bag of Words (BoW)*
- *BoW + N-Gram*
- *TF-IDF*
- *TF-IDF + N-Gram*

Tujuan dari eksperimen ini adalah membandingkan performa setiap algoritma dengan berbagai variasi representasi fitur.

---

### *2. Deep Learning (LSTM)*

Model LSTM digunakan untuk mempelajari konteks urutan kata secara mendalam. Tahapan yang dilakukan:

- Tokenisasi & padding
- Embedding layer
- LSTM layer
- Dense layer untuk klasifikasi

Model ini dibandingkan performanya dengan model machine learning berbasis fitur.

---

## 📂 Dataset

Dataset berada pada folder Dataset/ dan terdiri dari:

- *Train.csv* → data pelatihan model  
- *Test.csv* → data pengujian model  
- *Label.xlsx* → dataset dengan label lengkap  

Dataset memiliki kolom teks dan label yang digunakan untuk pelatihan dan evaluasi.

---

## ⚙ Alur Kerja Proyek

1. Preprocessing teks
2. Ekstraksi fitur (untuk ML)
3. Pelatihan model (ML & DL)
4. Evaluasi model
5. Dokumentasi hasil dan analisis

---

## 🎯 Tujuan

- Membandingkan metode ML dan DL pada tugas klasifikasi teks.
- Menentukan teknik ekstraksi fitur terbaik.
- Menyediakan baseline untuk penelitian NLP lebih lanjut.

---

## 🛠 Teknologi yang Digunakan

- Python 3.x  
- TensorFlow / Keras  
- Scikit-learn  
- Pandas, NumPy  
- Jupyter Notebook  
- Matplotlib / Seaborn  
