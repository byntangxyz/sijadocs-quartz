---
title: 1.2. Subnetting
date: 2025-05-22
---


<iframe width="750" height="350" 
  src="https://www.youtube.com/embed/l5vLxYrZAgA?start=239" 
  title="OSI Layers" 
  frameborder="0" 
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
  allowfullscreen>
</iframe>

>Dari video Mas NanangMrk kita belajar banyak istilah baru

| Istilah           | Penjelasan                                                                 |
| ----------------- | -------------------------------------------------------------------------- |
| **IP Address**    | Alamat unik yang diberikan ke setiap perangkat dalam jaringan              |
| **Subnet Mask**   | Menentukan bagian mana dari IP yang mewakili network dan host              |
| **Network ID**    | Bagian dari IP address yang menunjukkan identitas jaringan                 |
| **Host ID**       | Bagian dari IP address yang menunjukkan identitas perangkat dalam jaringan |
| **CIDR Notation** | Format penulisan IP + prefix subnet, misal: `192.168.1.0/24`               |

>

## Tabel Subnet

| CIDR | Subnet Mask     | Jumlah Subnet | Host per Subnet |
| ---- | --------------- | ------------- | --------------- |
| /24  | 255.255.255.0   | 1             | 254             |
| /25  | 255.255.255.128 | 2             | 126             |
| /26  | 255.255.255.192 | 4             | 62              |
| /27  | 255.255.255.224 | 8             | 30              |
| /28  | 255.255.255.240 | 16            | 14              |
| /29  | 255.255.255.248 | 32            | 6               |
| /30  | 255.255.255.252 | 64            | 2               |

## Subnet Manual
1. **Tentukan IP Address dan Prefix**  
   Misalnya: IP = `192.168.10.0/24`
>
2. **Tentukan jumlah subnet yang dibutuhkan**  
   Misalnya: ingin membuat 4 subnet
>
3. **Hitung jumlah bit yang perlu dipinjam untuk subnet**  
   Gunakan rumus:  
   $2^n \geq \text{jumlah subnet}$  
   Contoh: 4 subnet → $2^2 = 4$ → pinjam 2 bit
>
4. **Hitung subnet mask baru**  
   Rumus:  
   $Prefix\ baru = Prefix\ awal + n$  
   Contoh: `/24 + 2 = /26`, maka subnet mask = `255.255.255.192`
>
5. **Hitung jumlah host per subnet**  
   Rumus:  
   $\text{Jumlah host} = 2^s - 2$  
   Di mana `s` adalah jumlah bit host  
   Contoh: 32 - 26 = 6 → $2^6 - 2 = 62$
>
6. **Hitung subnet increment**  
   Rumus:  
   $Subnet\ increment = 256 - \text{angka subnet mask pada oktet terakhir}$  
   Contoh: 256 - 192 = 64
>
7. **Tentukan tabel subnet**
    Lanjutkan dengan menghitung Network Address, First Host, Last Host, dan Broadcast Address untuk masing-masing subnet.
    | Subnet | Network Address | First Host     | Last Host      | Broadcast Address |
    | ------ | --------------- | -------------- | -------------- | ----------------- |
    | 1      | 192.168.10.0    | 192.168.10.1   | 192.168.10.62  | 192.168.10.63     |
    | 2      | 192.168.10.64   | 192.168.10.65  | 192.168.10.126 | 192.168.10.127    |
    | 3      | 192.168.10.128  | 192.168.10.129 | 192.168.10.190 | 192.168.10.191    |
    | 4      | 192.168.10.192  | 192.168.10.193 | 192.168.10.254 | 192.168.10.255    |
>
