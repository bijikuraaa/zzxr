# Bloomy Florist — katalog bunga

Storefront florist satu halaman dengan HTML, CSS, dan JavaScript biasa. Tidak perlu memasang paket.

## Menjalankan

Buka `index.html` di browser. Bila browser membatasi perilaku saat membuka file lokal, jalankan server statis dari folder ini, misalnya `python -m http.server 8000`, lalu buka `http://localhost:8000`.

## Folder gambar

Semua gambar situs disimpan di `assets/` dan dipanggil menggunakan jalur relatif, jadi halaman tidak perlu mengunduh foto dari tautan gambar saat dibuka. Folder ini berisi foto hero, cerita, foto buket, ilustrasi maskot, dan foto referensi kucing.

Untuk mengganti foto produk, letakkan file baru di `assets/`, lalu ubah `image` dan `gallery` pada `catalog.js` menjadi jalur seperti `assets/nama-foto.jpg`.

## Memperbarui katalog

Semua data produk ada di `catalog.js`, terpisah dari tampilan. Untuk menambah produk, salin satu objek produk yang ada dan ubah nilai berikut:

- `id`: penanda unik, huruf kecil tanpa spasi.
- `name`, `category`, dan `tag`: nama, kategori, dan label produk.
- `price`: harga dalam angka Rupiah tanpa titik atau simbol.
- `subtitle` dan `description`: komposisi singkat dan keterangan detail.
- `image`: jalur foto utama pada kartu katalog.
- `gallery`: daftar jalur foto detail; urutan pertama menjadi foto utama.
- `tint`: warna latar foto dalam format hex.

Kategori baru perlu ditambahkan sebagai tombol filter di `index.html`. Untuk perubahan harga saja, ubah `price` di objek produk terkait.

## Fitur

Hero, koleksi contoh dengan galeri foto, pencarian, filter kategori, detail produk, favorit, dan maskot kucing yang bergerak ke kartu aktif. Halaman ini fokus sebagai katalog dan daftar harga; tidak ada keranjang atau checkout.

Harga dan produk hanya contoh untuk prototipe. Foto buket dan florist berasal dari Unsplash dan disimpan lokal di `assets/`.
