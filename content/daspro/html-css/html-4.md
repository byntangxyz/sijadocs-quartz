---
title: 1.4. Membuat Form HTML
date: 2025-05-18
---

# Membuat Form HTML

Formulir (form) di HTML digunakan untuk mengumpulkan data dari pengguna, seperti nama, email, password, dan lainnya. Form sering digunakan dalam halaman pendaftaran, login, pencarian, dan sebagainya.

## Struktur Dasar Form

Tag utama yang digunakan adalah `<form>`, di dalamnya berisi berbagai elemen input:

```html
<form action="/submit" method="POST">
  <label for="nama">Nama:</label>
  <input type="text" id="nama" name="nama" />

  <br />

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" />

  <br />

  <input type="submit" value="Kirim" />
</form>
```

## Atribut Penting pada `<form>`

- action: URL tujuan untuk mengirim data.

- method: Metode pengiriman (GET atau POST).

- target: Tempat untuk menampilkan respons (misalnya \_blank, \_self).

## Jenis-Jenis Input

1. Teks

```html
<input type="text" name="nama" />
```

2. Email

```html
<input type="email" name="email" />
```

3. Password

```html
<input type="password" name="password" />
```

4. Radio Button

```html
<input type="radio" name="gender" value="Laki-laki" /> Laki-laki
<input type="radio" name="gender" value="Perempuan" /> Perempuan
```

5. Checkbox

```html
<input type="checkbox" name="hobi" value="Membaca" /> Membaca
<input type="checkbox" name="hobi" value="Menulis" /> Menulis
```

6. Select (Dropdown)

```html
<select name="kota">
  <option value="jakarta">Jakarta</option>
  <option value="bandung">Bandung</option>
</select>
```

7. Textarea (Teks Panjang)

```html
<textarea name="pesan" rows="4" cols="30"></textarea>
```

8. Tombol Kirim

```html
<input type="submit" value="Kirim" /> <button type="submit">Submit</button>
```

## Label dan Aksesibilitas

Gunakan tag `<label>` untuk menghubungkan teks label ke input dengan atribut for.

```html
<label for="nama">Nama Lengkap:</label> <input type="text" id="nama" name="nama" />
```

## Validasi Form HTML

HTML5 menyediakan atribut validasi otomatis:

- required: Wajib diisi.

- min, max: Untuk angka.

- pattern: Untuk mencocokkan pola regex.

- maxlength, minlength: Batas panjang karakter.

Contoh:

```html
<input type="email" name="email" required />
<input type="text" name="nama" minlength="3" maxlength="20" />
```

## Contoh Form Lengkap

```html
<form action="/kirim" method="POST">
  <label for="nama">Nama:</label>
  <input type="text" id="nama" name="nama" required />

  <br />

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required />

  <br />

  <label for="pesan">Pesan:</label>
  <textarea id="pesan" name="pesan" required></textarea>

  <br />

  <input type="submit" value="Kirim" />
</form>
```
