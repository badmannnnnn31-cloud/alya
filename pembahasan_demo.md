# Panduan Demo Lisan UTS Pemrograman Web Dasar (5 Menit)

## Alur Pembicaraan (Skrip Demo)

### 1. Pembukaan & Pengenalan Usaha (1 Menit)
"Selamat pagi/siang Pak Ditra. Nama saya Budi Santoso, NIM 210101999. Pada UTS Pemrograman Web Dasar ini, saya memilih **Tema A: Profil UMKM** dengan objek usaha **Money Laundry**, yaitu jasa layanan laundry kiloan, satuan, dan perawatan sepatu profesional."

### 2. Demonstrasi Halaman & Fitur HTML/CSS (2 Menit)
* **Beranda (`index.html`):** "Di halaman utama terdapat *hero section* dengan animasi `@keyframes fadeIn`, ringkasan usaha, 3 kartu unggulan, dan tabel jam operasional yang dibuat menggunakan tag semantik `<table>`, `<thead>`, dan `<tbody>`."
* **Tentang Usaha (`tentang.html`):** "Halaman ini memuat sejarah, visi/misi, serta 3 tim pengurus yang ditata menggunakan layout CSS Grid."
* **Katalog Layanan (`katalog.html`):** "Katalog menyajikan 6 kartu layanan yang disusun dengan CSS Grid. Di tampilan HP, layout ini otomatis berubah menjadi 1 kolom responsif melalui `@media (max-width: 600px)`."
* **Kontak (`kontak.html`):** "Halaman kontak dilengkapi embed Google Maps dan formulir validasi HTML5 (`required`, `type="email"`, `pattern="[0-9]{10,13}"`)."

### 3. Demonstrasi Fitur Bonus JavaScript (1 Menit)
* **Hamburger Menu:** "Pada layar kecil, menu navigasi disembunyikan dan diakses via tombol hamburger yang menggunakan `classList.toggle('active')`."
* **Filter Katalog Dinamis:** "Fitur ini mendengarkan event `input` dan `change` untuk menyaring kartu katalog berdasarkan teks pencarian dan kategori tanpa me-reload halaman."
* **Validasi Form JS:** "Mencegah pengiriman form default dengan `e.preventDefault()`, lalu menampilkan pesan error langsung di bawah masing-masing elemen `<input>`."

### 4. Penutup (1 Menit)
"Seluruh kode CSS telah disatukan di file eksternal `css/style.css` menggunakan 5 variabel root, dan kode lolos validasi W3C tanpa error. Terima kasih."

---

## Jawaban Pertanyaan Kemungkinan dari Dosen

1. **Mengapa menggunakan elemen semantik seperti `<header>`, `<nav>`, `<main>`, `<footer>`?**
   * *Jawaban:* Agar struktur dokumen HTML lebih rapi, mudah dibaca oleh mesin pencari (SEO), dan mendukung keterbacaan perangkat pembaca layar (*screen reader*), tidak hanya menggunakan `<div>` semata.

2. **Bagaimana cara kerja responsivitas di CSS?**
   * *Jawaban:* Saya menggunakan *media query* `@media (max-width: 600px)` untuk tampilan HP, di mana `grid-template-columns` diubah dari 3 kolom menjadi `1fr` (1 kolom), serta menyembunyikan navigasi menjadi menu hamburger.

3. **Bagaimana fungsi `classList.toggle('active')` pada JavaScript?**
   * *Jawaban:* Fungsi tersebut mengecek apakah kelas `active` sudah ada pada elemen navigasi. Jika belum ada, kelas akan ditambahkan (membuka menu); jika sudah ada, kelas akan dihapus (menutup menu).
