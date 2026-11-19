# UTS DAM - Analisis Data Pariwisata Bali

Integrasi dataset BPS (wisatawan domestik bulanan ke Bali 2004-2025), data cuaca Open-Meteo (titik Denpasar), dan satu tabel hasil web scraping.
sumber: https://bali.bps.go.id/id/statistics-table?subject=561

## Struktur
- data/raw/        : berkas mentah (BPS, open_meteo.json, scraping_destinasi.html, robots.txt)
- data/processed/  : bps_clean.csv, cuaca_clean.csv, destinasi_clean.csv, data_gabungan.csv
- metadata/        : provenance.csv, data_dictionary.csv, metadata_gabungan.json, robots_check.json, api_selection.json, validasi_merge.json
- ethics/          : data_ethics_checklist.csv

## Menjalankan
1. Letakkan CSV/XLS BPS domestik di data/raw/ (nama berkas memuat kata 'Domestik').
2. (Opsional) buat .env berisi BPS_API_KEY=... atau pakai Colab Secrets. Jangan commit .env.
3. Jalankan semua sel UTS_DAM_Pariwisata.ipynb dari atas.

## Atribusi
- Data: BPS Provinsi Bali (Hasil Survei Dinas Pariwisata Provinsi Bali).
- Weather data by Open-Meteo.com (CC BY 4.0).
- Tabel scraping: Wikipedia (CC BY-SA 4.0).

Dibuat: 2026-11-17 05:37:30
