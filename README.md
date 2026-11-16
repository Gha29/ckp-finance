# CKP Finance V5 – Perbaikan Saldo & Sound Effect

1. Upload seluruh isi folder ini ke root repository GitHub Pages, branch `main`, timpa file lama.
2. Refresh aplikasi. Buat backup JSON sebelum melakukan impor ulang.
3. Impor ulang workbook Excel untuk menerapkan perbaikan pemetaan rekening tujuan transfer.
4. Periksa ringkasan impor, khususnya `transferWithoutDestination` yang harus 0. Jika bukan 0, jangan gunakan saldo sebagai angka final dan kirim ringkasannya.

V5 menambahkan sound effect Web Audio pada interaksi tombol (dengan pengaturan ON/OFF), memperbaiki normalisasi tujuan transfer, dan menambahkan diagnostik saldo saat impor. Data lama di localStorage tidak otomatis dihapus.
