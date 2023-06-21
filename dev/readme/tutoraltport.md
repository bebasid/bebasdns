# Cara Memakai Port Alternatif
Jika ISP-nya menggunakan *Transparent DNS Proxy*, maka itu tidak akan bisa menggunakan **bebasdns** melalui Do53 IPv4/6.<br>
Untuk mengelabuhi, yaitu memakai *port alternatif* agar bisa menggunakan **bebasdns**.

### MikroTik

Salin dan tempel skrip di bawah ini ke terminal:

<b>PILIH SALAH SATU</b>

<b>Default DNS</b>

``` 
/ip firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=tcp to-addresses=103.87.68.24 to-ports=1753
/ip firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=udp to-addresses=103.87.68.24 to-ports=1753
```

```
/ipv6 firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=tcp to-address=2a06:1287:1605:5353::beba:51d to-ports=1753
/ipv6 firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=udp to-address=2a06:1287:1605:5353::beba:51d to-ports=1753
```

<b>Malware Blocking Only (Hanya memblokir situs malware)</b>

``` 
/ip firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=tcp to-addresses=103.87.68.23 to-ports=1753
/ip firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=udp to-addresses=103.87.68.23 to-ports=1753
```

```
/ipv6 firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=tcp to-address=2001:df1:7340:c::beba:51d to-ports=1753
/ipv6 firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=udp to-address=2001:df1:7340:c::beba:51d to-ports=1753
```

### GoodbyeDPI

**1. Pilih ``2_any_country_dnsredir.cmd``, tekan Edit atau buka di __Notepad++__** *(Jika memiliki program pihak ke-tiga)*

![tutorialygy](https://media.discordapp.net/attachments/1059052464919298049/1107666667732992130/image.png)

**2. Gantikan baris di bawah ini ke bagian ``start "" goodbyedpi.exe -5``**
>  --dns-addr 103.87.68.24 --dns-port 1753 --dnsv6-addr 2a06:1287:1605:5353::beba:51d --dnsv6-port 1753

![goodbyedpi](https://media.discordapp.net/attachments/1059052464919298049/1107664890761580574/image.png)

**3. Lalu, simpan file ``2_any_country_dnsredir.cmd`` tersebut.**

### Pi-Hole
**1. Tambahkan baris di bawah ini ke Custom DNS dan wajib di ceklist.**

Custom 1 (IPv4): ``103.87.68.24#1753``

Custom 2 (IPv4): ``103.87.68.23#1753``

![Pi-Hole](https://media.discordapp.net/attachments/1059052464919298049/1059052488428372030/image.png)

**2. Lalu klik simpan.**

### Periksa Konfigurasi sudah berfungsi atau belum

**Untuk memperiksa bahwa konfigurasi sudah bekerja dengan baik, buka Command Prompt lalu ketik:**
```
nslookup lamanlabuh.aduankonten.id
```
![cek](https://media.discordapp.net/attachments/1059052464919298049/1107658636001542154/image.png)

Jika hasil yang keluar adalah `0.0.0.0`, `127.0.0.1`, `::`, atau `Server Failed`, maka **bebasdns** sudah berfungsi dan terpakai.

