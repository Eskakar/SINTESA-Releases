# Menggunakan Kelola data

## Pembaruan 1.2.5

Folder utama Google Drive mencakup PDF dalam subfolder yang terlihat bagi akun.
Daftar menampilkan jalur subfolder dan progres; pemuatan dapat dibatalkan.
Shortcut tidak diikuti. Sinkronisasi biasa tidak mengulang OCR hasil selesai;
tahun dan DI tetap tidak ditebak dari folder. Batas satu sumber: 50.000 PDF,
10.000 folder termasuk root, dan 100 tingkat subfolder; jika terlampaui,
pemuatan gagal dengan keterangan, bukan menampilkan hasil terpotong.

Bantuan **?** di pojok panel dapat ditutup dengan klik di luar atau Escape.
Zoom admin 50–150% tersedia di header. Pada laporan nama ditolak, pilih satu
radio entri lalu **Simpan satu nama terpilih** untuk CSV nama/sumber/alasan.
Pilihan dibersihkan ketika daftar dirender ulang, termasuk saat pindah halaman.
Ini ekspor laporan, bukan unduhan PDF. Ekspor seluruh laporan tetap tersedia.

Pilih kegiatan sesuai kebutuhan. Satu kelompok ditampilkan agar tidak perlu
membaca semua form sekaligus. Isi form dan pilihan tetap ada ketika berpindah.

| Kegiatan | Kapan digunakan | Langkah awal |
| --- | --- | --- |
| Tambah PDF | PDF belum dimasukkan atau ingin memilih sumber kembali | Pilih file/folder komputer, atau masukkan tautan folder Drive |
| Perbarui folder | Mencari PDF baru pada folder yang pernah digunakan | Periksa pembaruan, lalu sinkronkan folder aktif atau folder pilihan |
| Isi dari rekap | Mencatat nomor berkas, lokasi dan keterangan Excel/CSV/Google Sheets | Pilih file rekap, cocokkan kolom, periksa, lalu terapkan |
| Pindahkan data | Bertukar data dengan komputer SINTESA lain | Simpan paket .sintesa atau buka paket yang diterima |
| Laporan | Memeriksa nama PDF ditolak atau menyimpan riwayat | Buka pemeriksaan nama atau pusat ekspor log |

Pengaturan Cara menambahkan PDF berada paling atas dan berlaku untuk Tambah PDF
serta Perbarui folder. Default Catat metadata saja tidak mengunduh PDF Drive
untuk OCR. Jika dimatikan, sumber baru/Belum diekstraksi dapat dilanjutkan ke ekstraksi.
Pengaturan lanjutan OCR dapat dibuka pada bagian yang sama. Pengaturan ini tidak
mengubah penerapan rekap maupun paket pertukaran.

Folder tersimpan muncul otomatis dari sumber folder yang pernah digunakan.
Sinkronisasi biasa tidak mengulang hasil selesai. Untuk menggantinya, pilih folder
dan gunakan Proses ulang OCR folder, periksa pilihan status lalu mulai.

Paket SINTESA membawa metadata dan referensi Drive, bukan PDF atau cadangan lengkap
aplikasi. Log disimpan terpisah melalui Laporan. Pemantauan proses berjalan tetap
pada tab Progres pemrosesan. Referensi: [Pertukaran data](PERTUKARAN_DATA.md) dan
[Proses ulang folder](OCR_DAN_PROSES_ULANG.md).

Pada Progres pemrosesan, klik judul Riwayat tambah & sinkronisasi data untuk
membuka atau menutup daftar. Riwayat tertutup saat aplikasi dibuka dan tidak
terbuka otomatis ketika progres diperbarui.

## Rekap online

Pada Isi dari rekap tersedia sumber Google Sheets selain Excel/CSV. Hubungkan
Google, tempel link, pilih lembar, periksa pemetaan dan pratinjau, lalu terapkan.
Sumber pernah diterapkan dapat dimuat ulang dari daftar. Tidak sync otomatis.
[Petunjuk dan batas rekap online](REKAP_ONLINE.md).
