# 🚕 NYC Taxi Fare Analysis & Prediction
### Big Data Processing and Machine Learning with PySpark

<p align="center">
  **Analyzing and Predicting NYC Yellow Taxi Trip Fares Using Distributed Data Processing**
</p>

<p align="center">
  <a href="https://github.com/tanzz15/Analisis-dan-Prediksi-Menggunakan-Pyspark-dan-Algoritma-Machine-Learning/blob/main/5638_DAN_5641_UAS_BDL.ipynb">
    📓 View Jupyter Notebook
  </a>
</p>

---

## 📌 About the Project

Proyek ini merupakan implementasi **Big Data Analytics dan Machine Learning** untuk menganalisis serta memprediksi total tarif perjalanan taksi Yellow Taxi di New York City.

Dataset yang digunakan adalah **NYC Yellow Taxi Trip Record – January 2021**, yang berisi lebih dari satu juta catatan perjalanan.

Pengolahan data dilakukan menggunakan Apache Spark melalui PySpark untuk menerapkan konsep pemrosesan data berskala besar. Tahapan proyek meliputi batch processing dengan konsep MapReduce, Exploratory Data Analysis (EDA), data preprocessing, manipulasi data menggunakan Spark SQL, hingga pembangunan dan evaluasi model Machine Learning.

Dua algoritma regresi digunakan untuk membandingkan performa prediksi, yaitu Linear Regression dan Random Forest Regression. Model Random Forest kemudian dioptimalkan menggunakan CrossValidator untuk memperoleh performa prediksi yang lebih baik.

## 🎯 Project Objectives

- Menerapkan konsep Big Data Processing menggunakan Apache Spark.
- Memahami pemrosesan batch dengan konsep MapReduce.
- Melakukan eksplorasi dan analisis dataset perjalanan taksi.
- Mengolah data menggunakan PySpark dan Spark SQL.
- Membangun model regresi untuk memprediksi total tarif perjalanan.
- Membandingkan performa Linear Regression dan Random Forest Regression.
- Melakukan hyperparameter tuning untuk meningkatkan performa model.

## 🔄 Data Processing Pipeline

### 1. Data Loading
Mengunduh dan memuat dataset NYC Yellow Taxi Trip Record Januari 2021 ke dalam Spark DataFrame.

### 2. Batch Processing
Menerapkan konsep pemrosesan batch dan MapReduce untuk memahami pengolahan data dalam lingkungan terdistribusi.

### 3. Exploratory Data Analysis (EDA)
Mengeksplorasi karakteristik dataset, termasuk:
- Jumlah penumpang (`passenger_count`).
- Jarak perjalanan (`trip_distance`).
- Total tarif perjalanan (`total_amount`).
- Distribusi dan hubungan antarvariabel.

### 4. Data Preprocessing
Melakukan pemeriksaan dan persiapan data sebelum digunakan dalam proses pemodelan.

### 5. Spark SQL
Memanfaatkan kemampuan Spark untuk melakukan manipulasi dan analisis data.

### 6. Machine Learning
Membangun dua model regresi:
- Linear Regression.
- Random Forest Regression.

### 7. Hyperparameter Tuning
Mengoptimalkan Random Forest menggunakan CrossValidator dengan konfigurasi 3-fold validation.

### 8. Model Evaluation
Mengevaluasi performa model menggunakan:
- Root Mean Squared Error (RMSE).
- Mean Squared Error (MSE).
- R-squared (R²).

## 🤖 Machine Learning Models

| Model | Configuration |
|---|---|
| Linear Regression | Model regresi linear |
| Random Forest Regression | 20 trees, max depth 5 |
| Tuned Random Forest | CrossValidator, 3 folds |

Hyperparameter tuning menggunakan kombinasi:
- `numTrees`: 10 dan 20.
- `maxDepth`: 5 dan 10.

## 📊 Model Evaluation Results

Berikut hasil evaluasi yang diperoleh dari eksperimen dalam notebook:

| Model | RMSE | MSE |
|---|---:|---:|
| Linear Regression | 12.7946 | 163.7026 |
| Random Forest | 8.5111 | 72.4396 |
| **Tuned Random Forest** | **8.4104** | **70.7356** |

### Random Forest Before vs After Tuning

| Metric | Before Tuning | After Tuning |
|---|---:|---:|
| RMSE | 8.5111 | **8.4104** |
| MSE | 72.4396 | **70.7356** |
| R² | 0.5581 | **0.5685** |

**Key Findings:**

- Random Forest menghasilkan RMSE lebih rendah dibandingkan Linear Regression.
- Hyperparameter tuning berhasil menurunkan RMSE dan MSE.
- Nilai R² meningkat dari 0.5581 menjadi 0.5685 setelah tuning.
- Tuned Random Forest memberikan hasil terbaik di antara model yang diuji.

## 🛠️ Technologies & Tools

| Technology | Purpose |
|---|---|
| Python | Programming Language |
| Apache Spark | Distributed Data Processing |
| PySpark 3.5.0 | Big Data Processing Framework |
| Spark SQL | Data Manipulation and Analysis |
| Java 17 | Runtime Environment for Apache Spark |
| Spark MLlib | Machine Learning and Model Evaluation |
| Matplotlib | Data Visualization |
| Seaborn | Data Visualization |
| Google Colab | Notebook Development Environment |

## 📂 Dataset

**NYC Yellow Taxi Trip Record – January 2021**

Dataset berisi informasi perjalanan taksi Yellow Taxi di New York City, termasuk waktu penjemputan, waktu pengantaran, jumlah penumpang, jarak perjalanan, dan komponen biaya perjalanan.

Target prediksi:
- `total_amount`

Dataset diunduh langsung melalui notebook dari sumber data NYC TLC yang tersedia di GitHub DataTalksClub.

## 🚀 How to Run

Proyek ini dikembangkan menggunakan Google Colab.

1. Buka notebook melalui tautan berikut:

   [5638_DAN_5641_UAS_BDL.ipynb](https://github.com/tanzz15/Analisis-dan-Prediksi-Menggunakan-Pyspark-dan-Algoritma-Machine-Learning/blob/main/5638_DAN_5641_UAS_BDL.ipynb)

2. Buka notebook menggunakan Google Colab.
3. Jalankan setiap cell secara berurutan.
4. Pastikan Google Drive sudah terhubung apabila menggunakan penyimpanan yang dikonfigurasi di notebook.
5. Notebook akan menyiapkan Java, PySpark, library pendukung, dan dataset yang diperlukan.

## 🎓 Project Scope

Proyek ini dikembangkan sebagai tugas akhir mata kuliah **Big Data Learning (BDL)** dengan fokus pada penerapan pemrosesan Big Data dan Machine Learning untuk menyelesaikan permasalahan prediksi tarif perjalanan.

---

<p align="center">
  **Big Data Analytics | PySpark | Machine Learning**
  <br />
  Developed by <a href="https://github.com/tanzz15">tanzz15</a>
</p>
