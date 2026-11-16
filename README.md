# CKP Finance V6

Perbaikan rekonsiliasi saldo berdasarkan kolom bantu Excel `Efek ke Rek. Asal` dan `Efek ke Rek. Tujuan`. Ini mengikuti perhitungan workbook sumber untuk pemasukan, pengeluaran, transfer, utang, dan piutang. Sound effect V5 dipertahankan.

## Pemasangan
Unggah isi folder ini ke root repository branch `main`, timpa file lama, lalu commit. Setelah deploy, buat backup JSON sebelum impor ulang. Impor ulang workbook akan mengganti data modul hasil impor.

## Verifikasi
Setelah impor, ringkasan menampilkan `computedAccountTotal`. Cocokkan dengan total `Saldo Saat Ini` di sheet Rekening Excel. Untuk workbook yang diberikan, targetnya Rp3.110.452. Verifikasi akhir tetap perlu dilakukan di browser.
