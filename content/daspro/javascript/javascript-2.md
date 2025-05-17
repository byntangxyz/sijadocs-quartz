---
title: 2. Menulis Kode Javascript
date: 2025-05-17
---

# Beberapa cara menulis kode javascript

Karena [javascript](javascript-1.md) adalah bahasa pemrograman berbasis web, maka cara untuk menulis kode javascript bisa menggunakan file html. Untuk mendapatkan output dari kode javascript kalian bisa melihat pada bagian `console` pada web browser (dengan inspect element atau developer tools)

## Menulis Javascript pada tag `<script>`

Penulisan kode Javascript menggunakan tag `<script>` adalah cara umum yang digunakan.

Tag <script> dapat kita buat di dalam tag `<head>` maupun `<body>`.

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <title>Penulisan Javascript</title>
  </head>
  <body>
    <script>
      console.log("Javascript itu keren!")
    </script>
  </body>
</html>
```

## Menulis Javascript pada file eksternal `(.js)`

Jika menggunakan file eksternal kalian harus membuat 2 file, yaitu `index.html` dan `script.js` (namanya bebas namun wajib menggunakan ekstensi `.js`). Setelah itu menambahkan pada tag `<script>`, atribut `src` dengan alamat file javascript yang kalian buat.

Contoh

```html
<script src="script.js"></script>
```

Setelah itu kalian tinggal menulis kode javscript pada file `script.js` tersebut.

> [!tip] Berikutnya
>
> [Variabel dan Tipe Data](javascript-3.md)

> [!info] Just info
>
> Sebenarnya ada satu cara lagi untuk menulis kode javascript namun tidak menggunakan file html alias tidak memakai console web browser sebagai output. Cara ini biasa digunakan untuk menulis kode aplikasi non-web, misalnya script untuk mengatur sistem operasi, membuat bot/services, dan lain-lain. Dengan memanfaatkan [NodeJS](https://nodejs.org) kalian cukup menjalankan kode javascript dengan menggunakan perintah `node {nama-file.js}` di terminal.
