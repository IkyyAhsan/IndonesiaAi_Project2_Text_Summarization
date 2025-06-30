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
- 
Dataset diproses terlebih dahulu dengan menghapus kolom yang tidak diperlukan dan membersihkan data untuk kompatibilitas model.
