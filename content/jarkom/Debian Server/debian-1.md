---
title: 1.1. Installation
date: 2025-5-28
---
1.  
<img src="dokumentasi.png" alt="dokumentasi" width="650" height="550">

2.  
<img src="dokumentasi0.png" alt="dokumentasi0" width="650" height="550">

3.  
<img src="dokumentasi1.png" alt="dokumentasi1" width="650" height="550">

4.  
<img src="dokumentasi2.png" alt="dokumentasi2" width="650" height="550">

5.  
<img src="dokumentasi3.png" alt="dokumentasi3" width="650" height="550">

6.  
<img src="dokumentasi4.png" alt="dokumentasi4" width="650" height="550">

7.  
<img src="dokumentasi5.png" alt="dokumentasi5" width="650" height="550">

8.  
<img src="dokumentasi6.png" alt="dokumentasi6" width="650" height="550">

9.  
<img src="dokumentasi7.png" alt="dokumentasi7" width="650" height="550">

10.  
<img src="dokumentasi8.png" alt="dokumentasi8" width="650" height="550">

11.  
<img src="dokumentasi9.png" alt="dokumentasi9" width="650" height="550">

12.  
<img src="dokumentasi10.png" alt="dokumentasi10" width="650" height="550">

13.  
<img src="dokumentasi11.png" alt="dokumentasi11" width="650" height="550">

14.  
<img src="dokumentasi12.png" alt="dokumentasi12" width="650" height="550">

15.  
<img src="dokumentasi13.png" alt="dokumentasi13" width="650" height="550">

16.  
<img src="dokumentasi14.png" alt="dokumentasi14" width="650" height="550">

17.  
<img src="dokumentasi15.png" alt="dokumentasi15" width="650" height="550">

18.  
<img src="dokumentasi16.png" alt="dokumentasi16" width="650" height="550">

19.  
<img src="dokumentasi17.png" alt="dokumentasi17" width="650" height="550">

20.  
<img src="dokumentasi18.png" alt="dokumentasi18" width="650" height="550">

21.  
<img src="dokumentasi19.png" alt="dokumentasi19" width="650" height="550">

22.  
<img src="dokumentasi20.png" alt="dokumentasi20" width="650" height="550">

23.  
<img src="dokumentasi21.png" alt="dokumentasi21" width="650" height="550">

24.  
<img src="dokumentasi22.png" alt="dokumentasi22" width="650" height="550">

25.  Aktifkan SSH dengan command ```nano /etc/ssh/sshd_config```
<img src="dokumentasi23.png" alt="dokumentasi23" width="750" height="650">

26.  "Active" menandakan ssh sudah dapat dilakukan dengan ```ssh user@ip-address```
<img src="dokumentasi24.png" alt="dokumentasi24" width="750" height="650">

27.  Cari repositori terdekat dan ubah dengan link repo yang tersedia : saya menggunakan repo SMKN 2 Depok
<img src="dokumentasi26.png" alt="dokumentasi25" width="650" height="550">
```
    deb http://repo.stembayo.sch.id/debian/ bookworm main non-free-firmware                 
    deb-src http://repo.stembayo.sch.id/debian/ bookworm main non-free-firmware
    deb http://repo.stembayo.sch.id/debian-security bookworm-security main non-free-firmware
    deb-src http://repo.stembayo.sch.id/debian-security bookworm-security main non-free-firmware
    deb http://repo.stembayo.sch.id/debian bookworm-updates main non-free-firmware
    deb-src http://repo.stembayo.sch.id/debian bookworm-updates main non-free-firmware
```
28. Setelah mengganti, jangan lupa ```apt update```
<img src="dokumentasi25.png" alt="dokumentasi25" width="650" height="550">

