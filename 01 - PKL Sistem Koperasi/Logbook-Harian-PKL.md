# Skema Pengerjaan Role Manager (1 - 15 Maret 2026)

Rencana ini disusun untuk keperluan laporan PKL dengan pembagian tugas Backend dan Frontend. Jadwal dibuat secara logis dengan beberapa fitur kompleks (Excel & PDF) yang masih dalam status *In Progress* sesuai kondisi riil pengembangan.

## Ringkasan Proyek

- **Target:** Implementasi Role Manager dan Fitur Laporan.

- **Periode:** 1 Maret 2026 - 31 Maret 2026.

- **Status Saat Ini:** Pengembangan modul inti selesai, fitur ekspor (Excel/PDF) sedang dikerjakan.

## Jadwal Pengerjaan Backend (Logbook)

|     Tanggal     | Aktivitas Pengerjaan                          | Status           | Detail Kendala/Catatan                                 |
| :-------------: | --------------------------------------------- | ---------------- | ------------------------------------------------------ |
| **1 Mar 2026**  | Analisis struktur DB & Migrasi role `manager` | ✅ Selesai        | Menyiapkan field `role` baru pada tabel `users`.       |
| **2 Mar 2026**  | Research library `PHPSpreadsheet` & `DomPDF`  | ✅ Selesai        | Cek kompatibilitas library dengan versi PHP.           |
| **3 Mar 2026**  | Pengembangan Logic Aggregator Dashboard (P1)  | ✅ Selesai        | Query dasar untuk total simpanan & pinjaman.           |
| **4 Mar 2026**  | Pengembangan Logic Aggregator Dashboard (P2)  | ✅ Selesai        | Penambahan kalkulasi saldo kas harian & bulanan.       |
| **5 Mar 2026**  | Implementasi Middleware Auth Role Manager     | ✅ Selesai        | Proteksi route agar hanya bisa diakses role tertentu.  |
| **6 Mar 2026**  | Integrasi Manager Logic ke `AuthController`   | ✅ Selesai        | Redirect otomatis setelah login berdasarkan role.      |
| **7 Mar 2026**  | Update `LaporanController` (Access Mapping)   | ✅ Selesai        | Penyesuaian hak akses untuk menu laporan utama.        |
| **8 Mar 2026**  | _Libur / Istirahat Mingguan_                  | -                | -                                                      |
| **9 Mar 2026**  | Perancangan Query SQL Laporan Bulanan (Join)  | ✅ Selesai        | Menggabungkan data dari 4 tabel transaksi utama.       |
| **10 Mar 2026** | Implementasi API Endpoint Laporan Bulanan     | ✅ Selesai        | Pembuatan struktur data JSON yang efisien.             |
| **11 Mar 2026** | Validasi Data & Penanganan Null Values        | ✅ Selesai        | Memastikan laporan tetap tampil meski data kosong.     |
| **12 Mar 2026** | Refactoring & Optimasi Query Laporan          | ✅ Selesai        | Mengurangi beban server saat load data ribuan baris.   |
| **13 Mar 2026** | Integrasi Awal Export Excel (Template Dasar)  | ✅ Selesai        | Berhasil generate file .xlsx namun format masih polos. |
| **14 Mar 2026** | Logic Formatting Excel (Auto-size & Styling)  | 🚧 _In Progress_ | Kendala pada pengaturan lebar kolom otomatis.          |
| **15 Mar 2026** | Pengembangan Core Logic Generate PDF          | 🚧 _In Progress_ | Masalah pada library DomPDF saat merender CSS tabel.   |
| **16 Mar 2026** |                                               |                  |                                                        |
| **17 Mar 2026** |                                               |                  |                                                        |
| **18 Mar 2026** |                                               |                  |                                                        |
| **19 Mar 2026** |                                               |                  |                                                        |
| **20 Mar 2026** |                                               |                  |                                                        |
| **21 Mar 2026** |                                               |                  |                                                        |
| **22 Mar 2026** | _Libur / Istirahat Mingguan_                  | -                | -                                                      |
| **23 Mar 2026** |                                               |                  |                                                        |
| **24 Mar 2026** |                                               |                  |                                                        |
| **25 Mar 2026** |                                               |                  |                                                        |
| **26 Mar 2026** |                                               |                  |                                                        |
| **27 Mar 2026** |                                               |                  |                                                        |
| **28 Mar 2026** |                                               |                  |                                                        |
| **29 Mar 2026** | _Libur / Istirahat Mingguan_                  | -                | -                                                      |
| **30 Mar 2026** |                                               |                  |                                                        |
| **31 Mar 2026** |                                               |                  |                                                        |

## Jadwal Pengerjaan Frontend (Logbook)

