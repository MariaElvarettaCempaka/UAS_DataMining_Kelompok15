# Steam Game Success Analyzer

## Deskripsi

Steam Game Success Analyzer merupakan aplikasi berbasis Streamlit yang dikembangkan untuk menganalisis potensi kesuksesan game pada platform Steam menggunakan teknik Data Mining dan Machine Learning. Aplikasi ini mengimplementasikan metode klasifikasi dan clustering untuk memberikan analisis serta rekomendasi berbasis data historis game Steam.

Project ini dibuat sebagai pemenuhan Ujian Akhir Semester Mata Kuliah Data Mining Program Studi Sistem Informasi, Universitas Negeri Surabaya.

---

## Anggota Kelompok 15

| Nama | NIM |
|--------------------------------------|--------------|
| Daniel Evan Rusli | 24051214009 |
| Azzahra Anggarista Yoan Putri | 24051214032 |
| Maria Elvaretta Cempaka Ayu S. | 24051214033 |

---

## Struktur Project

```
UAS_DataMining_Kelompok15/
│
├── dataset/
├── notebook/
│   └── analysis.ipynb
├── model/
│   └── model.pkl
├── app/
│   ├── app.py
│   ├── pages/
│   └── assets/
├── laporan/
│   └── laporan.pdf
├── requirements.txt
└── README.md
```

---

## Dataset

Dataset yang digunakan adalah **Steam Games Dataset** yang diperoleh dari HuggingFace.

**Sumber Dataset**

https://huggingface.co/datasets/FronkonGames/steam-games-dataset

**Karakteristik Dataset**

- Total data : 124.146 game
- Total atribut : 41 kolom sebelum preprocessing
- Rentang data : 1997–2026
- Tidak terdapat missing value

---

## Metode yang Digunakan

### Data Preparation

- Data Cleaning
- Feature Engineering
- One Hot Encoding
- StandardScaler
- SMOTE (Synthetic Minority Over-sampling Technique)

### Supervised Learning

- Gradient Boosting Classifier
- Random Forest Classifier
- Logistic Regression

### Unsupervised Learning

- K-Means Clustering

---

## Teknologi

- Python 3.11
- Streamlit
- Pandas
- NumPy
- Scikit-learn
- Imbalanced-learn
- Plotly
- Matplotlib
- Joblib
- Jupyter Notebook

---

## Fitur Aplikasi

- Home
- Dataset Overview
- Prediction
- Visualization
- About

---

## Cara Menjalankan Project

### 1. Clone Repository

```bash
git clone https://github.com/MariaElvarettaCempaka/UAS_DataMining_Kelompok15.git
```

### 2. Masuk ke Folder Project

```bash
cd UAS_DataMining_Kelompok15
```

### 3. Install Seluruh Dependency

```bash
pip install -r requirements.txt
```

### 4. Jalankan Aplikasi

```bash
streamlit run app/app.py
```

---

## Hasil Model

| Model | AUC-ROC |
|-------------------------|---------|
| Gradient Boosting | 0.8732 |
| Random Forest | 0.8688 |
| Logistic Regression | 0.7654 |

Model terbaik yang digunakan pada aplikasi ini adalah **Gradient Boosting Classifier** karena memiliki nilai AUC-ROC tertinggi.

---

## Repository

Repository ini berisi:

- Source code aplikasi Streamlit
- Notebook analisis Data Mining
- Model Machine Learning
- Dataset
- Laporan UAS
- File requirements.txt
- File README.md

---

## Laporan

Laporan penelitian tersedia pada folder:

```
laporan/
```

---

## Lisensi

Project ini dikembangkan untuk keperluan akademik sebagai pemenuhan tugas Ujian Akhir Semester Mata Kuliah Data Mining Program Studi Sistem Informasi Universitas Negeri Surabaya.