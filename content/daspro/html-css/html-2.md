---
title: 1.2. Menambahkan Video dan Audio
date: 2025-05-18
---

# Menambahkan Video dan Audio kedalam HTML

## Menambahkan Video di HTML

Untuk menampilkan video, gunakan tag `<video>`. Tag ini bisa disertai dengan atribut seperti controls, autoplay, loop, dan muted.

Contoh dasar:

```html
<video width="640" height="360" controls>
  <source src="video.mp4" type="video/mp4" />
  Browser kamu tidak mendukung tag video.
</video>
```

## Atribut penting:

- controls: Menampilkan kontrol pemutar (play, pause, dll).

- autoplay: Memutar video otomatis saat halaman dimuat.

- loop: Memutar ulang video terus-menerus.

- muted: Menonaktifkan suara secara default.

- poster: Gambar yang ditampilkan sebelum video diputar.

Contoh dengan atribut tambahan:

```html
<video width="640" height="360" controls autoplay loop muted poster="thumbnail.jpg">
  <source src="video.mp4" type="video/mp4" />
  Video tidak dapat diputar di browser ini.
</video>
```

## Menambahkan Audio di HTML

Menambahkan Audio di HTML Untuk memutar suara atau musik, gunakan tag `<audio>`. Mirip seperti `<video>`, elemen ini juga mendukung berbagai atribut. Contoh dasar:

```html
<audio controls>
  <source src="audio.mp3" type="audio/mpeg" />
  Browser kamu tidak mendukung tag audio.
</audio>
```

## Atribut penting:

- controls: Menampilkan kontrol audio.
- autoplay: Memutar audio otomatis.
- loop: Mengulang audio terus-menerus.
- muted: Memulai dalam keadaan suara mati.

Contoh dengan atribut tambahan:

```html
<audio controls autoplay loop>
  <source src="musik.mp3" type="audio/mpeg" />
  Browser kamu tidak mendukung pemutar audio.
</audio>
```

Format File yang Didukung Untuk Video: `mp4` (paling umum dan didukung hampir semua browser), `webm`,
`ogg`

Untuk Audio: `mp3`, `ogg`, `wav`
Agar kompatibel di semua browser, disarankan menyediakan lebih dari satu format:

```html
<video controls>
  <source src="video.mp4" type="video/mp4" />
  <source src="video.webm" type="video/webm" />
  Browser kamu tidak mendukung video tag.
</video>
```

> [!tip] Materi Berikutnya!
>
> Lanjut ke [Membuat Tabel](html-3.md)
