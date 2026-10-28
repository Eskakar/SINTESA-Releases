# Panduan pengguna SINTESA

SINTESA membantu pencarian dan pencatatan warkah. PDF asli tetap di sumbernya;
metadata disimpan di komputer admin. Instalasi: [Windows](../INSTALASI.md).

## 1. Catat arsip

Buka Kelola data dan pilih kegiatan sesuai sumber:

- **Tambah PDF → Dari komputer**: pilih PDF atau folder yang tersedia di komputer.
- **Tambah PDF → Dari Google Drive**: hubungkan Google di menu kiri, masukkan
  tautan folder, muat daftar dan proses pilihan yang diperlukan.
- **Isi dari rekap**: pilih Excel (.xlsx) atau CSV, cocokkan kolom, periksa hasil,
  lalu terapkan baris valid. Untuk Excel, pilih lembar yang berisi rekap.
  Untuk sumber online, buka Google Sheets, tempel link, muat rekap, pilih lembar
  dan periksa pemetaan yang sama. [Panduan rekap online](REKAP_ONLINE.md).

Biarkan Catat metadata saja aktif untuk pencatatan awal yang cepat. Nama, tahun
serta sumber PDF dicatat tanpa download/OCR PDF Drive. Rekap juga dapat mencatat
arsip yang PDF-nya belum tersedia. Ikuti [format nama PDF](NAMA_PDF.md).

No. DI 208 berasal dari identitas nama PDF/uraian Warkah 208. **Nomor Berkas**
adalah nomor administratif pada kolom rekap; keduanya merupakan informasi berbeda.
Contoh: nama PDF `345 TAHUN 2021.pdf` tidak otomatis berarti Nomor Berkas `345`.

## 2. Cari dan periksa

Pada Ruang arsip, ketik potongan nomor, tahun, nama PDF atau lokasi.
Hasil nomor DI yang cocok utuh didahulukan. Pilih dokumen untuk melihat Metadata,
ketersediaan sumber dan Detail OCR. Nilai yang belum tercatat ditampilkan `-`.

Gunakan Edit metadata untuk koreksi, Preview PDF untuk melihat halaman dokumen,
dan salin/buka link Drive bila tersedia. Link tersimpan tidak menjamin akun yang
digunakan saat itu masih memiliki izin Drive. Arsip dari rekap saja belum tentu
bisa dipreview sebelum PDF lokal atau Drive ditautkan.

## 3. Perbarui sumber dan OCR bila diperlukan

Perbarui folder menampilkan sumber yang pernah digunakan. Periksa pembaruan,
lalu sinkronkan folder aktif atau folder tertentu. Pengaturan PDF di atas berlaku
untuk tindakan tersebut. Sinkronisasi biasa tidak mengulang hasil yang sudah selesai.

OCR bersifat pilihan dan dapat membutuhkan waktu lama. Untuk melengkapi sumber
baru/belum diekstraksi, matikan Catat metadata saja sebelum menambah/sinkronkan.
Untuk mengulang hasil, pilih folder dan Proses ulang OCR folder. Tinjau status:
Selesai tidak dipilih secara default. Cadangan database dibuat sebelum proses ulang.

Progres pemrosesan menampilkan pekerjaan berjalan dan hasilnya. Klik judul Riwayat
tambah & sinkronisasi data untuk membuka riwayat tersimpan. Batal tidak menghapus
hasil yang sudah selesai. [Rincian Kelola data](KELOLA_DATA.md).

## 4. Pertukaran data dan laporan

Pindahkan data digunakan untuk paket `.sintesa` antarkomputer. Paket berisi metadata
serta referensi Drive, bukan PDF atau backup lengkap aplikasi. Periksa pratinjau
sebelum menerapkan. Pada Laporan, periksa nama PDF ditolak atau ekspor riwayat ke
CSV. [Cakupan paket dan ekspor](PERTUKARAN_DATA.md).

## 5. Layani pencarian melalui jaringan kantor

Pada Service web, nyalakan service lalu salin alamat jaringan untuk client pada
jaringan yang sama. Client memakai satu kolom pencarian untuk No. DI/nama PDF,
tahun, nomor berkas, lokasi, nama lengkap atau NIK utuh 16 digit yang sudah tercatat.
Hasil paling sesuai diutamakan; NIK tidak ditampilkan dalam hasil. Permintaan terbaru
terlihat di samping hasil pada desktop atau di atas hasil pada layar kecil.
Untuk permintaan lain, buka tab Permintaan saya atau tombol Lihat permintaan lainnya.
Riwayat memuat 50 permintaan terbaru browser ini; kembali ke Pencarian tidak
menghapus kata dan hasil pencarian.
Client dapat membuka preview halaman pertama tanpa
persetujuan. Akses PDF lengkap memerlukan persetujuan admin; hak akses Google
terhadap link PDF tetap berlaku. Service memakai HTTP tanpa login dan mati ketika
aplikasi ditutup. [Panduan jaringan](SERVICE_LAN.md).

## Hal yang perlu diingat

- Hasil OCR/kandidat bukan hasil yang otomatis terverifikasi; periksa dokumen.
- Sumber lokal perlu tetap tersedia; Drive membutuhkan konfigurasi, login dan izin.
- Kehilangan sumber tidak otomatis menghapus metadata arsip.
- Simpan data, ekspor dan cadangan secara terbatas; gunakan data sintetis untuk demo.
- Pemulihan backup belum memiliki tombol khusus. Minta bantuan pengelola komputer
  sebelum memindahkan atau mengganti database.

## Batas PDF Drive untuk ekstraksi

Unduhan untuk ekstraksi/OCR maksimal **1 GB (1.024 MiB) per PDF**. File lebih
besar diberi keterangan gagal dan antrean berlanjut ke berkas berikutnya. Ukuran
diperiksa sebelum dan selama unduhan; salinan unduhan yang gagal dibersihkan.
Metadata utama tetap dapat dicatat tanpa mengunduh PDF. Preview Drive tetap
dibatasi 200 MB; batas ini tidak mengubah pemrosesan PDF lokal.
