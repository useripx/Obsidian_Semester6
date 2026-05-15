# FINAL REVISI PER ROLE (100% Sesuai Rekaman Dosen)

## 1. ROLE ANGGOTA

  

### Dashboard

- Total Pinjaman

- Total Angsuran

- Ringkasan kewajiban:

  - Simpanan Wajib

  - Simpanan Pokok

- Jika simpanan pokok belum lunas → tampilkan keterangan “Belum Lunas”

- Hapus bagian yang tidak relevan sesuai arahan dosen

  

### Profil / Setting

- Tambahkan:

  - Gaji / Penghasilan

  - Nomor rekening (Mandiri)

  - Nomor WA

  - Alamat lengkap

- Identitas:

  - NIK

  - NIP

  - NIY

  - NIDN

- Tombol “Lengkapi Data” untuk melihat dan menambahkan data profil

  

### Simpanan

- Menampilkan:

  - Riwayat transaksi

  - Total saldo

  - Total setoran

  - Total penarikan

- Riwayat transaksi dibuat per tahun

- Total tetap tampil seperti biasa

  

### Detail Simpanan

- Kolom anggota dihapus

- Diganti menjadi:

  - Simpanan Pokok

  - Simpanan Wajib

  - Simpanan Sukarela

  

### Pengajuan Pinjaman

- Saat klik “Ajukan Pinjaman” → popup:

  “Silakan simulasikan rencana pinjaman Anda terlebih dahulu”

- Setelah klik OK → masuk ke simulasi pinjaman

  

### Cetak Pernyataan

- Permohonan → bukan bermaterai

- Pernyataan → menggunakan materai

  

### Pelunasan

- Transfer bank menggunakan rekening Mandiri

- Status:

  - Belum Lunas

  - Lunas

  

### Simulasi Pinjaman

- Tambahkan:

  - Gaji saat ini (otomatis dari profil)

  - Gaji yang diterima per bulan

- Ubah istilah:

  - “Total Tagihan Per Bulan”

  menjadi

  - “Total Kewajiban Per Bulan”

  

### Pengaturan

- Ganti password tetap diperlukan

  

---

  

## 2. ROLE VALIDATOR

  

### Konfigurasi Simpanan

- Tambahkan:

  - Simpanan Motor

  - Simpanan Mobil

- Jika aktif → tampil di dashboard manager

- Jika nonaktif → tidak tampil

  

### Pendapatan Lain-Lain

- Tambahkan menu:

  - Pendapatan Lain-Lain

- Contoh:

  - Fotokopi

  - Pendapatan tambahan lainnya

- Fitur:

  - Input manual

  - Tombol plus (+)

  

### Reset Password User

- Popup reset password sudah ada

- Harus benar-benar terkirim ke user saat login

  

### Data untuk BAU

- Validator menyiapkan:

  - Status (Dosen / Karyawan)

  - NIDN / NIY

  - Nama

  - Jumlah kewajiban

  

---

  

## 3. ROLE MANAGER

  

### Dashboard

- Simpanan Wajib

- Simpanan Pokok

- Simpanan Sukarela

- Belanja

- Dana Sosial

- Simpanan Motor

- Simpanan Mobil

- Total Keseluruhan

  

### Pengaturan Suku Bunga

- Bisa mengatur bunga:

  - 1%

  - 0.6%

  - 1.5%

  - 2.5%

- Hapus tulisan “per bulan”

- Cukup gunakan persen (%)

  

### Generate Data Bulanan

- Manager melakukan generate data bulanan

- Digunakan untuk BAU download Excel

  

---

  

## 4. ROLE BAU

  

### Tampilan Data Potongan

Kolom:

1. Nomor

2. Status (Dosen / Karyawan)

3. NIDN / NIY

4. Nama

5. Jumlah Kewajiban

  

Catatan:

- Tidak perlu rincian detail

- Cukup nominal total potongan

  

### Download Excel

- Download per bulan

- Berdasarkan tahun yang dipilih

- Tampilan Januari — Desember

- Jika belum digenerate manager:

  - tombol belum tersedia

  atau

  - notifikasi “Data belum tersedia”

  

---

  

## CATATAN BESAR DOSEN

  

### Database

- Nominal tidak disimpan 200.000

- Tetapi disimpan menjadi 200

- (3 angka nol terakhir dihilangkan)

  

Tujuan:

- Menghemat memori database

- Efisiensi penyimpanan

  

### Validasi Input

Semua input angka wajib:

- Pemisah ribuan otomatis

- Hanya menerima angka

  

Jika salah input:

- Muncul pesan error merah

  

Berlaku untuk semua form

  

### Target Project

- Sebelum tanggal 18 → semua fitur harus clear

- Setelah itu (tanggal 25–26) → menggunakan data real koperasi

- Tidak lagi menggunakan data dummy