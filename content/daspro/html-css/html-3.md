---
title: 1.3. Tabel pada HTML
date: 2025-05-18
---

# Membuat Tabel pada HTML

Tabel digunakan untuk menampilkan data dalam bentuk baris dan kolom. HTML menyediakan elemen khusus untuk membuat struktur tabel dengan mudah.

## Struktur Dasar Tabel

Berikut struktur umum untuk membuat tabel:

```html
<table>
  <tr>
    <th>Nama</th>
    <th>Umur</th>
    <th>Kota</th>
  </tr>
  <tr>
    <td>Budi</td>
    <td>17</td>
    <td>Jakarta</td>
  </tr>
  <tr>
    <td>Sari</td>
    <td>18</td>
    <td>Bandung</td>
  </tr>
</table>
```

Penjelasan Elemen Tabel

- `<table`>: Elemen utama untuk membuat tabel.

- `<tr>` (table row): Baris dalam tabel.

- `<th>` (table header): Judul kolom. Teks dalam `<th>` biasanya dicetak tebal dan rata tengah.

- `<td>` (table data): Isi dari setiap sel dalam tabel.

## Menambahkan Border dan Styling

Secara default, tabel HTML tidak memiliki border. Kamu bisa menambahkannya lewat atribut border (hanya untuk contoh) atau lebih baik menggunakan [CSS](css-1.md).

Contoh dengan atribut border:

```html
<table border="1">
  <tr>
    <th>Produk</th>
    <th>Harga</th>
  </tr>
  <tr>
    <td>Notebook</td>
    <td>Rp10.000</td>
  </tr>
</table>
```

## Menggabungkan Baris & Kolom:

`rowspan` digunakan untuk menggabungkan baris, sedangkan `colspan` digunakan untuk menggabungkan kolom.

```html
<tr>
  <td rowspan="2">Rudi</td>
  <td>IPA</td>
</tr>
<tr>
  <td>IPS</td>
</tr>
```

## Elemen Tambahan

- `<caption>`: Menambahkan judul tabel.

- `<thead>`, `<tbody>`, `<tfoot>`: Memisahkan bagian atas, isi, dan bawah tabel.

```html
<table>
  <caption>
    Daftar Nilai
  </caption>
  <thead>
    <tr>
      <th>Nama</th>
      <th>Nilai</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Andi</td>
      <td>85</td>
    </tr>
  </tbody>
</table>
```

> [!tip] Materi Berikutnya!
>
> Lanjut ke [Membuat Form](html-4.md)
