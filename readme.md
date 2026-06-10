# STEAM GAME SUCCESS ANALYZER

## Sistem Analisis Prediksi Kesuksesan Game Berbasis Machine Learning

---

## 1. Deskripsi Sistem

**Steam Game Success Analyzer** merupakan aplikasi berbasis *Streamlit* yang dikembangkan untuk menganalisis potensi kesuksesan game pada platform Steam menggunakan pendekatan **Data Mining** dan **Machine Learning**.

Sistem ini mengimplementasikan metode **supervised learning (classification)** dan **unsupervised learning (clustering)** untuk menghasilkan prediksi serta insight berbasis data historis game Steam.

Proyek ini disusun sebagai pemenuhan Ujian Akhir Semester Mata Kuliah **Data Mining**, Program Studi **Sistem Informasi, Universitas Negeri Surabaya**.

---

## 2. Identitas Kelompok

| Nama | NIM |
|------|------|
| Daniel Evan Rusli | 24051214009 |
| Azzahra Anggarista Yoan Putri | 24051214032 |
| Maria Elvaretta Cempaka Ayu S. | 24051214033 |

---

## 3. Struktur Direktori Sistem

```
UAS_DataMining_Kelompok15/
│
├── app/
│   ├── pages/
│   │   ├── __pycache__/
│   │   ├── about.py
│   │   ├── dataset.py
│   │   ├── home.py
│   │   ├── prediction.py
│   │   └── visualization.py
│   └── app.py
│
├── dataset/
│   └── data.zip
│
├── laporan/
│   └── laporan.pdf
│
├── model/
│   ├── metadata.json
│   └── prediction_model.pkl
│
├── notebook/
│   └── analysis.ipynb
│
├── readme.md
├── requirements.txt
└── video.txt
```

---

## 4. Dataset yang Digunakan

Dataset yang digunakan adalah **Steam Games Dataset** dari HuggingFace.

### Karakteristik Dataset:
- Jumlah data: 124.146 entri game
- Jumlah fitur: 41 kolom (sebelum preprocessing)
- Rentang tahun: 1997 – 2026
- Missing value: tidak ditemukan pada dataset utama

---

## 5. Metodologi Penelitian

### 5.1 Data Preparation
- Data Cleaning  
- Feature Engineering  
- One Hot Encoding  
- Standardization (StandardScaler)  
- Handling imbalance (SMOTE)

### 5.2 Supervised Learning
- Gradient Boosting Classifier  
- Random Forest Classifier  
- Logistic Regression  

### 5.3 Unsupervised Learning
- K-Means Clustering  

---

## 6. Teknologi yang Digunakan

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

## 7. Fitur Sistem

- Home (Halaman Utama)  
- Dataset Overview  
- Prediction System  
- Data Visualization  
- About System  

---

## 8. Hasil Evaluasi Model

| Model | AUC-ROC |
|------|--------|
| Gradient Boosting Classifier | **0.8732** |
| Random Forest Classifier | 0.8688 |
| Logistic Regression | 0.7654 |

Model terbaik: **Gradient Boosting Classifier**

---

## 9. Cara Menjalankan Aplikasi (Local)

### 1. Clone Repository
```bash
git clone https://github.com/MariaElvarettaCempakaCempaka/UAS_DataMining_Kelompok15.git
```

### 2. Masuk Folder Project
```bash
cd UAS_DataMining_Kelompok15
```

### 3. Install Library
```bash
pip install -r requirements.txt
```

### 4. Jalankan Aplikasi
```bash
streamlit run app/app.py
```

### 5. Buka di Browser
```
http://localhost:8501
```

---

## 10. Catatan Penting

- Aplikasi hanya dijalankan secara **lokal (offline)**
- Dataset berada di `dataset/data.zip` (tidak perlu diekstrak manual)
- Pastikan Python sudah terinstall sebelum menjalankan aplikasi

---

## 11. Kesimpulan

Steam Game Success Analyzer berhasil mengimplementasikan machine learning untuk menganalisis dan memprediksi kesuksesan game berdasarkan data Steam. Model terbaik yang digunakan adalah Gradient Boosting Classifier dengan performa AUC-ROC tertinggi.

---

## 12. Lisensi

Proyek ini dibuat untuk kebutuhan akademik Ujian Akhir Semester Mata Kuliah Data Mining, Program Studi Sistem Informasi, Universitas Negeri Surabaya.

© 2026 Kelompok 15
