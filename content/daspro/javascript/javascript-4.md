---
title: 4. Operator dan Build-In Objects
date: 2025-05-17
---

# Operator dan Built-in Objects di JavaScript

Setelah memahami [variabel dan tipe data](javascript-3.md), sekarang kita bahas **operator** dan beberapa **built-in objects** penting yang sering digunakan di JavaScript.

## Operator dalam JavaScript

Operator digunakan untuk melakukan operasi terhadap nilai (value) dan variabel. Berikut beberapa kategori utama:

### Operator Aritmatika

Digunakan untuk operasi matematika dasar.

| Operator | Fungsi      | Contoh         |
| -------- | ----------- | -------------- |
| `+`      | Penjumlahan | `5 + 3` → `8`  |
| `-`      | Pengurangan | `10 - 4` → `6` |
| `*`      | Perkalian   | `2 * 5` → `10` |
| `/`      | Pembagian   | `8 / 2` → `4`  |
| `%`      | Modulus     | `7 % 2` → `1`  |
| `**`     | Pangkat     | `2 ** 3` → `8` |

### Operator Perbandingan

Digunakan untuk membandingkan dua nilai.

| Operator | Fungsi                  | Contoh                |
| -------- | ----------------------- | --------------------- |
| `==`     | Sama nilai              | `5 == '5'` → `true`   |
| `===`    | Sama nilai & tipe       | `5 === '5'` → `false` |
| `!=`     | Tidak sama              | `5 != 3` → `true`     |
| `!==`    | Tidak sama (nilai/tipe) | `5 !== '5'` → `true`  |
| `>`      | Lebih besar             | `10 > 5` → `true`     |
| `<`      | Lebih kecil             | `3 < 7` → `true`      |
| `>=`     | Lebih besar atau sama   | `5 >= 5` → `true`     |
| `<=`     | Lebih kecil atau sama   | `4 <= 5` → `true`     |

### Operator Logika

Digunakan untuk logika boolean.

```
| Operator | Fungsi          | Contoh                   |
|----------|-----------------|--------------------------|
| `&&`     | AND             | `true && false` → `false`|
| `||`     | OR              | `true || false` → `true` |
| `!`      | NOT             | `!true` → `false`        |
```

### Operator Penugasan (Assignment Operators)

Operator ini digunakan untuk menentukan nilai baru untuk variabel.

| Operator | Fungsi                    | Contoh     | Arti          |
| -------- | ------------------------- | ---------- | ------------- |
| `=`      | Pengisian nilai           | `x = '5'`  | x = 5         |
| `+=`     | Pengisian dan penambahan  | `x += '5'` | x = x + 5     |
| `-=`     | Pengisian dan pengurangan | `x -= 5`   | x = x - 5     |
| `*=`     | Pengisian dan perkalian   | `x *= '5'` | x = x \* 5    |
| `**=`    | Pengisian dan pangkat     | `x **= 5`  | x = x \*\*= 5 |
| `/=`     | Pengisian dan bagi        | `x /= 2`   | x = x / 5     |
| `%=`     | Pengisian dan modulus     | `x %= 5`   | x = x % 5     |

Maksud dari operator penugasan adalah untuk mengubah nilai variabel dengan menggunakan operator yang sesuai. Misalnya

```javascript
let x = 5

x += 5 // x = 10 atau sama saja dengan x = x + 5
```

> [!info] Increment & Decrement
>
> Increment (`++`) digunakan untuk menambahkan 1 ke nilai variabel, sedangkan decrement (`--`) digunakan untuk mengurangi 1 dari nilai variabel. Cara ini akan sering digunakan untuk [Looping](javascript-7.md). Contoh penggunaannya adalah sebagai berikut:
>
> ```js
> let x = 5
> x++
> console.log(x) // 6
> ```

### Operator Ternary

Operator ini digunakan untuk menentukan nilai berdasarkan kondisi, sama seperti [if-else](javascript-5.md) tetapi hanya dipisahkan oleh tanda tanya (?) sebagai operator.

![ternary-petani-code](https://3.bp.blogspot.com/-OKB4MDtGjE4/WObxiPfq-wI/AAAAAAAAEmQ/kR9Ldcc1hr88u90060rCff0Gvs4lDRfQgCPcB/s1600/operator%2Bternary%2Bdi%2Bjava.png)
_Source: Petani Code_

## Built-in Objects di JavaScript

Built-in objects adalah objek yang sudah disediakan oleh JavaScript untuk mempermudah berbagai operasi umum.

### `Math` — Operasi Matematika

Contoh penggunaan:

```javascript
Math.PI // 3.14159...
Math.round(4.6) // 5
Math.floor(4.9) // 4
Math.ceil(4.1) // 5
Math.random() // Angka acak
```

### 2. Date — Tanggal dan Waktu

Contoh penggunaan:

```js
const sekarang = new Date()
console.log(sekarang.getFullYear()) // Tahun sekarang
console.log(sekarang.getMonth()) // Bulan (0 = Januari)
```

### 3. String — Objek untuk manipulasi teks

```javascript
let nama = "Tono"
console.log(nama.length) // 4
console.log(nama.toUpperCase()) // "TONO"
console.log(nama.includes("i")) // true
```

### 4. Array — Objek untuk daftar data

```js
const angka = [1, 2, 3, 4]
angka.push(5) // Tambah elemen ke akhir
angka.pop() // Hapus elemen terakhir
console.log(angka) // [1, 2, 3, 4]
```

> [!tip] Berikutnya!
>
> [IF ELSE](javascript-5.md)
