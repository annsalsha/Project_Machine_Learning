# 📝 Text Classification & Sentiment Analysis Project

Proyek ini bertujuan untuk membangun model klasifikasi teks menggunakan dua pendekatan utama, yaitu machine learning dan deep learning. Dataset terdiri dari 1500 komentar YouTube yang mencakup data latih, data uji, serta dataset berlabel manual. Model yang dikembangkan mencakup SVM, Logistic Regression, Random Forest, LSTM, serta IndoBERT dengan LoRA.

---

## 📁 Struktur Folder

```
.
├── Dataset/
│   ├── Train.csv
│   ├── Test.csv
│   ├── Label.xlsx
│   └── youtube_comments.json
│
├── Laporan Machine Learning
│
├── Modeling/
│   ├── Machine Learning.ipynb
│   ├── LSTM.ipynb
│   ├── IndoBERT.ipynb
│   └── indobert_+_LoRa_XAI.ipynb
│
├── Scientific Research Poster
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

### *2. Deep Learning*

- LSTM (Long Short-Term Memory), Model berbasis RNN yang digunakan sebagai baseline untuk memahami urutan kata dalam teks.
- IndoBERT, Model transformer berbahasa Indonesia yang di-fine-tuning pada dataset komentar YouTube untuk menghasilkan representasi teks yang lebih kontekstual.
- IndoBERT + LoRA, Pengembangan dari IndoBERT dengan metode parameter-efficient fine-tuning (LoRA). Model ini menjadi model utama yang juga dianalisis menggunakan teknik Explainable AI (LIME dan SHAP).

Model ini dibandingkan performanya dengan model machine learning berbasis fitur.

---

## 🔍 Explainable AI (XAI)

Untuk memahami alasan model memberikan prediksi tertentu, proyek ini menggunakan:

1. LIME (Local Interpretable Model-Agnostic Explanations)

- Menjelaskan bagian kata yang paling berpengaruh pada prediksi model
- Memberikan interpretasi lokal terhadap satu sampel teks

2. SHAP (SHapley Additive ExPlanations)

- Memberikan skor kontribusi setiap kata
- Menyediakan interpretasi global dan lokal terhadap prediksi
- Digunakan terutama pada model IndoBERT + LoRA

Metode XAI ini membantu membuktikan bahwa model tidak hanya akurat, tetapi juga dapat dijelaskan (explainable).

---

## 📂 Dataset

Dataset berada pada folder Dataset/ dan terdiri dari:

- *Train.csv* → data pelatihan model  
- *Test.csv* → data pengujian model  
- *Label.xlsx* → dataset dengan label lengkap
- *youtube_comments.json* → dataset mentah

Dataset .csv memiliki kolom teks dan label yang digunakan untuk pelatihan dan evaluasi.

---

## ⚙ Alur Kerja Proyek

1. Preprocessing teks
2. Ekstraksi fitur (untuk ML)
3. Pelatihan model (ML & DL)
4. Evaluasi model
5. Dokumentasi hasil dan analisis

---

## 🎯 Tujuan

- Membandingkan performa Machine Learning, LSTM, dan IndoBERT + LoRA
- Menentukan teknik ekstraksi fitur terbaik untuk model ML
- Menggunakan model transformer sebagai baseline lanjutan
- Memberikan interpretasi prediksi model menggunakan XAI

---

## 🛠 Teknologi yang Digunakan

- Python 3.x
- TensorFlow / Keras
- Scikit-learn
- HuggingFace Transformers
- Pandas, NumPy
- Jupyter Notebook
- Matplotlib / Seaborn
- LIME
- SHAP
- PEFT (LoRA)
