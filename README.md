UTS Data Acquisition & Management
Analisis dan Penggabungan Data Pariwisata Yogyakarta
Proyek ini merupakan pengerjaan UTS mata kuliah Data Acquisition & Management. Notebook digunakan untuk memperoleh, memeriksa, membersihkan, dan menggabungkan data pariwisata Yogyakarta dari beberapa sumber.
Tujuan
1. Mengakuisisi dan memeriksa dataset pariwisata dari Kaggle.
2. Membersihkan data serta menghitung estimasi kebutuhan storage berdasarkan ukuran file aktual.
3. Mengambil data cuaca historis melalui Open-Meteo Archive API.
4. Memeriksa kebijakan robots.txt sebelum melakukan scraping situs Visiting Jogja.
5. Menormalisasi nama destinasi dan menggabungkan data dengan mempertahankan seluruh baris destinasi dari dataset utama.
6. Menyimpan provenance, metadata, dan checksum untuk mendokumentasikan proses akuisisi serta pengolahan data.
Sumber Data
Sumber	Data yang digunakan	Tautan
Kaggle – Dataset Pariwisata Yogyakarta	tour.csv, tour_rating.csv, user.csv	https://www.kaggle.com/datasets/saufan/dataset-pariwisata-yogyakarta
Open-Meteo Archive API	Data cuaca historis untuk satu titik koordinat Kota Yogyakarta	https://archive-api.open-meteo.com/v1/archive
Visiting Jogja	Judul dan tautan artikel wisata dari halaman yang diizinkan oleh robots.txt
