---
title: 3. Variabel dan Tipe Data
date: 2025-05-17
---

# Variabel dan Tipe Data

Apa itu variabel dan tipe data?
Apapun bahasa pemrograman yang digunakan. Dua hal ini akan selalu ada.

## Apa itu Variabel?

Variabel adalah sebuah nama yang mewakili sebuah nilai. Variabel bisa diisi dengan berbagai macam nilai seperti string (teks), number (angka), objek, array, dan sebagainya. Kita bisa ibaratkan, variabel itu seperti wadah untuk menyimpan sesuatu.

Dibahsa pemrograman javascript, terdapat 3 cara membuat variabel, yaitu:

### Variabel Mutable dengan `var` dan `let`

```javascript
var nama = "Bintang"

console.log(nama)
```

kode diatas akan menghasilkan output `"Bintang"` pada console. Output `"Bintang"` ini mempunyai [tipe data](#apa-itu-tipe-data) _string_. `Variabel yang menggunakan var dan let disebut variabel mutable karena nilai variabel ini bisa diubah`. Perhatikan kode berikut

```javascript
let umur = 16
umur = 17

console.log(umur)
```

Berapakah output dari variabel `umur`? Karena variabel `let` bersifat mutable maka output dari `umur` menjadi 17 bukan lagi 16.

### Variabel Immutable dengan `const`

Kalian tau [Konstanta](<https://id.wikipedia.org/wiki/Konstanta_(matematika)>)? atau kalian mengenal rumus-rumus pada pelajaran matematika ataupun fisika? Contohnya saja rumus Gaya (F) = Massa (m) x percepatan (a). Disoal apapun, kalian tidak mungkin mengubah rumus tersebut. Begitu juga dengan variabel immutable, variabel ini tidak bisa diubah isinya.

```javascript
const sekolah = "SMKN 2 Depok"
console.log(sekolah) // output: "SMKN 2 Depok"

const guru = "Pak Eka"
guru = "Pak Yun"
console.log(guru) // error: Assignment to constant variable.
```

## Apa itu Tipe Data?

Tipe data adalah jenis data yang digunakan untuk menyimpan nilai. Berikut adalah tipe data pada bahasa pemrograman javascript:

### Tipe Data Primitif

- **String**: Bernilai teks

```javascript
let nama = "Eko"
```

- **Number**: Bernilai angka

```javascript
let umur = 20
```

- **Boolean**: Bernilai true atau false

```javascript
let lulus = true
```

- **Null**: Bernilai kosong

```javascript
let data = null
```

- **Undefined**: Belum memiliki nilai

```javascript
let alamat
console.log(alamat) // undefined
```

### Tipe Data Non-Primitif

- **Object**: Kumpulan data dalam pasangan key-value

```javascript
const siswa = {
  nama: "Doni Kurniawan",
  umur: 17,
  jurusan: "SIJA",
}
```

- **Array**: Kumpulan data dalam satu variabel. Aray juga dapat dibuat didalam array (Nested Array).

```javascript
const angka = [1, 2, 3, 4, 5]
const SiswaSija = [
  ["Fino", 7],
  ["Miko", 34],
  ["Dinda", 1],
  ["Gaza", 28],
]
```

> [!tip] Berikutnya!
>
> [ Operator dan Build-In Objects](javascript-4.md)
