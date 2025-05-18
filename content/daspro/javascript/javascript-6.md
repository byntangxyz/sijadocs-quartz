---
title: 6. Fungsi
date: 2025-05-17
---

# Fungsi (Function) dalam JavaScript

Dalam pemrograman, **fungsi** adalah blok kode yang dirancang untuk melakukan tugas tertentu. Fungsi memungkinkan kita untuk menulis kode yang **terstruktur, dapat digunakan ulang (reusable), dan mudah dirawat**.

---

## Apa itu Fungsi?

Fungsi adalah sub-program yang bisa digunakan kembali, baik di dalam program itu sendiri maupun di program lain. Di JavaScript, fungsi merupakan objek karena memiliki properti dan metode.

---

## Cara Membuat Fungsi di JavaScript

Ada tiga cara untuk membuat fungsi di JavaScript:

### 1. Menggunakan Cara Biasa

Cara ini paling sering digunakan, terutama bagi yang baru belajar JavaScript.

```js
function namaFungsi() {
  console.log("Hello World!")
}
```

### 2. Menggunakan Ekspresi

Kita menggunakan variabel, lalu diisi dengan fungsi anonim (tanpa nama).

```js
var namaFungsi = function () {
  console.log("Hello World!")
}
```

### 3. Menggunakan Tanda Panah (Arrow Function)

Cara ini sering digunakan di kode JavaScript masa kini karena lebih sederhana. Namun, mungkin sulit dipahami bagi pemula. Fungsi ini mulai muncul pada standar ES6.

```js
var namaFungsi = () => {
  console.log("Hello World!")
}
```

## Cara Memanggil atau Mengeksekusi Fungsi

Setelah mengetahui cara membuat fungsi, lalu bagaimana cara memanggilnya?

Kita bisa memanggil fungsi di dalam kode JavaScript dengan menuliskan nama fungsinya seperti ini:

```js
namaFungsi()
```

Contoh:

```js
// membuat fungsi
function sayHello() {
  console.log("Hello World!")
}

// memanggil fungsi
sayHello() // Output: Hello World!
```

## Fungsi dengan Parameter

Parameter adalah variabel yang menyimpan nilai untuk diproses di dalam fungsi. Contoh:

```js
function kali(a, b) {
  var hasilKali = a * b
  console.log("Hasil kali a*b = " + hasilKali)
}
```

Pada contoh di atas, a dan b adalah parameter. Cara memanggil fungsi yang memiliki parameter:

```js
kali(3, 2) // Output: Hasil kali a*b = 6
```

## Fungsi yang Mengembalikan Nilai

Agar hasil pengolahan nilai di dalam fungsi dapat digunakan untuk proses berikutnya, maka fungsi harus mengembalikan nilai. Pengembalian nilai pada fungsi menggunakan kata kunci return. Contoh:

```js
function bagi(a, b) {
  var hasilBagi = a / b
  return hasilBagi
}

// memanggil fungsi
var nilai1 = 20
var nilai2 = 5
var hasilPembagian = bagi(nilai1, nilai2)
console.log(hasilPembagian) // Output: 4
```

> [!tip] Berikutnya!
>
> [Perulangan](javascript-7.md)
