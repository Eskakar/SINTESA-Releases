# Format nama PDF warkah

Nomor pada nama PDF adalah **No. DI 208**, berbeda dari Nomor Berkas pada kolom rekap.

## Format yang diterima

- Satu nomor: `5018 TAHUN 2019.pdf`.
- Rentang meningkat: `3904-3909 TAHUN 2021.pdf`.
- Nomor positif; nol awal boleh, misalnya `0001 Tahun 2025.PDF`.
- Tepat satu spasi sebelum dan sesudah TAHUN. Tahun tepat empat digit.
- Huruf besar/kecil TAHUN dan ekstensi PDF boleh berbeda.
- Tanpa spasi tambahan di awal/akhir nama, sekitar tanda hubung, atau sebelum `.pdf`.

Nomor akhir rentang harus lebih besar dari nomor awal. SINTESA tidak membetulkan
tahun atau mengganti nama PDF sumber secara otomatis.

| Nama | Hasil |
| --- | --- |
| `5018 TAHUN 2019.pdf` | Diterima |
| `003904-003909 Tahun 2021.pdf` | Diterima |
| `2888TAHUN 20018.pdf` | Ditolak: spasi dan tahun tidak sesuai |
| `1  TAHUN 2025.pdf` | Ditolak: spasi ganda |
| `0 TAHUN 2025.pdf` | Ditolak: nomor harus positif |
| `3909-3904 TAHUN 2021.pdf` | Ditolak: rentang terbalik |
| `surat.pdf` | Ditolak: bukan format warkah |

Format yang benar belum membuktikan isi PDF sudah sesuai; admin tetap memeriksa sumber.

## Jika nama ditolak

1. Buka **Kelola data → Laporan**, lalu buka pemeriksaan nama PDF.
2. Pilih laporan yang diperlukan dan baca nama serta alasannya.
3. Gunakan pencarian/pindah halaman untuk meninjau hasil, atau **Simpan seluruh nama ditolak** untuk CSV seluruh penolakan laporan tersebut.
4. Perbaiki nama pada file/folder sumber, lalu pilih atau periksa folder kembali.

Berkas valid tetap dapat diproses meskipun ada berkas lain yang ditolak. Nama yang
tidak sesuai tidak diubah otomatis. Pemeriksaan nama arsip yang sudah tercatat
tidak menghapus arsip lama, mengganti nama, atau menjalankan OCR.

## Nama dari rekap

Uraian seperti `Berkas Pelayanan No DI 208: 9767 Tahun 2025` membentuk nama
`9767 Tahun 2025.pdf`. Nomor Berkas tetap mengikuti kolom Nomor Berkas, bukan angka DI.
`No DI 208: sdnsd1212 Tahun 2019` atau `No DI 208: 33Tahun 2010` ditolak.

Rentang disimpan sebagai satu identitas. `3904-3909` tidak dipecah menjadi enam
arsip dan tidak otomatis dianggap sama dengan arsip tunggal `3904`.

[Kembali ke panduan](README.md)
