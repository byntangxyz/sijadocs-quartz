---
title: 2.3. Basic Properti CSS
date: 2025-05-18
---

# Basic Properti CSS

Setelah memahami properti CSS yang berhubungan dengan [teks dan font](css-2.md), kini saatnya mempelajari properti dasar CSS lainnya yang sering digunakan untuk mengatur layout, spasi, ukuran, warna, dan border dari elemen HTML. Properti-properti ini merupakan fondasi penting dalam membuat tampilan web yang rapi dan enak dilihat.

1. `width dan height`

Digunakan untuk menentukan lebar dan tinggi dari elemen.

```css
.box {
  width: 200px;
  height: 100px;
}
```

Satuan yang umum digunakan: `px`, `%`, `em`, `rem`, `vw`, `vh`

`%` tergantung dari element paret (diatasnya).

2. `background`

Digunakan untuk memberi latar belakang pada elemen. Lihat preferensi properti di [W3School](https://www.w3schools.com/cssref/css3_pr_background.php)

```css
.container {
  background-color: #f0f0f0;
  background-image: url("bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
```

> [!info] Shorthand (digabung jadi 1 baris):
>
> ```css
> background: #f0f0f0 url("bg.jpg") no-repeat center / cover;
> ```

3. `margin` dan `padding`

margin: jarak luar antar elemen
padding: jarak dalam antara isi dan batas elemen

![Box Model](https://miro.medium.com/v2/resize:fit:1400/1*3STqKwTGNXBoZgbXbp3aDA.png)
_Source: Medium_

Mempunyai satuan yang sama dengan `width` dan `height` (px, %, em, rem, vw, vh)

```css
.card {
  margin: 20px;
  padding: 15px;
}
```

Kamu bisa mengatur masing-masing sisi:

```css
margin-top: 10px;
margin-right: 15px;
margin-bottom: 20px;
margin-left: 25px;
```

> [!info] Shorthand (digabung jadi 1 baris):
>
> ```css
> padding: 10px 15px 20px 25px; /* top right bottom left */
> ```

4. `border`
   Untuk memberi garis tepi (border) pada elemen. Mempunyai satuan yang sama dengan `margin` dan `padding` (px, %, em, rem, vw, vh)

```css
.box {
  border: 2px solid #333;
}
```

Properti lain:

- border-style: solid, dashed, dotted, double, dll

- border-color

> [!info] Shorthand (digabung jadi 1 baris):
>
> ```css
> border: 1px dashed red;
> ```

5. `box-sizing`
   Menentukan apakah padding dan border dihitung dalam ukuran elemen (width/height).

```css
* {
  box-sizing: border-box;
}
```

Nilai:

- content-box (default): padding dan border tidak termasuk width

- border-box: padding dan border termasuk dalam width

![Box Sizing](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*rJalI52XK72c32eFsyI1xg.png)
_Source Medium: @nico.jcbp_

6. `display`
   Mengatur bagaimana elemen ditampilkan.

```css
div {
  display: block;
}
```

Nilai umum:

- `block`: elemen memiliki lebar penuh (100%)

- `inline` : elemen memiliki lebar sesuai dengan kontennya

- `inline-block` : elemen memiliki lebar sesuai dengan kontennya

- `flex` : elemen dapat diatur sebagai flex container atau item. Akan kita pelajari di [Flexbox](css-4.md)

- `grid` : elemen dapat diatur sebagai grid container atau item.

- `none` : elemen tidak ditampilkan.s

7. `position`
   Mengatur posisi elemen secara manual. Lihat dokumentasi lengkap nya di [W3School](https://www.w3schools.com/css/css_positioning.asp)

```css
.absolute-box {
  position: absolute;
  top: 20px;
  left: 50px;
}
```

Nilai:

- `static` (default): posisi elemen ditentukan oleh dokumen

- `relative` : posisi elemen ditentukan oleh dokumen, tetapi elemen dapat diatur secara manual

- `absolute` : posisi elemen ditentukan secara manual, elemen tidak akan berinteraksi dengan elemen lainnya

- `fixed` : posisi elemen ditentukan secara manual, elemen tidak akan berinteraksi dengan elemen lainnya dan tidak akan berubah ketika pengguna menggeser halaman

- `sticky` : posisi elemen ditentukan secara manual, tetapi elemen akan berinteraksi dengan elemen lainnya ketika pengguna menggeser halaman

Biasanya digunakan bersama properti `top`, `right`, `bottom`, `left`.

8. `z-index`
   Menentukan tumpukan elemen (mana yang di atas atau di bawah).

```css
.box {
  position: relative;
  z-index: 10;
}
```

Semakin besar nilai z-index, maka elemen akan tampil di atas elemen lain yang z-index-nya lebih rendah.

9. `overflow`
   Mengatur bagaimana konten yang melebihi ukuran elemen ditampilkan.

```css
.box {
  width: 200px;
  height: 100px;
  overflow: auto;
}
```

Nilai:

- `visible` (default): konten akan ditampilkan secara normal

- `hidden` : konten yang melebihi ukuran elemen akan disembunyikan

- `scroll` : konten yang melebihi ukuran elemen akan ditampilkan dengan scroll

- `auto` : konten yang melebihi ukuran elemen akan ditampilkan dengan scroll jika elemen memiliki ukuran yang lebih besar dari konten, atau disembunyikan jika elemen memiliki ukuran yang lebih kecil dari konten

10. `cursor`
    Mengubah tampilan kursor saat diarahkan ke elemen. Lihat contoh lengkap di[W3School](https://www.w3schools.com/css/tryit.asp?filename=trycss_cursor)

```css
button {
  cursor: pointer;
}
```

Nilai umum: `pointer`, `default`, `text`, `move`, `not-allowed`, `grab`, dll.

11. `opacity`
    Mengatur tingkat transparansi elemen.

```css
.box {
  opacity: 0.5; /* 0 = transparan, 1 = tidak transparan */
}
```

12. `transition`
    Memberikan efek transisi saat nilai properti berubah.

```css
.box {
  transition: all 0.3s ease;
}
```

> [!tip] Materi CSS Berikutnya!
>
> Lanjutke [CSS Flexbox](css-4.md)
