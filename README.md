# Proyek UTS Pemrograman Web Dasar

* **Nama:** Budi Santoso
* **NIM:** 210101999
* **Tema:** Profil UMKM
* **Objek Usaha:** Money Laundry (Layanan Jasa Laundry Pakaian & Sepatu)

---

## Daftar Fitur Website
1. **Navigasi Multi-Halaman & Responsif:** Memiliki 4 halaman HTML utama (Beranda, Tentang Usaha, Katalog Layanan, Kontak) yang saling terhubung.
2. **Desain Modern & Layout Responsif:** Menggunakan Flexbox untuk navigasi dan CSS Grid untuk tata letak card katalog serta responsivitas tampilan HP ($\le600$ px) dan Desktop ($\ge992$ px).
3. **Menu Hamburger JS:** Toggle navigasi responsif pada perangkat mobile dengan `classList.toggle`.
4. **Validasi Formulir Kontak Double Layer:** Validasi bawaan HTML5 (`required`, `pattern`, `type="email"`, `type="tel"`) + Validasi tambahan JavaScript dengan tampilan error inline di bawah input.
5. **Pencarian & Filter Dinamis Katalog:** Pencarian nama layanan dan filter berdasarkan kategori (Kiloan, Satuan, Sepatu) secara real-time.
6. **Variabel & Interaksi CSS:** Pengunaan 5 variabel CSS root, efek `:hover`, `transition`, dan animasi `@keyframes fadeIn`.

---

## Riwayat Commit Git (Minimal 5 Commit)
1. `commit 1`: `feat: inisialisasi struktur folder proyek dan file HTML dasar`
2. `commit 2`: `feat: menambahkan gaya CSS utama, variabel root, flexbox navigasi, dan CSS grid`
3. `commit 3`: `feat: melengkapi konten halaman tentang kami dan tabel jam operasional pada beranda`
4. `commit 4`: `feat: membuat formulir kontak beserta atribut validasi HTML5`
5. `commit 5`: `feat: menambahkan fitur JavaScript hamburger menu, validasi form inline, dan filter katalog`

---

## Sumber Gambar & Aset
* Gambar Hero & Layanan: Unsplash (sumber bebas lisensi)
* Ikon & Ilustrasi: SVG Standar Browser

---

## Kendala dan Solusi
* **Kendala:** Tampilan kartu katalog berantakan di layar smartphone.
  * **Solusi:** Menambahkan `@media (max-width: 600px)` pada `css/style.css` untuk mengubah kolom CSS Grid menjadi 1 kolom penuh (`grid-template-columns: 1fr`).
* **Kendala:** Menu navigasi menutupi konten hero saat mode mobile dibuka.
  * **Solusi:** Memberikan properti `position: absolute` dengan `top: 60px` dan `z-index` yang sesuai pada menu navigasi.
