# Tutorial pemakaian alt port
Jika ISP anda menggunakan *Transparent DNS Proxy*, maka anda tidak akan bisa menggunakan BebasDNS melalui Do53<br>
Untuk mengelabuhi itu, maka kita akan memakai *alt-port* agar anda bisa menggunakan BebasDNS.

### MikroTik

Silahkan copy & paste script ini di terminal:

```
/ip firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=tcp to-addresses=47.254.192.66 to-ports=1753
/ip firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=udp to-addresses=47.254.192.66 to-ports=1753
```

<b>Jika jaringan anda support IPv6 dan MikroTik anda dikonfigurasikan untuk IPv6</b><br>
```
/ipv6 firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=tcp to-address=2001:470:36:b90:beba:5::1d to-ports=1753
/ipv6 firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=udp to-address=2001:470:36:b90:beba:5::1d to-ports=1753
```
<h3>Pastikan routeros anda berada di Versi 7 atau keatas untuk penggunaan IPv6!</h3>



### GoodbyeDPI

Silahkan tambahkan line ini dibelakang GoodbyeDPI.exe
>  --dns-addr 47.254.192.66 --dns-port 1753

### Pi-Hole
**1. Silahkan tambahkan line ini di Custom DNS dan jangan lupa diceklist**
```
47.254.192.66#1753
```
![Pi-Hole](https://media.discordapp.net/attachments/1059052464919298049/1059052488428372030/image.png)

**2. Click Save**



<br><br>**Untuk mengecek bahwa konfigurasi sudah bekerja dengan baik, silahkan buka Command Prompt dan ketik:**
```
nslookup lamanlabuh.aduankonten.id
```

Jika hasil yang keluar adalah `0.0.0.0` dan `::` atau `Server Failed`, maka BebasDNS sudah berfungsi
