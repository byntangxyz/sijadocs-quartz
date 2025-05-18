---
title: 5. Percabangan
date: 2025-05-17
---

# Percabangan dalam Javascript

Dalam dunia pemrograman, **percabangan** digunakan untuk menjalankan kode tertentu berdasarkan kondisi yang diberikan. Di JavaScript, ada beberapa cara untuk membuat percabangan.

## 1. `if` Statement

Digunakan untuk mengeksekusi blok kode **jika kondisi bernilai true**.

```js
let nilai = 80

if (nilai >= 75) {
  console.log("Kamu lulus!")
}
```

## 2. `if...else` Statement

Jika kondisi if tidak terpenuhi, maka blok else akan dijalankan.

```js
let umur = 16

if (umur >= 17) {
  console.log("Kamu sudah bisa bikin KTP.")
} else {
  console.log("Belum cukup umur.")
}
```

## 3. `if...else if...else`

Digunakan untuk mengecek beberapa kondisi berbeda.

```js
let nilai = 65

if (nilai >= 90) {
  console.log("Nilai kamu A")
} else if (nilai >= 75) {
  console.log("Nilai kamu B")
} else {
  console.log("Nilai kamu C")
}
```

## 4. Ternary Operator (? :)

Percabangan singkat dalam satu baris.

```js
let status = umur >= 17 ? "Dewasa" : "Remaja"
```

## 5. switch Statement

Digunakan ketika ada banyak kondisi dengan nilai tetap.

```js
let hari = "Senin"

switch (hari) {
  case "Senin":
    console.log("Hari pertama kerja")
    break
  case "Jumat":
    console.log("Hari terakhir kerja")
    break
  default:
    console.log("Hari biasa")
}
```

`break` digunakan untuk menghentikan eksekusi agar tidak lanjut ke case berikutnya.

> [!tip] Berikutnya!
>
> [Function](javascript-6.md)
