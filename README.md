# AlgoritmaDanPemograman-BisDig
TugasUTS


# DasarAlgoritmaDanPemrograman-BisDig

Repository ini berisi dokumentasi dan penjelasan lengkap untuk **5 studi kasus** pemrograman Python pada mata kuliah Dasar Algoritma dan Pemrograman (BisDig).  
Setiap studi kasus terdiri dari:  
1. **Studi Kasus** – deskripsi masalah  
2. **Penjelasan Konsep & Logika** – algoritma, struktur data, dan kontrol yang digunakan  
3. **File Python** – nama file tempat solusi dikodekan  

---

## STUDI KASUS 1: Diskon E-Commerce

### Studi Kasus  
Dalam sistem e-commerce, pelanggan mendapatkan diskon **10%** jika total belanja **> Rp 500.000**.

### Penjelasan Konsep & Logika  
- **Struktur Kontrol Percabangan (`if` / `else`)**  
  - Cek apakah `total_belanja > 500_000`.  
  - Jika benar, hitung `diskon = 0.10 × total_belanja`, else `diskon = 0`.  
- **Operator Aritmatika**  
  - `*` untuk menghitung persentase diskon  
  - `-` untuk mengurangi diskon dari total belanja  

### Algoritma Singkat  
1. Baca input `total_belanja` (tipe `float`)  
2. Jika `total_belanja > 500_000` → `diskon = 0.1 × total_belanja`, cetak “Anda mendapatkan diskon 10%!”  
3. Else → `diskon = 0`, cetak “Maaf, tidak ada diskon.”  
4. Hitung `total_bayar = total_belanja – diskon`  
5. Tampilkan `diskon` dan `total_bayar`  

### File  
`diskon_belanja.py`

---

## 📌 Soal 2: Rata-Rata Nilai & Status Kelulusan

### Studi Kasus  
Seorang siswa ingin mengetahui apakah ia **lulus** berdasarkan rata-rata dari **3 mata pelajaran**.  
Kriteria lulus: **rata-rata ≥ 75**.

### Penjelasan Konsep & Logika  
- **Tipe Data Numerik (`float`)**  
  - Agar hasil rata-rata dapat berupa bilangan desimal  
- **Operator Aritmatika (`+` & `/`)**  
  - `rata_rata = (nilai1 + nilai2 + nilai3) / 3`  
- **Operator Perbandingan (`>=`)**  
  - Menghasilkan boolean untuk struktur `if`  
- **Percabangan (`if` / `else`)**  
  - Jika `rata_rata >= 75` → “LULUS”  
  - Else → “TIDAK LULUS”  

### Algoritma Singkat  
1. Baca tiga input nilai (`float`)  
2. Hitung `rata_rata`  
3. Cek `rata_rata >= 75`  
4. Cetak status kelulusan  

### File  
`cek_kelulusan.py`

---

## 📌 Soal 3: Faktorial dengan Fungsi Rekursif

### Studi Kasus  
Buat **fungsi** untuk menghitung **faktorial** dari suatu bilangan menggunakan **metode rekursif**.

### Penjelasan Konsep & Logika  
- **Fungsi**  
  - Mengemas logika faktorial dalam blok yang bisa dipanggil berulang  
- **Rekursi**  
  - Fungsi memanggil dirinya sendiri hingga mencapai **base case** (`n == 0` atau `n == 1`)  
  - `n! = n × (n−1)!`  

### Algoritma Singkat  
1. Definisikan `faktorial(n)`  
   - Jika `n <= 1`, return `1`  
   - Else return `n * faktorial(n−1)`  
2. Baca input `n` (tipe `int`)  
3. Panggil `faktorial(n)` dan cetak hasil  

### File  
`faktorial_rekursif.py`

---

## 📌 Soal 4: Input Nilai 5 Siswa & Cari Nilai Tertinggi

### Studi Kasus  
Seorang guru ingin program yang menerima **5 nilai siswa**, lalu menampilkan **nilai tertinggi** dan **siswa ke-berapa** yang mendapatkannya.

### Penjelasan Konsep & Logika  
- **List (Array)**  
  - Menyimpan nilai-nilai dalam `list` untuk memudahkan operasi  
- **Perulangan (`for`)**  
  - Loop untuk input nilai sebanyak 5 kali  
- **Fungsi Baku Python**  
  - `max(list)` untuk nilai tertinggi  
  - `list.index(nilai_tertinggi)` untuk posisi (indeks)  

### Algoritma Singkat  
1. Inisialisasi `nilai_siswa = []`  
2. `for i in range(5)`:  
   - Baca `nilai` → `.append()` ke `nilai_siswa`  
3. `nilai_tertinggi = max(nilai_siswa)`  
4. `posisi = nilai_siswa.index(nilai_tertinggi) + 1`  
5. Cetak `nilai_tertinggi` dan `posisi`  

### File  
`nilai_tertinggi.py`

---

## 📌 Soal 5: Hitung Total Harga 3 Barang

### Studi Kasus  
Seorang kasir toko ingin program sederhana untuk menghitung **total harga** pembelian **3 barang** dan menampilkan totalnya.

### Penjelasan Konsep & Logika  
- **Variabel & Input**  
  - Baca tiga harga sebagai `float`  
- **Operator Aritmatika (`+`)**  
  - Menjumlahkan ketiga harga  
- **Output**  
  - Cetak total dengan format rapi  

### Algoritma Singkat  
1. Baca `harga1`, `harga2`, `harga3` (tipe `float`)  
2. Hitung `total = harga1 + harga2 + harga3`  
3. Cetak `total` dengan format dua desimal dan pemisah ribuan  

### File  
`kasir_sederhana.py`

---

## Struktur Folder yang Direkomendasikan

