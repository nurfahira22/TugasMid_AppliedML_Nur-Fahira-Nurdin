# TugasMid_AppliedML_Nur-Fahira-Nurdin
# 🎓 Analisis Prediksi Risiko Putus Sekolah (School Dropout Prediction)

> **Tugas Besar Mata Kuliah Applied Machine Learning**
>
> **Topik:** Prediksi Risiko Putus Sekolah Tingkat Provinsi Berbasis Indikator Sumber Daya Sekolah.

## 📋 Deskripsi Proyek
Proyek ini bertujuan untuk membangun model Machine Learning yang dapat memprediksi tingkat putus sekolah (*dropout rate*) di berbagai provinsi di Indonesia. Analisis dilakukan berdasarkan data statistik sekolah terbaru tahun 2025 yang mencakup rasio guru, kepadatan kelas, dan kinerja siswa.

Proyek ini mengikuti standar metodologi **CRISP-DM** (*Cross Industry Standard Process for Data Mining*) mulai dari pemahaman bisnis hingga deployment aplikasi.

## 📂 Dataset
Dataset yang digunakan berasal dari **Pusat Data dan Teknologi Informasi Kemendikdasmen** (Statistik Sekolah 2024/2025).
* **Sumber Data:** Data Terbuka Kemendikdasmen (https://data.kemendikdasmen.go.id/)
* **Fitur Utama:** Jumlah Siswa, Guru, Ruang Kelas, Siswa Mengulang, Status Sekolah.

## ⚙️ Alur Pengerjaan (Methodology)
1.  **Data Preparation:** Pembersihan data, penanganan *missing values*, dan *Feature Engineering* (membuat variabel rasio: `Student_Teacher_Ratio`, `Class_Crowdedness`, `Repeater_Rate`).
2.  **Modeling:** Melatih dan membandingkan dua algoritma:
    * **Decision Tree Regressor**
    * **Random Forest Regressor**
3.  **Evaluation:** Menggunakan metrik **MAE** (*Mean Absolute Error*) dan **R-Squared**, serta validasi silang (*Cross-Validation*).
4.  **Deployment:** Implementasi model menggunakan framework **Gradio** untuk simulasi interaktif.

## 📊 Hasil Analisis
Berdasarkan hasil pemodelan, ditemukan bahwa faktor yang paling dominan mempengaruhi risiko putus sekolah adalah:
1.  **Repeater Rate** (Persentase siswa tinggal kelas) - *Pengaruh Tertinggi*
2.  **Student Teacher Ratio** (Rasio beban guru)

Model terpilih adalah Random Forest karena memiliki tingkat error yang paling rendah pada data uji.

