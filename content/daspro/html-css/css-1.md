---
title: 2.1. Mengenal Styling Tampilan Website (CSS)
date: 2025-05-18
---

# Mengenal CSS

CSS (Cascading Style Sheets) adalah bahasa yang digunakan untuk mengatur tampilan dan gaya elemen dalam dokumen HTML. Dengan CSS, kamu bisa mengatur warna, ukuran, posisi, spasi, dan desain visual lainnya pada halaman web.

## Mengapa CSS Penting?

Tanpa CSS, semua halaman HTML hanya akan terlihat polos dan tidak menarik. CSS memungkinkan kamu untuk:

- Mendesain tampilan website sesuai keinginan

- Membuat layout yang responsif (mobile friendly)

- Memisahkan struktur (HTML) dan tampilan (CSS)

- Menghemat waktu dengan menerapkan gaya yang sama ke banyak elemen

## Cara Menyisipkan CSS

Ada 3 cara menyisipkan CSS ke dalam HTML:

1. Inline CSS

Langsung ditulis di dalam elemen HTML menggunakan atribut style.

```html
<p style="color: red;">Ini teks berwarna merah</p>
```

2. Internal CSS

Ditulis di dalam tag `<style>` pada bagian `<head>` HTML.

```html
<head>
  <style>
    p {
      color: blue;
    }
  </style>
</head>
```

3. External CSS

CSS ditulis di file terpisah dengan ekstensi `.css`, lalu dipanggil menggunakan tag `<link>`.

```html
<!-- Di file HTML -->
<head>
  <link rel="stylesheet" href="style.css" />
</head>
```

```css
/* Di file style.css */
p {
  color: green;
}
```

## Selektor CSS

Selektor digunakan untuk memilih elemen HTML yang ingin diberi gaya.

- Selektor Tag HTML: memilih elemen berdasarkan tag / elemet HTMLnya.
- Selektor ID: memilih elemen berdasarkan atribut ID.
- Selektor Kelas: memilih elemen berdasarkan atribut Kelas.

Contoh Selektor:

```css
/* Selektor tag */
h1 {
  color: darkblue;
}

/* Selektor class */
.kotak {
  width: 100px;
  height: 100px;
  background: orange;
}

/* Selektor ID */
#judul {
  font-size: 24px;
  text-align: center;
}
```

## Properti Umum CSS

Berikut beberapa properti umum yang sering digunakan dalam CSS, kedepnnya akan kita bahas lebih banyak:

| Properti     | Fungsi                              | Value                            |
| ------------ | ----------------------------------- | -------------------------------- |
| color        | Mengatur warna teks                 | RGB, HEX, nama warna             |
| background   | Mengatur warna/ gambar latar        | RGB, HEX, nama warna, URL gambar |
| font-size    | Mengatur ukuran teks                | px, em, rem, %                   |
| padding      | Jarak dalam dari isi ke tepi elemen | px, em, rem, %                   |
| margin       | Jarak luar antar elemen             | px, em, rem, %                   |
| border       | Mengatur garis tepi elemen          | px, em, rem, %                   |
| width/height | Mengatur lebar dan tinggi elemen    | px, em, rem, %                   |

> [!tip] Materi CSS Berikutnya!
>
> Lanjutke [Typography dan Text Formatting](css-2.md)
