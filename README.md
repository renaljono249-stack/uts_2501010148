# Pariwisata Yogyakarta

## 1. Identitas Mahasiswa

- **Nama:** Renala Febrian Jono
- **NIM:** 2501010148
- **Program Studi:** Informatika
- **Perguruan Tinggi:** Institut Bisnis dan Teknologi Indonesia (INSTIKI)
- **Mata Kuliah:** Data Acquisition & Management
- **Kelas:** F
- **Tahun Akademik:** 2026/2027
- **Topik Proyek:** Pariwisata Yogyakarta

## 2. Deskripsi Proyek

Proyek ini bertujuan untuk melakukan pengumpulan, pemeriksaan, pembersihan, pengolahan, dan penggabungan data yang berkaitan dengan pariwisata di Yogyakarta.

Data diperoleh melalui tiga metode, yaitu:

1. Open Dataset dari Kaggle.
2. API Open-Meteo.
3. Web Scraping dari website Visiting Jogja.

## 3. Sumber Data

### A. Open Dataset – Kaggle

**Nama Dataset:** Dataset Pariwisata Yogyakarta

**URL:** https://www.kaggle.com/datasets/saufan/dataset-pariwisata-yogyakarta

File:
- `tour.csv`
- `tour_rating.csv`
- `user.csv`

### B. API – Open-Meteo

**URL:** https://api.open-meteo.com/v1/forecast

**Lokasi:** Yogyakarta

**Koordinat:**
- Latitude: -7.8014
- Longitude: 110.3647

**Variabel:**
- Temperature
- Rain
- Wind Speed
- Weather Code

### C. Web Scraping – Visiting Jogja

**Website:** https://visitingjogja.jogjaprov.go.id/

**Halaman Scraping:** https://visitingjogja.jogjaprov.go.id/wisata-jogja/

**Jumlah Data Hasil Scraping:** 107 data unik.

## 3. Proses Pengolahan Data

### A. Open Dataset

- Membaca file CSV.
- Memeriksa jumlah baris dan kolom.
- Memeriksa tipe data dan nilai kosong.
- Memeriksa data duplikat.
- Melakukan pembersihan data.
- Menyimpan data hasil pembersihan.

### B. API

- Mengakses API Open-Meteo.
- Memeriksa status HTTP.
- Menggunakan timeout dan mekanisme retry.
- Mengambil data cuaca Yogyakarta.
- Mengubah JSON menjadi tabel CSV.
- Menyimpan data mentah dan provenance.

### C. Web Scraping

- Memeriksa robots.txt.
- Mengakses halaman Visiting Jogja.
- Menggunakan Requests dan BeautifulSoup.
- Mengambil judul dan URL artikel wisata.
- Mengumpulkan data dari beberapa halaman.
- Menghapus data duplikat.
- Menghasilkan 107 data unik.

### D. Penggabungan Data

- Menggabungkan dataset Kaggle dan hasil scraping.
- Menggunakan metode Inner Join.
- Menggunakan nama tempat wisata sebagai kunci penghubung.
- Memeriksa duplikasi dan nilai kosong.
- Menyimpan hasil merge dan metadata.




## 4. Struktur Folder Proyek

```text
UTS_Renala_febrian_jono_2501010148/
│
│
├── data/
│   │
│   ├── raw/
│   │   │
│   │   ├── Api/
│   │   │   └── openmeteo_yogyakarta_raw.json
│   │   │
│   │   ├── download/
│   │   │   ├── tour.csv
│   │   │   ├── tour_rating.csv
│   │   │   └── user.csv
│   │   │
│   │   └── scraping/
│   │       ├── halaman_1.html
│   │       ├── halaman_2.html
│   │       ├── halaman_3.html
│   │       ├── halaman_4.html
│   │       ├── halaman_5.html
│   │       ├── halaman_6.html
│   │       ├── halaman_7.html
│   │       ├── halaman_8.html
│   │       ├── halaman_9.html
│   │       └── halaman_10.html
│   │
│   └── processed/
│       ├── data_ethics_checklist.csv
│       ├── hasil_merge_pariwisata_yogyakarta.csv
│       ├── hasil_normalisasi_api.csv
│       ├── metadata_merge.json
│       ├── openmeteo_yogyakarta.csv
│       ├── provenance_api.json
│       ├── provenance_scraping.json
│       ├── tour_clean.csv
│       ├── tour_rating_clean.csv
│       ├── user_clean.csv
│       ├── validasi_merge.json
│       └── visitingjogja_yogyakarta.csv
│
├── README.md
└── uts_dam.ipynb
```


