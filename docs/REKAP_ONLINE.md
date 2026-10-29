# Mengambil metadata dari Google Sheets

Gunakan sumber **Google Spreadsheet asli**, bukan file Excel (.xlsx) yang hanya
tersimpan di Drive. Untuk Excel, gunakan impor file lokal atau pilih File →
Simpan sebagai Google Spreadsheet di Google Sheets terlebih dahulu.

## Langkah admin

1. Hubungkan akun Google melalui sidebar. Akun harus diberi akses baca ke rekap.
2. Buka **Kelola data → Isi dari rekap → Ambil rekap dari Google Sheets**.
3. Tempel link Google Sheets dan tekan **Muat / perbarui rekap online**.
4. Pilih lembar yang benar, periksa nama sumber dan cocokkan judul kolom.
5. Tekan **Periksa kecocokan**, tinjau hasil, lalu terapkan pilihan atau seluruh baris valid.

No. DI 208 dan tahun dibaca dari uraian Warkah 208; Nomor Berkas berasal dari
kolom Nomor Berkas. Identitas DI yang belum ada dapat dibuat sebagai arsip baru
meskipun PDF-nya belum ditautkan. Nama yang tidak valid dan konflik tidak diterapkan.
Nilai yang dilindungi karena koreksi manual tidak ditimpa begitu saja.

## Memakai rekap yang sama lagi

**Sumber online pernah diterapkan** berisi Google Sheets yang sebelumnya sudah
berhasil diterapkan, bukan hanya dimuat. Pilih sumber, lalu muat/perbarui rekap.
Tersimpan link, lembar, nama sumber, pemetaan kolom, dan waktu penerapan.
Pemetaan dipakai kembali jika susunan header masih sama; tetap periksa sebelum menerapkan.

Pemuatan mengambil keadaan rekap pada saat itu. Jika rekap di Google berubah,
muat ulang untuk membaca perubahan. Tidak ada sinkronisasi terjadwal otomatis.
SINTESA tidak menulis ke spreadsheet, mengunduh PDF, atau menjalankan OCR lewat alur ini.

## Kebutuhan dan batas

- Pengelola menyiapkan konfigurasi Google dan mengaktifkan Google Sheets API.
- Tanpa konfigurasi/login, fitur online tidak aktif; file Excel/CSV lokal tetap dapat dipakai.
- Akun Google harus mempunyai akses; rekap tidak perlu dibagikan ke publik.
- Maksimal 10.000 baris data dan ukuran data 20 MB.
- Lembar online maksimal 10.030 baris termasuk header dan 100 kolom, termasuk baris/kolom kosong. Kurangi grid kosong berlebih atau gunakan lembar yang lebih kecil jika ditolak.

Daftar sumber Google Sheets tersimpan belum ikut paket `.sintesa`; metadata yang
sudah diterapkan tetap mengikuti cakupan [pertukaran data](PERTUKARAN_DATA.md).

Jika gagal, baca pemberitahuan: periksa jenis file, link, akun yang terhubung,
izin rekap dan koneksi. Jika perlu bantuan, sampaikan teks pesan kepada pengelola
SINTESA tanpa mengirim credentials, token, atau data pribadi ke laporan publik.

[Kembali ke panduan](README.md)

## Pembaruan paket 1.2.1

Pemuatan menampilkan tahap dan baris yang dibaca. Sel kosong di ujung baris
diterima. Jika masih ada data setelah judul kolom terakhir, lengkapi judul kolom
atau pindahkan catatan di luar tabel sebelum mencoba lagi.
