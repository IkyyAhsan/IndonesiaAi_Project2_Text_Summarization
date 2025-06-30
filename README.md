# Project 2: Text Summarization using IndoBERT

## Rizky Ahsan Syarif

Proyek ini bertujuan untuk membangun model ringkasan teks menggunakan arsitektur IndoBERT. IndoBERT merupakan model yang telah dilatih sebelumnya pada teks Bahasa Indonesia, dan proyek ini memanfaatkannya untuk melakukan extractive text summarization, yang berfokus pada artikel-artikel dari Liputan6. Tujuan utama dari proyek ini adalah untuk menghasilkan model yang dapat merangkum artikel berita dalam Bahasa Indonesia secara otomatis dan efisien.

## 🎯 Tujuan Proyek

- Membangun dan menyempurnakan model IndoBERT pada dataset Liputan6 untuk meringkas artikel dalam Bahasa Indonesia.
- Mengevaluasi kinerja model menggunakan berbagai metrik seperti ROUGE dan BERTScore.

## Dataset

Kumpulan data yang digunakan dalam proyek ini adalah Ringkasan Liputan6, yang terdiri dari artikel-artikel beserta ringkasannya. Kumpulan data tersebut dibagi menjadi set pelatihan, validasi, dan pengujian.
- Training data: 27,000 articles
- Test data: 3,000 articles
Dataset diproses terlebih dahulu dengan menghapus kolom yang tidak diperlukan dan membersihkan data untuk kompatibilitas model.

# Model Training
Model ini didasarkan pada IndoBERT, yang disesuaikan untuk ringkasan ekstraktif. Proses pelatihan mencakup beberapa langkah, seperti praproses data, penyiapan model, pelatihan, dan evaluasi.

## Training Configuration
- Batch Size: 4
- Learning Rate: 2e-5
- Epochs: 3

## Training Output:
- Epoch 1/3
- Training Epoch 100% | 2625/2625 [04:35<00:00, 9.53it/s]
- Training loss: 0.0051
- Epoch 2/3
- Training Epoch 100% | 2625/2625 [04:34<00:00, 9.56it/s]
- Training loss: 0.0002
- Epoch 3/3
- Training Epoch 100% | 2625/2625 [04:34<00:00, 9.56it/s]
- Training loss: 0.0003

## Model Evaluation
- ROUGE-1 F-measure: 1.0000
- ROUGE-2 F-measure: 1.0000
- ROUGE-L F-measure: 1.0000
- BERTScore Precision: 1.0000
- BERTScore Recall: 1.0000
- BERTScore F1: 1.0000

Model ini mencapai kinerja yang sangat baik pada ROUGE dan BERTScore, dengan skor sempurna di semua aspek. Penggunaan ukuran batch yang kecil dan presisi campuran (fp16) untuk pelatihan secara signifikan mengurangi waktu pelatihan sambil mempertahankan kinerja yang tinggi. Model ini sekarang siap digunakan dalam tugas-tugas ringkasan ekstraktif di dunia nyata.
