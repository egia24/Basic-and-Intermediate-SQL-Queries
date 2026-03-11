# Basic and Intermediate SQL Queries

Latihan ini berfokus pada **querying data** menggunakan SQL untuk analisis bisnis, meliputi filtering, aggregasi, join, dan conditional statement.

---

## Table Schema
- Student diminta melakukan **insert manual** menggunakan tools Import Data di DBeaver.  
- Pastikan **tipe data sesuai dengan list table schema** saat memasukkan data ke database.

---

## Latihan Query

### 1. Produk mengandung “Sport”
Tampilkan **10 produk** dengan nama produk mengandung kata *Sport*, urutkan berdasarkan `product_id`.

**Ekspektasi output:**  
- 10 baris produk yang mengandung kata "Sport".  
- Kolom: `product_id`, `product_name`, `category`, dll.

---

### 2. 10 Produk Paling Mahal & 10 Paling Murah
Tampilkan **10 produk termahal** dan **10 termurah**.

**Ekspektasi output:**  
- Kolom: `product_id`, `product_name`, `price`.  
- Terurut dari harga tertinggi/rendah.

---

### 3. Total Jumlah Barang per Kategori di Asia
Hitung total jumlah barang terjual per kategori untuk negara di **benua Asia**.  
**Hints:** Filter `status = 'Complete'`.

**Ekspektasi output:**  
- Kolom: `category`, `total_quantity`.

---

### 4. Customer Berdasarkan Range Umur
Hitung jumlah customer berdasarkan range umur:  
- 0 – 18 → Remaja  
- 19 – 55 → Dewasa  
- > 56 → Lanjut Usia  
**Hints:** Gunakan conditional statement (`CASE WHEN`).

**Ekspektasi output:**  
- Kolom: `age_group`, `customer_count`.

---

### 5. Bulan 2024 dengan Total Sale Price > 1000
Tampilkan daftar **bulan di tahun 2024** dengan total `sale_price` > 1000.  
**Hints:** Gabungkan nama menjadi `full_name`, abaikan status pemesanan.

**Ekspektasi output:**  
- Kolom: `month`, `total_sale_price`.

---

### 6. 10 Hari dengan Pemesanan 'Complete' Terbanyak
Tampilkan **10 tanggal** dengan jumlah pemesanan `status = 'Complete'` terbanyak.  
**Hints:** Ambil tanggal dari `created_at`.

**Ekspektasi output:**  
- Kolom: `date`, `total_orders`.

---

## Reflection Questions
1. Bagian mana dari query (filtering, aggregation, join) yang paling menunjukkan bahwa SQL **tidak hanya mengambil data**, tetapi **membantu menjawab kebutuhan bisnis**?  
2. Saat melakukan **JOIN** antar tabel, apa yang dipelajari tentang hubungan antar data dalam database relasional?  
3. Apa risiko yang muncul jika struktur tabel dan relasi tidak dipahami, misalnya hasil analisis yang **salah atau misleading**?  
