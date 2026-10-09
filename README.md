# Enterprise POS (Point of Sale) Multi-Cabang & Multi-Role

Sistem aplikasi Point of Sale (POS) modern berbasis web yang dirancang untuk mendukung operasional bisnis multi-cabang (multi-store), dilengkapi dengan manajemen inventori lengkap, laporan keuangan otomatis dengan visualisasi grafik (chart), dan sistem otorisasi multi-role (RBAC).

---

## 🚀 Fitur Utama

### 1. Multi-Cabang (Multi-Branch Management)
- Pengelolaan cabang terpusat untuk Owner / Super Admin.
- Isolasi data transaksi, kas, dan stok per cabang dengan opsi konsolidasi global.
- Pemilihan cabang aktif untuk manajer dan staf operasional.

### 2. Multi-Role & Hak Akses (RBAC)
- **Super Admin (Owner)**: Akses global ke semua cabang, kelola master data, laporan konsolidasi.
- **Branch Manager**: Manajemen operasional cabang, persetujuan transfer stok, monitor kasir.
- **Kasir (Cashier)**: Transaksi penjualan, input barcode, terima pembayaran, buka/tutup shift kas.
- **Staf Gudang (Inventory)**: Stok masuk/keluar, penerimaan supplier, transfer stok antar cabang, opname stok.
- **Akuntan / Finance**: Akses laporan keuangan, analisis laba rugi, pencatatan pengeluaran.

### 3. Modul Kasir (POS Terminal)
- Antarmuka kasir cepat & responsif (Desktop & Tablet).
- Integrasi Barcode Scanner & pencarian cepat produk.
- Keranjang belanja dinamis, diskon bertingkat, dan pajak (PPN).
- Berbagai metode pembayaran (Tunai, QRIS, Kartu Debit/Kredit, Transfer, Split Payment).
- Manajemen Shift Kasir (Buka modal awal kasir & rekap tutup kas).
- Cetak struk belanja thermal (format 58mm & 80mm).

### 4. Manajemen Inventori & Pergudangan
- Stok real-time per cabang dengan riwayat kartu stok digital.
- Alur transfer stok antar-cabang dengan status verifikasi (Pending -> Shipped -> Received).
- Modul Stock Opname (Audit fisik vs data sistem dengan perhitungan selisih).
- Notifikasi stok menipis (*low-stock alert*).
- Manajemen data Supplier & Purchase Order.

### 5. Laporan Keuangan & Visualisasi Chart
- Dashboard analitik eksekutif (Omzet, Total Transaksi, Laba Bersih, Rata-rata Nilai Keranjang).
- Grafik interaktif:
  - Tren penjualan harian, mingguan, dan bulanan.
  - Komparasi performa antar-cabang.
  - Donut chart kategori & produk terlaris.
  - Distribusi jam sibuk transaksi (*peak hours*).
- Laporan Laba Rugi komprehensif (Penjualan Bersih - HPP - Biaya Operasional = Laba Bersih).
- Ekspor laporan ke format Excel/CSV dan PDF siap cetak.

---

## 👥 Tim Multi-Agent Terdaftar

Proyek ini dikembangkan bersama 5 subagent spesialis:
1. **`pos-architect`**: Arsitektur sistem, skema database multi-cabang, API contracts, dan standarisasi struktur kode.
2. **`pos-auth-rbac`**: Autentikasi, perizinan role granular, security guard, dan audit trail.
3. **`pos-cashier-core`**: UI terminal kasir, transaksi cepat, pembayaran, dan pencetakan struk.
4. **`pos-inventory`**: Pergudangan multi-cabang, mutasi stok, transfer barang, dan stock opname.
5. **`pos-finance-analytics`**: Pembukuan keuangan, kalkulasi P&L/HPP, dan dashboard grafik interaktif.