<p align="center"><img src="assets/sintesa-logo.png" width="220" alt="Lambang SINTESA"></p>

# SINTESA — Unduhan aplikasi

**Sistem Informasi & Temu Balik Berkas Pertanahan**

SINTESA membantu petugas mencatat, mengelola, dan mencari metadata warkah.
Repository ini menyediakan installer Windows, panduan penggunaan awal, dan catatan rilis.

## Unduh

[**Unduh SINTESA untuk Windows**](https://github.com/Eskakar/SINTESA-Releases/releases/latest)

Pada halaman rilis, buka **Assets**, lalu unduh installer sesuai nomor rilis.
Paket terbaru yang disiapkan lokal adalah `SINTESA-Setup-1.2.5-x64.exe`.
File **Source code (zip)** dan **Source code (tar.gz)** adalah arsip repository ini,
bukan installer aplikasi.

- Versi yang disiapkan: **1.2.5**
- Sistem: **Windows 10/11, 64 bit**
- [Panduan untuk admin dan pihak BPN](docs/README.md)
- [Panduan pengguna sehari-hari](docs/PANDUAN_PENGGUNA.md)
- [Panduan instalasi](INSTALASI.md)
- [Catatan rilis 1.2.5](catatan-rilis/1.2.5.md)

## Fitur utama

- Pencarian metadata warkah, termasuk No. DI 208, nomor berkas, tahun, dan lokasi.
- Pencatatan sumber PDF lokal dan Google Drive, dengan pilihan mencatat metadata dahulu.
- Pengisian metadata dari rekap Excel, CSV, dan Google Sheets.
- Preview dokumen, ekstraksi/OCR opsional, serta pembaruan folder sumber.
- Service jaringan lokal untuk pencarian client, preview halaman pertama, dan permintaan akses PDF penuh kepada admin.
- Pertukaran paket metadata dan ekspor laporan kegiatan.

Tesseract beserta bahasa Indonesia/Inggris sudah disertakan. Tidak perlu memasang
Python atau Tesseract secara terpisah. Microsoft Edge WebView2 Runtime diperlukan.
Fitur Google memerlukan konfigurasi dan akun yang diberi akses; impor lokal dapat
digunakan tanpa konfigurasi Google.

## Pemeriksaan file unduhan

Setiap rilis menyediakan checksum SHA-256. Petunjuk pemeriksaan tersedia di
[panduan instalasi](INSTALASI.md#memeriksa-file-unduhan).

## Bantuan

Laporkan masalah melalui [Issues](https://github.com/Eskakar/SINTESA-Releases/issues)
dengan versi aplikasi dan langkah untuk mengulang masalah. Jangan menyertakan
token, credentials, PDF warkah, NIK, atau data pribadi dalam laporan publik.

Repository ini khusus distribusi aplikasi dan dokumentasi publik; source code
aplikasi tidak disertakan di sini.
