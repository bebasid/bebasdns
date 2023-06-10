# Cara Memakai Port Alternatif
Jika ISP-nya menggunakan *Transparent DNS Proxy*, maka itu tidak akan bisa menggunakan **bebasdns** melalui Do53 IPv4/6.<br>
Untuk mengelabuhi, yaitu memakai *port alternatif* agar bisa menggunakan **bebasdns**.

### MikroTik

Salin dan tempel skrip di bawah ini ke terminal:

``` 
/ip firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=tcp to-addresses=147.139.211.126 to-ports=1753
/ip firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=udp to-addresses=147.139.211.126 to-ports=1753
/ip firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=tcp to-addresses=47.254.192.66 to-ports=1753
/ip firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=udp to-addresses=47.254.192.66 to-ports=1753
```

<b>Jika jaringan-nya mendukung IPv6 dan MikroTik telah di konfigurasikan untuk IPv6 (RouterOS versi 7 atau tinggi):</b><br>
```
/ipv6 firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=tcp to-address=2a06:1287:1605:5353::beba:51d to-ports=1753
/ipv6 firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=udp to-address=2a06:1287:1605:5353::beba:51d to-ports=1753
```
<sup>Telkomsel dan XL Axiata menggunakan <i>Transparent DNS Proxy</i> untuk IPv6 nya juga. Pastikan menjalankan perintah IPv6 diatas dan menggunakan kedua ISP tersebut.</sup>

### GoodbyeDPI

**1. Pilih ``2_any_country_dnsredir.cmd``, tekan Edit atau buka di __Notepad++__** *(Jika memiliki program pihak ke-tiga)*

![tutorialygy](https://media.discordapp.net/attachments/1059052464919298049/1107666667732992130/image.png)

**2. Gantikan baris di bawah ini ke bagian ``start "" goodbyedpi.exe -5``**
>  --dns-addr 147.139.211.126 --dns-port 1753 --dnsv6-addr 2001:470:36:9be:ba5::1d --dnsv6-port 1753

![goodbyedpi](https://media.discordapp.net/attachments/1059052464919298049/1107664890761580574/image.png)

**3. Lalu, simpan file ``2_any_country_dnsredir.cmd`` tersebut.**

### Pi-Hole
**1. Tambahkan baris di bawah ini ke Custom DNS dan wajib di ceklist.**

Custom 1 (IPv4): ``147.139.211.126#1753``

Custom 2 (IPv4): ``47.254.192.66#1753``

![Pi-Hole](https://media.discordapp.net/attachments/1059052464919298049/1059052488428372030/image.png)

**2. Lalu klik simpan.**

### Periksa Konfigurasi sudah berfungsi atau belum

**Untuk memperiksa bahwa konfigurasi sudah bekerja dengan baik, buka Command Prompt lalu ketik:**
```
nslookup lamanlabuh.aduankonten.id
```
![cek](https://media.discordapp.net/attachments/1059052464919298049/1107658636001542154/image.png)

Jika hasil yang keluar adalah `0.0.0.0`, `127.0.0.1`, `::`, atau `Server Failed`, maka **bebasdns** sudah berfungsi dan terpakai.

