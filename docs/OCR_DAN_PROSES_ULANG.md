# OCR dan proses ulang dokumen

## Metadata dahulu atau langsung OCR?

Pada **Kelola data → Cara menambahkan PDF**:

- **Catat metadata saja** dicentang: simpan nama, tahun dan referensi sumber. PDF Drive tidak diunduh.
- Tidak dicentang: sesudah metadata sumber dicatat, berkas baru atau yang belum diekstraksi dapat dilanjutkan ke ekstraksi/OCR.

Mode Otomatis mencoba teks yang sudah tersedia pada PDF terlebih dahulu. Mode OCR
melakukan pembacaan gambar. PDF hasil scan tidak selalu memiliki lapisan teks;
keberhasilan pengenalan bergantung pada kualitas scan dan tata letaknya.

Untuk Drive, SINTESA **mengunduh satu PDF → mengekstraksi/OCR → menghapus salinan
sementara → lanjut ke PDF berikutnya**. File asli di Drive tidak dihapus.
Batas unduhan ekstraksi **1 GB per PDF**; preview Drive tetap **200 MB**.
Berkas lebih besar diberi keterangan gagal dan antrean berlanjut. Besar batas
bukan jaminan kinerja baik pada komputer RAM 4 GB.

## Melengkapi berkas yang belum diekstraksi

Pilih ulang PDF/folder yang diperlukan melalui Tambah PDF, atau gunakan Perbarui
folder. Matikan Catat metadata saja sebelum memulai. Sumber yang tersedia pada
pilihan itulah yang diproses; sinkronisasi biasa tidak mengulang hasil selesai.

## Mengulang satu dokumen

Pilih dokumen di Ruang arsip, tekan **Proses ulang**, lalu periksa pengaturan
sumbernya di Kelola data. Gunakan sumber tersimpan, ganti dengan PDF lokal, atau
link PDF Drive yang sesuai. Drive memerlukan konfigurasi, login, dan izin akun.

## Mengulang OCR folder

1. Matikan Catat metadata saja dan pilih mode Otomatis/OCR.
2. Buka **Perbarui folder**, tampilkan daftar folder, lalu pilih satu folder.
3. Tekan **Proses ulang OCR** dan periksa pratinjau.
4. Pilih status yang akan diproses. Secara default seluruh status dipilih kecuali **Selesai**.
5. Tinjau jumlah pilihan lalu mulai. Pilihan status berlaku pada seluruh halaman pratinjau.

Hanya arsip dengan referensi sumber yang sudah tertaut dan layak yang masuk
pratinjau. PDF baru, konflik, nama tidak valid, atau sumber tidak tersedia perlu
ditangani melalui alur tambah/sinkronisasi yang sesuai.

Sebelum proses ulang folder, SINTESA membuat cadangan database. Jika cadangan
gagal, OCR tidak dimulai. Metadata manual/rekap dan referensi sumber dipertahankan;
hasil ekstraksi lama dapat diganti ketika berkas mulai diproses. Jika gagal setelah
tahap itu, hasilnya dapat menjadi gagal; cadangan tetap tersedia. Belum ada tombol
pemulihan cadangan. Minta bantuan pengelola sebelum mengganti database.

## Memantau hasil

Buka **Progres pemrosesan**. Klik Riwayat tambah & sinkronisasi data untuk membuka
riwayat yang tersimpan; rincian kegiatan dibuka dari daftar. Pembatalan tidak
menghapus hasil berkas yang sudah selesai.

Pada Detail dokumen, **Metadata** mengelompokkan nilai yang sudah tercatat;
**Detail OCR** menjelaskan status dan ringkasan ekstraksi. Status Selesai berasal
dari proses otomatis, bukan persetujuan atau jaminan kebenaran metadata. Kandidat
nama/NIK perlu verifikasi dan tidak dipasangkan otomatis. Teks OCR lengkap baru
tidak disimpan atau ditampilkan sebagai isi detail.

[Kembali ke panduan](README.md)
