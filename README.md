# Analisis Sentimen Ulasan WhatsApp

Proyek ini bertujuan untuk melakukan analisis sentimen terhadap ulasan aplikasi WhatsApp yang diambil dari Google Play Store. Ulasan diklasifikasikan ke dalam tiga kategori sentimen: **positif**, **netral**, dan **negatif**, menggunakan pendekatan berbasis lexicon dan tiga skema pelatihan machine learning.

## Deskripsi Proyek
Proyek ini terdiri dari dua bagian utama:
1. **Scraping Data**: Mengambil ulasan WhatsApp dari Google Play Store menggunakan library `google-play-scraper`.
2. **Analisis Sentimen**: Melakukan pra-pemrosesan data, pelabelan sentimen, pelatihan model, dan evaluasi menggunakan tiga skema:
   - Skema 1: Decision Tree + TF-IDF
   - Skema 2: Random Forest + TF-IDF
   - Skema 3: Deep Learning (CNN)

## Dataset
- Sumber: Ulasan WhatsApp dari Google Play Store (bahasa Indonesia).
- Jumlah Data: 64.000 ulasan.
- Kelas Sentimen: Positif, Netral, Negatif.

## Struktur File
- `scraping_ulasan.py`: File untuk mengambil ulasan dari Google Play Store dan menyimpannya ke `ulasan_whatsapp.csv`.
- `analisis_sentimen.py`: File untuk pra-pemrosesan, pelabelan, pelatihan model, dan inference.
- `ulasan_whatsapp.csv`: File CSV berisi ulasan mentah hasil scraping.
- `processed_ulasan_whatsapp.csv`: File CSV berisi data yang sudah diproses (setelah pra-pemrosesan dan pelabelan).
- `requirements.txt`: Daftar library yang diperlukan untuk menjalankan proyek.
- `README.md`: Dokumentasi proyek ini.

## Prasyarat
Pastikan Anda memiliki Python 3.7 atau lebih tinggi. Instal semua dependensi dengan menjalankan:
```bash
pip install -r requirements.txt
