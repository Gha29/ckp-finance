# CKP Finance – Paket V2

Web app/PWA untuk pencatatan keuangan pribadi.

## Isi paket
- `index.html`: aplikasi dan logika fitur.
- `manifest.webmanifest`: metadata PWA.
- `sw.js`: cache dasar.
- `icon.svg`: ikon aplikasi.

## Pembaruan V2
- Impor workbook Excel `.xlsx` / `.xls` langsung melalui SheetJS (memerlukan internet saat library dimuat).
- Membaca dan mengarsipkan semua sheet workbook.
- Preview nama sheet dan jumlah baris sebelum impor.
- Pemetaan data utama: Rekening, Kategori, Transaksi, Anggaran Bulanan, Utang Saya, Piutang Saya, Tabungan, Investasi, Aset Tetap, Asuransi.
- Export transaksi CSV dan backup JSON.

## Instalasi GitHub Pages
1. Ekstrak ZIP.
2. Di repository pilih Add file → Upload files.
3. Upload seluruh isi folder ini ke root repository, timpa file lama.
4. Commit ke branch yang digunakan GitHub Pages.
5. Buka situs dengan koneksi internet, lalu lakukan refresh.

## Catatan penting
- Import membaca nilai yang tersimpan di sel Excel; rumus Excel tidak dieksekusi oleh aplikasi.
- Semua sheet disimpan sebagai arsip lokal di browser bersama data hasil pemetaan. Penyimpanan browser memiliki batas kapasitas; buat backup JSON setelah impor.
- Data lokal tidak otomatis sinkron antarperangkat.
- Neraca dan dashboard CKP menghitung dari model data aplikasi, bukan menjalankan ulang seluruh rumus dan tampilan Excel.
- Sebelum impor, ekspor backup data aplikasi yang sudah ada. Impor workbook menggantikan data utama yang bersesuaian.
