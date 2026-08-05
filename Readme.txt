SIDAP v1.5 CSR Final_Version
=============================

Deskripsi
---------
SIDAP adalah aplikasi manajemen data pelanggan, instalasi, dan permohonan air bersih untuk PDAM Kota Pematangsiantar. Aplikasi ini dibuat dengan Python Flask dan menggunakan SQLite sebagai basis data.

Fitur Utama
-----------
- Dashboard statistik pelanggan, instalasi, dan permohonan.
- Import data pelanggan dari file Excel.
- Import data permohonan masuk dan permohonan buka kembali dari Excel.
- Laporan bulanan dan laporan pertambahan sambungan.
- Pencarian pelanggan dan permohonan.
- CRUD untuk pelanggan, instalasi, dan permohonan.
- Ekspor data ke Excel.

Struktur Proyek
--------------
- app.py: file utama aplikasi Flask.
- templates/: folder template HTML untuk halaman aplikasi.
- static/: file CSS dan JavaScript untuk tampilan.
- data/: folder penyimpanan database SQLite (sidap.db).
- import_tmp/: folder sementara untuk file import.
- schema.sql: skrip inisialisasi basis data.

Persyaratan
-----------
- Python 3.8+ (direkomendasikan).
- Flask.
- openpyxl.
- SQLite (sudah terintegrasi dengan Python).

Instalasi
---------
1. Pastikan Python sudah terpasang.
2. Install dependensi:
   pip install flask openpyxl
3. Jalankan aplikasi:
   python app.py

Catatan
-------
- Aplikasi otomatis membuat database SQLite dan folder pendukung saat pertama kali dijalankan.
- File Excel import harus mengikuti format kolom yang sesuai dengan template yang disediakan.
- Backup database otomatis akan dibuat pada folder `backups` di direktori aplikasi.

Penggunaan
---------
1. Buka browser dan akses `http://127.0.0.1:5000`.
2. Gunakan menu untuk mengimpor data pelanggan atau permohonan.
3. Lihat statistik dan laporan dari dashboard.

Kontak
------
Untuk pengembangan lebih lanjut atau laporan bug, sesuaikan dengan pengembang proyek.
