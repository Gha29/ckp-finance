# CKP Finance — Paket awal

## Isi paket
- `index.html`: aplikasi utama; dashboard, transaksi CRUD, rekening, anggaran, laporan ringkas, neraca ringkas, modul utang/piutang/tabungan/investasi/aset/asuransi, sound effect, backup JSON, export CSV, dan import CSV.
- `manifest.webmanifest`: metadata PWA.
- `sw.js`: cache dasar untuk akses offline setelah kunjungan pertama.
- `icon.svg`: ikon aplikasi.

## Pasang ke GitHub Pages
1. Ekstrak ZIP di HP.
2. Buka repository GitHub `ckp-finance`.
3. Pilih Add file → Upload files.
4. Unggah ISI folder ini ke root repository (jangan unggah folder pembungkusnya).
5. Commit perubahan ke branch yang digunakan GitHub Pages.
6. Refresh website. Jika tampilan lama masih muncul, tutup tab lalu buka ulang atau bersihkan cache situs.

## Catatan penting
- Data disimpan lokal di browser dengan localStorage; tidak otomatis sinkron antarperangkat.
- Buat backup JSON berkala. Jangan hapus data browser sebelum backup.
- Import transaksi mendukung CSV dan Excel `.xlsx`/`.xls` (pembaca Excel dimuat dari CDN sehingga perlu internet saat impor), dengan kolom: tanggal,jenis,nominal,kategori,rekening,catatan. `jenis` berisi `income` atau `expense`.
- Import XLSX langsung, sinkronisasi cloud, login, enkripsi, transfer antar rekening, dan neraca akuntansi berpasangan memerlukan pengembangan dan pengujian lanjutan.
- Ini paket fondasi yang dapat diuji dan dikembangkan, bukan aplikasi final siap produksi.
