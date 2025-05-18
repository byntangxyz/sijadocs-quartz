---
title: 1.1. HTML Fundamental
date: 2025-05-18
---

# Dasar-dasar HTML

## Apa itu HTML?

HTML adalah bahasa markah (markup language), bukan bahasa pemrograman. HTML digunakan untuk menandai (mark up) bagian-bagian konten agar bisa ditampilkan secara terstruktur oleh browser.

## Struktur Dasar HTML

Setiap halaman HTML memiliki struktur umum yang terdiri dari beberapa bagian utama:

```html
<!DOCTYPE html>
<html lang="id">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Judul Halaman</title>
  </head>
  <body>
    <h1>Selamat datang!</h1>
    <p>Ini adalah halaman HTML pertamaku.</p>
  </body>
</html>
```

Penjelasan Struktur:

`<!DOCTYPE html>`: Menandai bahwa dokumen ini menggunakan standar HTML5.

`<html>`: Elemen root (paling luar) dari dokumen HTML.

`<head>`: Bagian ini berisi informasi tentang dokumen (metadata), seperti judul halaman, pengaturan karakter, dan link ke CSS atau script.

`<body>`: Berisi semua konten yang akan ditampilkan di browser, seperti teks, gambar, link, dll.

## Elemen-Elemen Umum HTML:

1. Judul (Heading)
   Digunakan untuk membuat judul dengan tingkat penting berbeda, dari `<h1>` sampai `<h6>`.

```html
<h1>Judul Utama</h1>
<h2>Subjudul</h2>
```

2. Paragraf
   Untuk membuat teks paragraf biasa:

```html
<p>Ini adalah sebuah paragraf teks.</p>
```

3. Link
   Untuk membuat tautan ke halaman lain atau URL tertentu:

```html
<a href="https://sijaarc.my.id">Kunjungi Website Sija A</a>
```

4. Gambar
   Menampilkan gambar dari URL atau file lokal:

```html
<img src="gambar.jpg" alt="Deskripsi Gambar" />
```

5. List (Daftar)
   Daftar Tak Terurut:

```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
</ul>
```

Daftar Terurut:

```html
<ol>
  <li>Item pertama</li>
  <li>Item kedua</li>
</ol>
```

## Atribut pada Tag HTML

Atribut memberikan informasi tambahan pada tag HTML. Contoh atribut umum:

```html
<a href="https://lms.stembayo.top" target="_blank">Buka di tab baru</a>
<img src="logo.png" width="200" height="100" />
```

## Komentar di HTML

Komentar tidak akan ditampilkan atau dieksekusi di browser:

```html
<!-- Ini adalah komentar 
 <p>Paragraf ini tidak terlihat</>
 -->
<p>Paragraf ini terlihat</p>
```

> [!tip] Materi Berikutnya!
>
> Lanjutke [Membuat Video dan Audio di HTML](html-2.md)
