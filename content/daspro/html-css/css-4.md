---
title: 2.4. CSS Flexbox
date: 2025-05-18
---

# CSS Flexbox

Flexbox (Flexible Box Layout) adalah metode layout satu dimensi di CSS yang memudahkan kita dalam menyusun elemen secara fleksibel, baik secara horizontal maupun vertikal.

Dengan Flexbox, kita bisa:

- Menyusun elemen secara horizontal/vertikal

- Mengatur ukuran otomatis berdasarkan ruang yang tersedia

- Membuat layout yang responsif tanpa media query kompleks

## 1. Dasar Flexbox

Untuk menggunakan Flexbox, kita harus menetapkan elemen sebagai **flex container**:

```css
.container {
  display: flex;
}
```

Elemen di dalamnya otomatis menjadi **flex item**.

## 2. Properti untuk Flex Container

- display: flex atau inline-flex
  Mengubah elemen menjadi flex container.

- flex-direction
  Menentukan arah utama (main axis) dari flex item.

```css
.container {
  flex-direction: row; /* default: horizontal dari kiri ke kanan */
  flex-direction: row-reverse; /* horizontal dari kanan ke kiri */
  flex-direction: column; /* vertikal dari atas ke bawah */
  flex-direction: column-reverse; /* vertikal dari bawah ke atas */
}
```

- justify-content
  Mengatur posisi item di sepanjang main axis (arah utama).

```css
.container {
  justify-content: flex-start; /* default, mulai dari kiri/atas */
  justify-content: center; /* tengah */
  justify-content: flex-end; /* akhir */
  justify-content: space-between; /* antar item */
  justify-content: space-around; /* ruang sekitar */
  justify-content: space-evenly; /* ruang sama rata */
}
```

![Justify Content](https://miro.medium.com/v2/resize:fit:640/format:webp/1*iigDGiNFBOUVJQ_07C1B2g.png)
_Source: CSS Tricks_

- align-items
  Mengatur posisi item di sepanjang cross axis (silang dari main axis).

```css
.container {
  align-items: stretch; /* default, isi seluruh tinggi container */
  align-items: flex-start;
  align-items: center;
  align-items: flex-end;
  align-items: baseline;
}
```

![Align Items](https://css-tricks.com/wp-content/uploads/2018/10/align-items.svg)
_Source: CSS Tricks_

- align-content
  Mengatur posisi baris flex jika lebih dari satu baris.

```css
.container {
  align-content: stretch;
  align-content: center;
  align-content: flex-start;
  align-content: flex-end;
  align-content: space-between;
  align-content: space-around;
}
```

![Align Content](https://css-tricks.com/wp-content/uploads/2018/10/align-content.svg)
_Source: CSS Tricks_

- flex-wrap
  Menentukan apakah item akan membungkus (wrap) jika melebihi lebar container.

```css
.container {
  flex-wrap: nowrap; /* default */
  flex-wrap: wrap; /* item membungkus */
  flex-wrap: wrap-reverse; /* item membungkus, tapi dari bawah ke atas (miror) */
}
```

> [!info] Shorthand flex-flow
> Gabungan dari flex-direction dan flex-wrap.
>
> ```css
> .container {
>   flex-flow: row wrap;
> }
> ```

## 3. Properti untuk Flex Item

- order
  Menentukan urutan item. Nilai default adalah 0.

```css
.item {
  order: 2; /* makin kecil = makin awal muncul */
}
```

![Order](https://css-tricks.com/wp-content/uploads/2018/10/order.svg)
_Source: CSS Tricks_

- flex-grow
  Menentukan seberapa besar item akan berkembang untuk mengisi ruang kosong.

```css
.item {
  flex-grow: 1; /* item akan tumbuh jika ada ruang kosong */
}
```

![flexgrow](https://css-tricks.com/wp-content/uploads/2018/10/flex-grow.svg)
_Source: CSS Tricks_

- flex-shrink
  Menentukan seberapa besar item akan menyusut ketika ruang tidak cukup.

```css
.item {
  flex-shrink: 1; /* default, item akan menyusut jika perlu */
}
```

- flex-basis
  Menentukan ukuran awal item sebelum flex-grow atau flex-shrink diterapkan.

```css
.item {
  flex-basis: 200px;
}
```

- align-self
  Mengatur perataan khusus untuk satu item saja (override align-items).

```css
.item {
  align-self: center;
}
```

![Align self](https://css-tricks.com/wp-content/uploads/2018/10/align-self.svg)
_Source: CSS Tricks_

## 4. Tips & Trik Flexbox

- Gunakan flex: 1 untuk membuat elemen berbagi lebar secara merata.

- Gunakan margin: auto untuk menengahkan item secara vertikal atau horizontal.

- Flexbox sangat cocok untuk navbar, card layout, form, dan component centering.

> [!tip] Materi Telah Selesai!
>
> Kembali ke Home [](/)
