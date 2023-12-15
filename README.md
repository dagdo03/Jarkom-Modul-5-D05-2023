# Jarkom-Modul-5-D05-2023
Laporan Resmi Praktikum Modul 5 Jaringan Komputer 2023

## Author
| Nama | NRP |Github |
|---------------------------|------------|--------|
|Ihsan Widagdo | 5025211231 | https://github.com/dagdo03 |
|Sandyatama Fransisna Nugraha | 5025211196 | https://github.com/TamaFn |

## Daftar Isi
- [Topologi](#topologi)
  - [Topologi pada GNS3](#topologi-pada-gns3)
  - [Pembagian Subnet](#pembagian-subnet)
- [VLSM](#vlsm)
  - [VLSM Tree](#vlsm-tree)
  - [Pembagian IP](#pembagian-ip)
- [Kendala](#kendala)

## Topologi

### Topologi pada GNS3
Berikut adalah topologi jaringan pada GNS3.  
![image](img/Topologi.png)

### Pembagian Subnet
Berikut adalah visualisasi pembagian subnet pada topologi jaringan.

![Subnet Map](img/Subnet.png)

## VLSM
### VLSM Tree

![Subnet Map](img/Tree.png)

### Pembagian IP

![Subnet Map](img/IP.png)

### Konfigurasi dan Routing
Berikut adalah konfigurasi jaringan tiap node pada topologi.
- Aura (Router)
```bash

```

- Freiren (Router)
```bash

```

- Heiter (Router)
```bash

```

- Himmel (Router)
```bash

```

- Fern (Router)
```bash

```

- Sein (Web Server)
```bash

```

- Stark (Web Server)
```bash

```

- Richter (DNS Server)
```bash

```

- Revolte (DHCP Server)
```bash

```

- TurkRegion (Client : 1022 Host) 
```bash

```

- GrobeForest (Client : 512 Host)
```bash

```

- LaubHills (Client : 255 Host) 
```bash

```

- SchwerMountain (Client : 64 Host) 
```bash

```

### Berikut adalah konfigurasi routing pada tiap node.
- Aura
```bash

```
- Frieren
```bash

```
- Heiter
```bash

```
- Himmel
```bash

```
- Fern
```bash

```

## Testing

## Soal Praktikum

1. Agar topologi yang kalian buat dapat mengakses keluar, kalian diminta untuk mengkonfigurasi Aura menggunakan iptables, tetapi tidak ingin menggunakan MASQUERADE

![Subnet Map](img/IP.png)

2. Kalian diminta untuk melakukan drop semua TCP dan UDP kecuali port 8080 pada TCP.

![Subnet Map](img/IP.png)

3. Kepala Suku North Area meminta kalian untuk membatasi DHCP dan DNS Server hanya dapat dilakukan ping oleh maksimal 3 device secara bersamaan, selebihnya akan di drop.

![Subnet Map](img/IP.png)

4. Lakukan pembatasan sehingga koneksi SSH pada Web Server hanya dapat dilakukan oleh masyarakat yang berada pada GrobeForest.

![Subnet Map](img/IP.png)

5. Selain itu, akses menuju WebServer hanya diperbolehkan saat jam kerja yaitu Senin-Jumat pada pukul 08.00-16.00.

![Subnet Map](img/IP.png)

6. Lalu, karena ternyata terdapat beberapa waktu di mana network administrator dari WebServer tidak bisa stand by, sehingga perlu ditambahkan rule bahwa akses pada hari Senin - Kamis pada jam 12.00 - 13.00 dilarang (istirahat maksi cuy) dan akses di hari Jumat pada jam 11.00 - 13.00 juga dilarang (maklum, Jumatan rek).

![Subnet Map](img/IP.png)

7. Karena terdapat 2 WebServer, kalian diminta agar setiap client yang mengakses Sein dengan Port 80 akan didistribusikan secara bergantian pada Sein dan Stark secara berurutan dan request dari client yang mengakses Stark dengan port 443 akan didistribusikan secara bergantian pada Sein dan Stark secara berurutan.

![Subnet Map](img/IP.png)

8. Karena berbeda koalisi politik, maka subnet dengan masyarakat yang berada pada Revolte dilarang keras mengakses WebServer hingga masa pencoblosan pemilu kepala suku 2024 berakhir. Masa pemilu (hingga pemungutan dan penghitungan suara selesai) kepala suku bersamaan dengan masa pemilu Presiden dan Wakil Presiden Indonesia 2024.

![Subnet Map](img/IP.png)

9. Sadar akan adanya potensial saling serang antar kubu politik, maka WebServer harus dapat secara otomatis memblokir  alamat IP yang melakukan scanning port dalam jumlah banyak (maksimal 20 scan port) di dalam selang waktu 10 menit. 
(clue: test dengan nmap)

![Subnet Map](img/IP.png)

10. Karena kepala suku ingin tau paket apa saja yang di-drop, maka di setiap node server dan router ditambahkan logging paket yang di-drop dengan standard syslog level. 

![Subnet Map](img/IP.png)

## Kendala
