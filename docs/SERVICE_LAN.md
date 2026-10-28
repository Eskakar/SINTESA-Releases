# Service web dan pencarian client di jaringan kantor

## Menyalakan sebagai admin

1. Buka SINTESA → **Service web**. Service mati saat awal aplikasi dibuka.
2. Pilih jaringan LAN kantor, periksa port, lalu nyalakan service.
3. Salin alamat jaringan yang ditampilkan dan bagikan kepada client pada jaringan yang sama.
4. Gunakan alamat IP jaringan kantor; `127.0.0.1` hanya dapat dipakai di komputer admin.
5. Bila tidak terhubung, periksa jaringan, isolasi Wi-Fi dan izin firewall bersama pengelola komputer.

Aplikasi tidak mengatur router/firewall otomatis. Matikan service jika tidak
dipakai; menutup SINTESA juga menghentikannya. Riwayat tetap tersimpan, tetapi
service tidak otomatis menyala lagi saat aplikasi dibuka.

## Mencari sebagai client

Buka alamat dari admin melalui browser. Pada tab **Pencarian**, gunakan satu kolom
untuk No. DI/nama PDF, tahun, nomor berkas, lokasi, nama lengkap atau NIK utuh
16 digit yang sudah tercatat. Hasil paling sesuai diutamakan: nama PDF/DI/tahun
file, lalu nomor berkas dan metadata lain. Belum ada pembetulan salah ketik otomatis.

Pencarian nama/NIK bergantung pada metadata yang sudah ada; tidak menjalankan OCR
saat mencari. NIK dan daftar nama kandidat tidak ditonjolkan dalam hasil utama.
Nama dan NIK tidak dipasangkan otomatis sebagai satu identitas.

## Preview dan PDF lengkap

- **Preview halaman pertama** langsung dibuka tanpa permintaan/persetujuan admin.
- Preview berupa gambar halaman pertama; gunakan zoom bila diperlukan.
- Untuk **PDF lengkap**, kirim permintaan dengan nama dan keperluan, lalu tunggu keputusan admin.

Preview memakai sumber admin: PDF lokal jika tersedia, atau Drive yang dapat
diakses akun admin. Untuk Drive, satu PDF penuh perlu diunduh sementara sebelum
halaman pertama dirender; bukan hanya mengunduh satu halaman. Batas preview Drive
200 MB. File sementara dibersihkan; gambar dapat disimpan sementara untuk mempercepat
permintaan berikutnya. Karena itu preview Drive dapat lebih lambat.

Client dapat melihat gambar preview tanpa izin akun Google client. Tidak ada
penyamaran data otomatis pada gambar halaman pertama.

## Menangani permintaan

Permintaan menunggu keputusan muncul pada aplikasi admin. Periksa pemohon,
keperluan, sumber/link PDF dan catatan, lalu terima atau tolak. Admin dapat memilih
masa persetujuan **1, 8 atau 24 jam**; pilihan awal 1 jam.

Persetujuan menampilkan link PDF Drive kepada pemohon. Izin akun Google pemohon
tetap berlaku; menerima permintaan tidak otomatis membagikan file di Google Drive.
Batas waktu mengatur akses melalui SINTESA, bukan mencabut izin Google atau
menarik kembali link/file yang sudah disalin/diperoleh.

Halaman utama client hanya menampilkan **permintaan terbaru**. Untuk lainnya,
buka navbar **Permintaan saya** atau **Lihat permintaan lainnya**. Riwayat menampilkan
50 permintaan terbaru pada browser yang sama. Berpindah tab tidak menghapus pencarian.
Menghapus cookie atau berpindah browser membuat riwayat sesi lama tidak terlihat
di client tersebut; catatan admin tetap tersedia.

Di admin, permintaan aktif berisi yang masih menunggu. Keputusan dan kejadian
lain dapat diperiksa melalui log permintaan. Ekspor tersedia di Kelola data →
Laporan → Pusat ekspor log.

## Batas penggunaan jaringan

Service ini untuk **jaringan kantor tepercaya**, memakai HTTP tanpa login SINTESA
atau HTTPS. Nama pemohon diisi sendiri dan bukan identitas terverifikasi. Jangan
membuka service ke internet melalui penerusan port router.

Aplikasi membatasi beban permintaan dan preview, bukan jumlah orang tetap.
Saat sibuk, tunggu lalu coba lagi. Pembatasan beban bukan pengganti pengamanan
jaringan kantor. Jika PDF hanya lokal dan tidak punya link Drive, preview mungkin
tersedia, tetapi akses PDF penuh melalui link Google belum tersedia.

[Kembali ke panduan](README.md)
