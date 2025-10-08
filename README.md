# analisis faktor psikometri prediktif penggunaan ganja (cannabis) menggunakan decision tree dan smote

repositori ini menyimpan kode implementasi (*jupyter notebooks*) untuk tugas mata kuliah metode penelitian (metopen) program studi teknik informatika, universitas dian nuswantoro.

## tujuan penelitian

tujuan utama dari proyek ini adalah:
1.  **benchmarking model:** membandingkan kinerja prediktif antara algoritma **decision tree**, **support vector machine (svm)**, dan **gaussian naive bayes (gnb)** dalam tugas klasifikasi biner status pengguna ganja.
2.  **ekstraksi insight:** mengidentifikasi dan memeringkat **faktor psikometri** yang paling signifikan (prediktif) menggunakan fitur *feature importance* dari model terbaik.

## metodologi komputasi

penelitian ini menggunakan pendekatan *machine learning* terstruktur untuk menjamin validitas hasil:
1.  **data acquisition:** data diperoleh dari **drug consumption dataset** (fehrman & vahidi, 2018).
2.  **penanganan imbalance:** implementasi **smote (*synthetic minority over-sampling technique*)** untuk mengatasi masalah ketidakseimbangan kelas.
3.  **validasi:** pengujian model menggunakan skema **5-fold cross-validation (cv)**.
4.  **evaluasi kinerja:** metrik utama adalah **f1-score** dan **recall**, yang difokuskan pada **kelas 1 (pengguna)**.

## hasil kunci (key findings)

berdasarkan analisis *feature importance* pada model **decision tree** (model terbaik), temuan utama penelitian ini adalah:
* **prediktor dominan:** variabel **negara (*country*)** teridentifikasi sebagai prediktor terkuat.
* **faktor psikologi kritis:** faktor **sensation seeking (ss)** dan **impulsiveness** merupakan variabel psikometri yang paling signifikan dalam memprediksi status penggunaan.

## struktur repositori

| file / folder | deskripsi |
| :--- | :--- |
| `metopen.ipynb` | *jupyter notebook* utama yang berisi seluruh kode pra-pemrosesan, implementasi smote, *benchmarking* model, dan ekstraksi *feature importance*. |
| `data/drug_consumption.csv` | salinan *dataset* yang digunakan dalam penelitian. |
| `readme.md` | halaman utama repositori ini. |

## informasi proyek

disusun oleh: thalita nadia azalai
nim: a11.2023.15291
program studi: teknik informatika, universitas dian nuswantoro
tahun: 2025
