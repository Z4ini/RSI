# SILOG-JKT (Sistem Informasi Bantuan dan Distribusi Logistik DKI Jakarta)

Repository Tugas Besar / Praktikum Perancangan Sistem Informasi (DPSI / RSI) - Telkom University.

## 👥 Tim F (Kelas CDK3FAB3)
1. **Ida Sri Rahayu** (103052400069)
2. **Ruqayyah Shofiyyah** (103052400053)
3. **Venanda Angelyca Sherly Melati** (103052400003)
4. **Windi Pramudya Wardani** (103052400006)
5. **Tubagus Muhamad Zaini Arsy** (103052400024)

---

## 📂 Struktur Berkas
* [`silog_jkt.sql`](silog_jkt.sql) : Skrip DDL pembentukan 10 tabel basis data, DML data dummy transaksi (1 Agt - 31 Okt 2026), serta 16 query SQL (SELECT dasar & query analitik GROUP BY/HAVING).
* [`erd_silog_jkt.png`](erd_silog_jkt.png) : Diagram Relasi Entitas (ERD) beresolusi tinggi (300 DPI) mencakup relasi 10 tabel.
* [`erd_silog_jkt.svg`](erd_silog_jkt.svg) : Diagram ERD dalam format vektor SVG.
* [`silog_jkt_viewer.html`](silog_jkt_viewer.html) : Antarmuka interaktif offline untuk melihat skema tabel, isi data transaksi, dan hasil query tugas.
* [`Tugas9_DB_SQL_SILOG-JKT.pdf`](Tugas9_DB_SQL_SILOG-JKT.pdf) : Dokumen panduan tugas 9 perancangan basis data dan SQL.

---

## 🗄️ Rancangan Entitas Basis Data (10 Tabel)
1. `bencana` (Master data bencana alam)
2. `posko` (Posko pengungsian & penanganan bencana)
3. `pengguna` (Akun pengguna petugas BPBD & posko dengan enkripsi SHA-256)
4. `jenis_logistik` (Katalog komoditas logistik)
5. `bantuan_masuk` (Penerimaan donasi logistik dari pihak luar)
6. `stok_gudang` (Persediaan di gudang utama BPBD)
7. `distribusi` (Transaksi pengiriman barang dari gudang ke posko)
8. `kebutuhan_logistik` (Estimasi kebutuhan logistik tiap posko)
9. `stok_posko` (Persediaan barang riil di posko)
10. `log_audit` (Rekam jejak perubahan data status & kuantitas)
