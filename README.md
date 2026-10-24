# Bloomy Florist — katalog bunga

Storefront florist satu halaman dengan HTML, CSS, dan JavaScript biasa. Tidak perlu memasang paket.

## Menjalankan

Buka `index.html` di browser. Bila browser membatasi perilaku saat membuka file lokal, jalankan server statis dari folder ini, misalnya `python -m http.server 8000`, lalu buka `http://localhost:8000`.

Foto hero dan produk memakai Unsplash dan memerlukan koneksi internet. Maskot memakai ilustrasi SVG lokal yang bergerak mengikuti kartu aktif.

## Memperbarui katalog

Semua data produk ada di `catalog.js`, terpisah dari tampilan. Untuk menambah produk, salin satu objek produk yang ada dan ubah nilai berikut:

- `id`: penanda unik, huruf kecil tanpa spasi.
- `name`, `category`, dan `tag`: nama, kategori, dan label produk.
- `price`: harga dalam angka Rupiah tanpa titik atau simbol.
- `subtitle` dan `description`: komposisi singkat dan keterangan detail.
- `image`: URL foto utama yang tampil di kartu katalog.
- `gallery`: daftar lima foto untuk galeri detail; urutan pertama menjadi foto utama.
- `tint`: warna latar foto dalam format hex.

Kategori baru perlu ditambahkan sebagai tombol filter di `index.html`. Untuk perubahan harga saja, ubah `price` di objek produk terkait.

## Fitur

Hero, koleksi delapan buket contoh, masing-masing dengan lima foto galeri, pencarian, filter kategori, detail produk, favorit, dan maskot kucing yang bergerak ke kartu aktif. Halaman ini fokus sebagai katalog dan daftar harga; tidak ada keranjang atau checkout.

Harga dan produk hanya contoh untuk prototipe.


Foto hero menggunakan foto interior florist oleh Esra Afşar di Unsplash: https://unsplash.com/photos/a-flower-shop-counter-with-bouquets-and-dried-arrangements-2D1GrH_Dwkk.com/photos/a-flower-shop-with-a-bunch-of-flowers-in-front-of-it-ReL2LOAdyHU.com/photos/a-flower-shop-counter-with-bouquets-and-dried-arrangements-2D1GrH_Dwkk.
