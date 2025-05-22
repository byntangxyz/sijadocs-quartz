---
title: 1.1. IP Address
date: 2025-05-21
---
## Selamat datang pada materi IP Address
>Apa itu IP Address?
>
**IP Address (Internet Protocol Address)** adalah alamat unik yang digunakan untuk mengidentifikasi perangkat (komputer, printer, smartphone, router, dll.) di dalam jaringan komputer, baik jaringan lokal (LAN) maupun jaringan internet.

IP Address berfungsi seperti alamat rumah: jika ingin mengirim data (seperti paket), maka sistem harus tahu ke mana data tersebut harus dikirim, yaitu ke alamat IP tujuan.
>
1. **Berdasarkan Versi Protokol** <br>
    - **IPv4** (Internet Protocol version 4)
    Panjang alamat: **32-bit**
    Format: empat **angka desimal** yang dipisahkan oleh titik, contoh: 192.168.1.1
    Jumlah kombinasi: sekitar 4,3 miliar alamat
    Versi paling umum digunakan saat ini <br>
    - **IPv6** (Internet Protocol version 6)
    Panjang alamat: **128-bit**
    Format: delapan **blok angka heksadesimal** yang dipisahkan oleh titik dua, contoh: 2001:0db8:85a3:0000:0000:8a2e:0370:7334
    Dirancang untuk menggantikan IPv4 karena keterbatasan jumlah alamat
    Memiliki kapasitas alamat yang jauh lebih besar dan mendukung fitur keamanan tambahan

2. **Berdasarkan Penggunaan Jaringan**
    - Public IP Address
    Digunakan untuk komunikasi melalui internet
    Diberikan oleh ISP (Internet Service Provider)
    Dapat **diakses secara global dari jaringan luar**

    - Private IP Address
    Digunakan dalam jaringan lokal (LAN)
    Tidak dapat diakses secara langsung dari internet
    Umumnya digunakan oleh <strong>perangkat di rumah atau kantor</strong>

        Contoh rentang:

    - ClassFull

            Class A: 10.0.0.0 – 10.255.255.255
            Subnet mask default: 255.0.0.0 (/8)

            Class B: 172.16.0.0 – 172.31.255.255
            Subnet mask default: 255.255.0.0 (/16)

            Class C: 192.168.0.0 – 192.168.255.255
            Subnet mask default: 255.255.255.0 (/24)

    - ClassLess

        | CIDR | Subnet Mask     | Jumlah Subnet | Host per Subnet |
        | ---- | --------------- | ------------- | --------------- |
        | /24  | 255.255.255.0   | 1             | 254             |
        | /25  | 255.255.255.128 | 2             | 126             |
        | /26  | 255.255.255.192 | 4             | 62              |
        | /27  | 255.255.255.224 | 8             | 30              |
        | /28  | 255.255.255.240 | 16            | 14              |
        | /29  | 255.255.255.248 | 32            | 6               |
        | /30  | 255.255.255.252 | 64            | 2               |

        

3. **Berdasarkan Penetapan IP**
    - Static IP Address
    Alamat IP tetap yang ditetapkan secara manual
    Cocok digunakan untuk server atau perangkat yang memerlukan koneksi stabil

    - Dynamic IP Address
    Alamat IP yang diberikan secara otomatis oleh DHCP server
    Bisa berubah setiap kali perangkat terhubung ke jaringan

    Umumnya digunakan untuk perangkat pengguna umum seperti laptop dan smartphone
>
>
>[!tip] Materi Berikutnya!
>
>Lanjut ke [Subnetting](ipaddress-2.md)
