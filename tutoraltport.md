# Cara Memakai Port Alternatif
Jika ISP anda menggunakan *Transparent DNS Proxy*, maka anda tidak akan bisa menggunakan **bebasdns** melalui Do53 IPv4/6.<br>
Untuk mengelabuhi, maka itu memakai *port alternatif* agar bisa menggunakan **bebasdns**.

### MikroTik

Salin dan tempel skrip di bawah ini ke terminal:

``` 
/ip firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=tcp to-addresses=147.139.211.126 to-ports=1753
/ip firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=udp to-addresses=147.139.211.126 to-ports=1753
/ip firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=tcp to-addresses=47.254.192.66 to-ports=1753
/ip firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=udp to-addresses=47.254.192.66 to-ports=1753
```

<b>Jika jaringan anda mendukung IPv6 dan MikroTik telah di konfigurasikan untuk IPv6 (RouterOS versi 7 atau tinggi)</b><br>
```
/ipv6 firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=tcp to-address=2001:470:36:b90:beba:5::1d to-ports=1753
/ipv6 firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=udp to-address=2001:470:36:b90:beba:5::1d to-ports=1753
```
<sup>Telkomsel dan XL Axiata menggunakan <i>Transparent DNS Proxy</i> untuk IPv6 nya juga. Pastikan anda menjalankan perintah IPv6 diatas dan menggunakan kedua ISP tersebut.</sup>


### GoodbyeDPI

Silahkan tambahkan baris ini di belakang GoodbyeDPI.exe
>  --dns-addr 147.139.211.126 --dns-port 1753

### Pi-Hole
**1. Tambahkan baris di bawah ini ke Custom DNS dan jangan lupa di ceklist.**
```
47.254.192.66#1753
147.139.211.126#1753
```
![Pi-Hole](https://media.discordapp.net/attachments/1059052464919298049/1059052488428372030/image.png)

**2. Lalu klik simpan.**


### Periksa Konfigurasi sudah bekerja atau tidak

**Untuk memperiksa bahwa konfigurasi sudah bekerja dengan baik, buka Command Prompt lalu ketik:**
```
nslookup lamanlabuh.aduankonten.id
```

Jika hasil yang keluar adalah `0.0.0.0`, `127.0.0.1`, `::`, atau `Server Failed`, maka **bebasdn** sudah berfungsi dan terpakai.
