# Pertukaran metadata dan ekspor laporan

## Kegunaan paket .sintesa

Buka **Kelola data → Pindahkan data** untuk mengirim atau menerima katalog metadata
antarkomputer SINTESA. Paket bukan PDF dan **bukan cadangan lengkap aplikasi**.

| Ikut paket | Tidak ikut paket |
| --- | --- |
| Nama PDF, DI/tahun, metadata rekap/manual dan kandidat hasil ekstraksi | File PDF dan teks OCR lengkap |
| Referensi file Drive serta folder Drive terdaftar | Path dan folder lokal |
| Hubungan sumber/folder dan riwayat ringkas yang tercatat | Semua log kegiatan/permintaan lama |
| Perlindungan koreksi manual yang didukung paket | Token, credentials, sesi/persetujuan client, dan Detail OCR per halaman |

Metadata arsip asal PDF lokal tetap dapat ikut walaupun tidak punya link Drive;
path lokalnya tidak ikut. Riwayat folder tidak membuktikan semua PDF selesai OCR
atau masih dapat diakses. Daftar sumber rekap Google Sheets tersimpan tidak ikut.

## Mengekspor

Pilih lokasi dan nama paket, lalu tunggu selesai. Ekspor memuat seluruh koleksi,
bukan hanya hasil pencarian/halaman yang terlihat. Tidak membaca atau mengunduh PDF.

Batas paket utama: 100.000 arsip, ukuran paket 1 GiB dan isi terurai 2 GiB; ada
batas jumlah kandidat/folder/hubungan sumber yang juga berlaku. Batas bukan
jaminan semua kombinasi data muat atau sudah diuji pada komputer kantor.
Paket tidak otomatis dibagi dan belum ada pemilihan tahun.

## Mengimpor

1. Pilih paket dan tunggu pemeriksaan; belum ada perubahan koleksi pada tahap ini.
2. Tinjau kategori baru, lengkapi dan konflik. Periksa nama paket yang sedang ditinjau.
3. Terapkan seluruh data valid. Tindakan berlaku lintas halaman, bukan halaman terlihat saja.
4. Nilai kosong dapat dilengkapi. Nilai berbeda, identitas ganda atau koreksi manual yang dilindungi ditahan sebagai konflik.
5. Periksa folder Drive yang masuk: folder baru nonaktif/belum diperiksa. Hubungkan Google, periksa dan aktifkan sesuai kebutuhan.

Jika pemeriksaan paket baru gagal, pratinjau lama dapat tetap tersedia; pastikan
nama paket sebelum menerapkan. Impor tidak mengunduh PDF, melakukan OCR, atau
memulihkan persetujuan akses client. Impor ulang paket sama tidak membuat duplikat.
Arsip yang tidak terdapat dalam paket tidak dihapus.

## Jika proses dibatalkan atau terputus

Hasil arsip yang sudah diterapkan tetap tersimpan. Paket yang sudah diperiksa dapat
dilanjutkan secara eksplisit, termasuk setelah aplikasi dibuka kembali. Jangan
mengganti pratinjau bila masih ingin melanjutkan paket tersebut.

Cadangan database dibuat sebelum penerapan pertama paket. Belum ada tombol
pemulihan atau penghapusan cadangan otomatis. Sediakan ruang disk dan minta bantuan
pengelola sebelum mengganti database. Simpan paket/cadangan sesuai aturan kantor.

## Laporan kegiatan dan permintaan PDF

Buka **Kelola data → Laporan → Pusat ekspor log**, lalu pilih:

- Pemrosesan/sinkronisasi: ringkasan kegiatan atau rincian sumber.
- Permintaan akses PDF: ringkasan permintaan atau riwayat keputusan/kejadian.

Ekspor CSV memuat seluruh riwayat jenis yang dipilih, lintas halaman. Belum ada
filter tanggal atau impor log kembali. Laporan hasil impor paket dapat disimpan
terpisah dari pratinjau. Ekspor log bukan cara memindahkan sesi atau persetujuan client.

[Kembali ke panduan](README.md)