|     Tanggal     | Aktivitas Pengerjaan                         | Status           | Detail Kendala/Catatan                                    |
|:---------------:| -------------------------------------------- | ---------------- | --------------------------------------------------------- |
| **1 Mar 2026**  | Inisialisasi komponen UI & Asset Manager     | ✅ Selesai       | Persiapan icon dan tema warna khusus dashboard.           |
| **2 Mar 2026**  | Slicing Layout Dashboard (Header & Summary)  | ✅ Selesai       | Implementasi grid sistem untuk ringkasan data.            |
| **3 Mar 2026**  | Integrasi Chart.js (Grafik Simpanan)         | ✅ Selesai       | Visualisasi tren simpanan anggota per bulan.              |
| **4 Mar 2026**  | Integrasi Chart.js (Grafik Pinjaman)         | ✅ Selesai       | Visualisasi perbandingan pinjaman lancar vs macet.        |
| **5 Mar 2026**  | Update Navigasi Sidebar Dinamis              | ✅ Selesai       | Menu "Manager Area" hanya tampil untuk role manager.      |
| **6 Mar 2026**  | Pembuatan Template View Laporan Bulanan      | ✅ Selesai       | Desain tabel laporan yang clean dan informatif.           |
| **7 Mar 2026**  | Implementasi Komponen Filter (Date Range)    | ✅ Selesai       | Menggunakan library DatePicker untuk kemudahan user.      |
| **8 Mar 2026**  | _Libur / Istirahat Mingguan_                 | -                | -                                                         |
| **9 Mar 2026**  | Integrasi Frontend-Backend Laporan (AJAX)    | ✅ Selesai       | Load data laporan tanpa refresh halaman (SPA style).      |
| **10 Mar 2026** | Styling Table Laporan (Sticky Header)        | ✅ Selesai       | Memudahkan user melihat header saat scroll data panjang.  |
| **11 Mar 2026** | Implementasi Loading States & Skeletons      | ✅ Selesai       | UX lebih baik saat data sedang ditarik dari server.       |
| **12 Mar 2026** | Penanganan Error & Notifikasi (Toast)        | ✅ Selesai       | Pesan error jika filter tanggal tidak valid.              |
| **13 Mar 2026** | Penambahan UI Action (Tombol Export & Cetak) | ✅ Selesai       | Desain tombol yang konsisten dengan tema aplikasi.        |
| **14 Mar 2026** | Styling PDF Template (CSS Media Print)       | 🚧 _In Progress_ | Penyesuaian font agar tidak terlalu kecil saat diprint.   |
| **15 Mar 2026** | Implementasi Modal Preview PDF               | 🚧 _In Progress_ | Menampilkan tampilan PDF di dalam modal sebelum download. |
| **16 Mar 2026** |                                              |                  |                                                           |
| **17 Mar 2026** |                                              |                  |                                                           |
| **18 Mar 2026** |                                              |                  |                                                           |
| **19 Mar 2026** |                                              |                  |                                                           |
| **20 Mar 2026** |                                              |                  |                                                           |
| **21 Mar 2026** |                                              |                  |                                                           |
| **22 Mar 2026** | _Libur / Istirahat Mingguan_                 | -                | -                                                         |
| **23 Mar 2026** |                                              |                  |                                                           |
| **24 Mar 2026** |                                              |                  |                                                           |
| **25 Mar 2026** |                                              |                  |                                                           |
| **26 Mar 2026** |                                              |                  |                                                           |
| **27 Mar 2026** |                                              |                  |                                                           |
| **28 Mar 2026** |                                              |                  |                                                           |
| **29 Mar 2026** | _Libur / Istirahat Mingguan_                 | -                | -                                                         |
| **30 Mar 2026** |                                              |                  |                                                           |
| **31 Mar 2026** |                                              |                  |                                                           |

## Pembagian Tugas Teknis

  

## Pembagian Tugas Teknis

  

### [Backend]

- **Auth System:** Penambahan konstanta `ROLE_MANAGER` dan pengecekan session di `Auth.php`.

- **Controller Logic:** Penambahan method `index()` di `ManagerController` dan penyesuaian di `LaporanController`.

- **Export Engine:** Integrasi library untuk konversi HTML ke PDF dan Array ke Excel (Masih tahap debugging).

  

### [Frontend]

- **Dashboard UI:** Penggunaan Chart.js untuk visualisasi data bagi Manager.

- **Navigation:** Update sidebar menu untuk menampilkan menu "Manager Area".

- **Print Styles:** Pembuatan template khusus `.html` yang akan di-convert menjadi PDF.

  

---

  

## Verifikasi & Progress

- [x] Login sebagai Manager berhasil.

- [x] Dashboard menampilkan ringkasan data koperasi.

- [x] Filter laporan bulanan berfungsi.

- [/] **Generate Excel:** Data masuk tapi format berantakan.

- [/] **Generate PDF:** Masih *blank page* pada laporan yang datanya ribuan.