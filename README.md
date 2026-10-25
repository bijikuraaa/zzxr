# Bloomy Florist — katalog bunga

Katalog florist satu halaman dengan HTML, CSS, dan JavaScript biasa. Tidak perlu memasang paket.

## Menjalankan

Buka `index.html` di browser. Bila browser membatasi perilaku saat membuka file lokal, jalankan server statis dari folder ini, misalnya `python -m http.server 8000`, lalu buka `http://localhost:8000`.

## Aset

Semua foto dan ilustrasi situs tersedia secara lokal di `assets/`, termasuk versi maskot yang dipakai halaman dan gambar sumbernya. Tidak ada foto katalog yang diunduh dari URL saat halaman dibuka. Beberapa font dapat dimuat dari Google Fonts saat koneksi internet tersedia.

Untuk mengganti foto, letakkan file baru di `assets/`, lalu ubah jalur `image` dan `gallery` pada `catalog.js` menjadi contoh seperti `assets/nama-foto.jpg`.

## Memperbarui katalog

Semua data produk ada di `catalog.js`. Salin satu objek produk untuk menambah item, lalu ubah:

- `id`: penanda unik, huruf kecil tanpa spasi.
- `name`, `category`, dan `tag`: nama, kategori, dan label produk.
- `price`: harga dalam angka Rupiah tanpa titik atau simbol.
- `subtitle` dan `description`: komposisi dan keterangan produk.
- `image`: jalur foto utama di kartu katalog.
- `gallery`: jalur foto untuk galeri detail.
- `tint`: warna latar foto dalam format hex.

Untuk mengubah harga, ubah `price` pada produk terkait. Kategori baru perlu ditambahkan ke filter di `index.html`.

## Fitur dan catatan

Hero toko bunga bernuansa pink, katalog dengan harga, pencarian dan filter, galeri detail yang dapat digeser, favorit, CTA WhatsApp dengan pesan nama produk otomatis, carousel testimoni yang bergeser setiap 4 detik dan berhenti saat diarahkan kursor (dengan tombol navigasi manual), serta maskot kucing yang bergerak dari hero ke produk yang disorot. Animasi menghormati pengaturan reduced motion.

Foto produk dan harga saat ini adalah contoh prototipe dan perlu diganti/diverifikasi dengan katalog Bloomy yang sebenarnya sebelum dipublikasikan. Nomor WhatsApp dan Instagram mengikuti informasi yang diberikan.

Bagian testimoni berisi teks dan nama contoh untuk memperlihatkan desain. Ganti semuanya dengan ulasan pelanggan asli sebelum situs dipublikasikan.

Foto hero: “Vibrant floral arrangements displayed in a shop” oleh Esra Afşar, digunakan dari Unsplash di bawah Unsplash License. Sumber: https://unsplash.com/photos/vibrant-floral-arrangements-displayed-in-a-shop-V3TtgXboqCc

Untuk mengganti contoh testimoni, edit daftar `testimonials` di `app.js`. Setiap ulasan memiliki `name`, `initials`, `date` (format `YYYY-MM-DD`), `rating` (1–5), dan `text`. Tanggal ditampilkan otomatis sebagai waktu relatif seperti “2 minggu lalu”.
