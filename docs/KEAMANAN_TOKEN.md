# Penyimpanan sesi Google SINTESA

Berlaku untuk SINTESA 1.2.0.

## Sesi Google di komputer admin

SINTESA menyimpan sesi Google dalam berkas terenkripsi `google-token.dpapi`,
bukan lagi `token.json` yang bisa dibaca sebagai teks. Tidak memerlukan password
SINTESA tambahan. Enkripsi terikat pada akun Windows yang menyimpannya.

Pada installer, lokasinya `%LOCALAPPDATA%\SINTESA\data\google-token.dpapi`.
`credentials.json` tetap konfigurasi aplikasi Google, terpisah dari token login;
perubahan ini tidak mengenkripsi file konfigurasi tersebut.

Token lama dipindahkan saat menghubungkan Google berikutnya. File lama baru
dihapus setelah berkas terenkripsi berhasil ditulis. Bila proses gagal, token
lama dipertahankan agar tidak hilang, tetapi SINTESA tidak beralih menyimpan
login baru sebagai teks biasa. Jangan menyebarkan cadangan token lama.
Penghapusan file bukan jaminan penghapusan forensik dari disk/backup.

Jika sesi tersimpan rusak atau tidak dapat dibuka oleh akun Windows saat ini,
SINTESA membuka proses login Google baru. Setelah login berhasil, sesi baru
disimpan dengan perlindungan akun Windows saat ini. Jangan mengandalkan penyalinan
token untuk pindah komputer; hubungkan akun Google kembali di komputer tujuan.

Keluar akun lokal menghapus berkas token terenkripsi dan token lama yang tersisa.
Tindakan ini tidak mencabut izin di Google atau menonaktifkan salinan token yang
sudah pernah dicuri. Pencabutan akses tetap melalui pengaturan akun Google.

## Batas perlindungan

DPAPI per pengguna melindungi isi berkas dari pembacaan langsung dan penggunaan
salinan melalui akun Windows lain pada keadaan normal. Perlindungan ini **tidak
mencegah program/orang yang menjalankan sesi Windows pengguna yang sama** untuk
mendapatkan akses. Pengguna komputer yang bisa memakai SINTESA yang sudah
terhubung tetap dapat memakai fitur Google yang tersedia. Administrator sistem,
malware dan kompromi akun Windows bukan ancaman yang diselesaikan enkripsi file
ini. Gunakan akun Windows terpisah dan kunci komputer saat ditinggalkan.

Mode OAuth Testing dan daftar Test users tetap dikelola Google Cloud. Enkripsi
tidak memperpanjang masa berlaku izin/token atau mengubah siapa yang boleh login.


[Kembali ke panduan](README.md)
