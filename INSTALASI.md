# Instalasi SINTESA di Windows

## Kebutuhan

- Windows 10 atau 11, 64 bit.
- Microsoft Edge WebView2 Runtime.
- Koneksi internet untuk fitur Google Drive/Google Sheets.

Python, Tesseract, serta model OCR Indonesia/Inggris sudah dibundel.
Performa OCR bergantung pada jumlah halaman dan kemampuan komputer. Ukuran PDF
maksimal yang diterima bukan jaminan OCR akan cepat pada komputer RAM 4 GB.

## Memasang aplikasi

1. Buka [halaman rilis](https://github.com/Eskakar/SINTESA-Releases/releases/latest).
2. Unduh installer `.exe` dari bagian Assets.
3. Jalankan installer dan ikuti petunjuknya. Instalasi dilakukan untuk pengguna Windows saat ini.
4. Buka SINTESA dari menu Start atau shortcut yang dibuat.

Jika WebView2 belum tersedia, installer mencoba memasangnya menggunakan internet.
Untuk komputer offline, siapkan WebView2 Runtime terlebih dahulu.

## Mulai menggunakan

- Untuk PDF lokal: buka **Kelola data → Tambah PDF → Dari komputer**.
- Biarkan **Catat metadata saja** aktif untuk pencatatan awal tanpa OCR.
- Untuk rekap: buka **Isi dari rekap**, pilih Excel/CSV atau Google Sheets.
- Cari arsip dan buka detailnya melalui **Ruang arsip**.

Nama PDF sumber memakai format `5018 TAHUN 2019.pdf`, atau rentang seperti
`3904-3909 TAHUN 2021.pdf`. Nomor harus positif dan tahun empat digit, dengan satu
spasi di sekitar TAHUN. Huruf besar/kecil TAHUN dan ekstensi PDF boleh berbeda.
Nama tidak sesuai akan dilaporkan untuk diperbaiki pada sumbernya.

No. DI 208 berbeda dari Nomor Berkas administratif pada rekap.

## Google Drive dan Google Sheets

Installer tidak menyertakan konfigurasi akun. Konfigurasi Google disiapkan pengelola
SINTESA melalui `credentials.json` pada `%LOCALAPPDATA%\SINTESA\credentials.json`.
Hubungkan Google melalui sidebar menggunakan akun yang mempunyai izin membaca
folder atau spreadsheet tujuan. Google Sheets API perlu aktif pada project Google
yang digunakan pengelola.

Untuk rekap online, gunakan **Google Spreadsheet asli**. File `.xlsx` yang hanya
disimpan di Drive dapat diunduh untuk impor lokal, atau disimpan sebagai Google
Spreadsheet terlebih dahulu.

Unduhan PDF Drive untuk ekstraksi/OCR dibatasi **1 GB per PDF** dan diproses satu
per satu. Preview Drive dibatasi **200 MB**. Mencatat metadata saja tidak mengunduh PDF.

## Memperbarui aplikasi dan menyimpan data

Tutup SINTESA sebelum menjalankan installer versi baru. Lokasi program terpisah
dari data pengguna. Cadangkan database saat aplikasi ditutup sebelum pembaruan.

- Data: `%LOCALAPPDATA%\SINTESA\data\waska.db`
- Log startup: `%LOCALAPPDATA%\SINTESA\logs\startup.log`

Token Google disimpan terenkripsi untuk akun Windows yang digunakan. Token lama
dipindahkan saat menghubungkan Google berikutnya. Jika berpindah komputer/akun
Windows, login Google kembali; jangan membagikan token. Orang yang memakai akun
Windows yang sama tetap dapat memakai aplikasi yang sudah terhubung.

## Memeriksa file unduhan

Unduh `SHA256SUMS-1.2.0.txt` dari rilis yang sama dengan installer. Di PowerShell,
jalankan pada folder unduhan:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath '.\SINTESA-Setup-1.2.0-x64.exe'
```

Bandingkan nilai Hash dengan checksum pada rilis. Untuk versi lain, sesuaikan
nama installer dan file checksum. Jika nilainya berbeda, unduh kembali file dari
halaman rilis yang benar.

## Catatan versi 1.2.0

Uji executable lulus untuk UI, OCR, service lokal, dan enkripsi token Windows.
Pemasangan/upgrade versi ini belum diuji otomatis pada instalasi baru karena
komputer pengujian sudah memiliki instalasi SINTESA. Uji kantor dan akun Google
live tetap perlu dilakukan sesuai kondisi setempat.

## Panduan pemakaian selanjutnya

Buka [panduan admin dan pihak BPN](docs/README.md) untuk Kelola data, rekap, OCR,
pertukaran metadata serta service client jaringan kantor.
