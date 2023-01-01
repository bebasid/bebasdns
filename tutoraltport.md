# Tutorial pemakaian alt port
Jika ISP anda menggunakan *Transparent DNS Proxy*, maka anda tidak akan bisa menggunakan BebasDNS melalui Do53<br>
Untuk mengelabuhi itu, maka kita akan memakai *alt-port* agar anda bisa menggunakan BebasDNS.

### MikroTik

Silahkan copy & paste script ini di terminal:

```
/ip firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=tcp to-addresses=47.254.192.66 to-ports=1753
/ip firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=udp to-addresses=47.254.192.66 to-ports=1753
```

### GoodbyeDPI

Silahkan tambahkan line ini dibelakang GoodbyeDPI.exe
>  --dns-addr 47.254.192.66 --dns-port 1753

### Pi-Hole
**1. Silahkan tambahkan line ini di Custom DNS dan jangan lupa diceklist**
```
47.254.192.66#1753
```
![Pi-Hole](https://media.discordapp.net/attachments/1059052464919298049/1059052488428372030/image.png)

**2. Lalu ceklist Use DNSSEC**
![DNSSEC](https://media.discordapp.net/attachments/1059052464919298049/1059053083214225478/image.png)

**3. Click Save**



<br><br>**Untuk mengecek bahwa konfigurasi sudah bekerja dengan baik, silahkan buka Command Prompt dan ketik:**
```
nslookup lamanlabuh.aduankonten.id
```

Jika hasil yang keluar adalah `0.0.0.0` dan `::` atau `Server Failed`, maka BebasDNS sudah berfungsi
