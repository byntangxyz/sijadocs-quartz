---
title: 7. Perulangan
date: 2025-05-17
---

# Perulangan dalam JavaScript

Dalam pemrograman, **perulangan** (looping) digunakan untuk menjalankan blok kode secara berulang selama kondisi tertentu masih terpenuhi. JavaScript menyediakan beberapa jenis perulangan yang bisa kita gunakan sesuai kebutuhan.

---

## 1. `for` Loop

Perulangan yang digunakan ketika kita tahu **berapa kali** perulangan akan dilakukan.

```js
for (let i = 0; i < 5; i++) {
  console.log("Perulangan ke-" + i)
}
```

Struktur for:

```text
for (inisialisasi; kondisi; increment/decrement) {
  // kode yang dijalankan
}
```

## 2. while Loop

Digunakan saat kita tidak tahu pasti berapa kali perulangan akan dilakukan, tapi tahu kondisinya.

```js
let i = 0

while (i < 5) {
  console.log("Nilai i adalah " + i)
  i++
}
```

Jika kondisi tidak pernah salah, maka akan terjadi infinite loop.

## 3. do...while Loop

Mirip seperti while, tapi perintah dijalankan minimal satu kali, walaupun kondisi awal false.

```js
let i = 0

do {
  console.log("Perulangan ke-" + i)
  i++
} while (i < 5)
```

## 4. for...of Loop

Digunakan untuk mengiterasi elemen pada array atau object iterable lainnya.

```js
let buah = ["apel", "jeruk", "mangga"]

for (let item of buah) {
  console.log(item)
}
```

## 5. for...in Loop (untuk objek)

Digunakan untuk mengiterasi properti pada objek.

```js
let siswa = {
  nama: "Andi",
  umur: 17,
  jurusan: "RPL",
}

for (let key in siswa) {
  console.log(key + ": " + siswa[key])
}
```

> [!tip] Materi Telah Selesai!
>
> Kembali ke Home [](/)
