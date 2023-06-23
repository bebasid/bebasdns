# Cara Mengaplikasikan / Memakai Port Alternatif
Jika ISP-nya menggunakan *Transparent DNS Proxy*, maka itu tidak akan bisa menggunakan **BebasDNS / BebasID DNS** melalui `Do53 IPv4/6`.<br>
Untuk mengelabuhi, yaitu dengan cara memakai *port alternatif* pada tersebut.

### MikroTik

Salin dan tempelkan skrip di bawah ini ke terminal tersebut.

<b><ins>PILIH SALAH SATU SKRIP BebasDNS / BebasID DNS UNTUK DIGUNAKAN.</ins></b>

<b>Default DNS</b>:

``` 
/ip firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=tcp to-addresses=103.87.68.24 to-ports=1753
/ip firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=udp to-addresses=103.87.68.24 to-ports=1753
```

```
/ipv6 firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=tcp to-address=2a06:1287:1605:5353::beba:51d to-ports=1753
/ipv6 firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=udp to-address=2a06:1287:1605:5353::beba:51d to-ports=1753
```
</br>
<b>Antivirus (Malware) Blocking Only</b> <i>(Hanya memblokir situs malware)</i>:

``` 
/ip firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=tcp to-addresses=103.87.68.23 to-ports=1753
/ip firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=udp to-addresses=103.87.68.23 to-ports=1753
```

```
/ipv6 firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=tcp to-address=2001:df1:7340:c::beba:51d to-ports=1753
/ipv6 firewall nat add action=dst-nat chain=dstnat comment="DNS BebasID" dst-port=53 protocol=udp to-address=2001:df1:7340:c::beba:51d to-ports=1753
```

### GoodbyeDPI

**1. Pilih ``2_any_country_dnsredir.cmd``, tekan Edit atau buka di __Notepad++__** *(Jika memiliki program pihak ke-tiga)*.

![tutorialygy](https://media.discordapp.net/attachments/1059052464919298049/1107666667732992130/image.png)

**2. Gantikan baris di bawah ini ke bagian ``start "" goodbyedpi.exe -5``**.</br></br>
<b><ins>PILIH SALAH SATU SKRIP BebasDNS / BebasID DNS UNTUK DIGUNAKAN</ins>.</b></br></br>
<b>Default DNS:</b></br>
>  --dns-addr 103.87.68.24 --dns-port 1753 --dnsv6-addr 2a06:1287:1605:5353::beba:51d --dnsv6-port 1753

</br>

<b>Antivirus (Malware) Blocking Only</b> <i>(Hanya memblokir situs malware)</i>:</br>
>  --dns-addr 103.87.68.23 --dns-port 1753 --dnsv6-addr 2001:df1:7340:c::beba:51d --dnsv6-port 1753

</br>

![goodbyedpi](https://media.discordapp.net/attachments/1059052464919298049/1107664890761580574/image.png)

**3. Lalu, simpan file di bagian ``2_any_country_dnsredir.cmd`` pada tersebut.**

### Pi-Hole
**1. Tambahkan baris di bawah ini ke Custom DNS bagian (IPv4) dan wajib di ceklist semua.**

Custom 1 (IPv4): ``103.87.68.24#53`` atau ``103.87.68.24#1753`` [Bagian DNS Default]

Custom 2 (IPv4): ``103.87.68.23#1753`` atau ``103.87.68.23#1753`` [Bagian DNS Antivirus (Malware)]

**2. Jika IPv6 mendukung, tambahkan baris di bawah ini ke Custom DNS bagian (IPv6) dan wajib di ceklist semua (Pilihan opsional atau lewatkan saja ke pilihan nomor 3, jika ISP-nya tidak mendukung IPv6).**

Custom 3 (IPv6): ``2a06:1287:1605:5353::beba:51d#53`` atau ``2a06:1287:1605:5353::beba:51d#1753`` [Bagian DNS Default]

Custom 4 (IPv6): ``2001:df1:7340:c::beba:51d#1753`` atau ``2001:df1:7340:c::beba:51d#1753`` [Bagian DNS Antivirus (Malware)]

![Pi-Hole](https://media.discordapp.net/attachments/1059052464919298049/1059052488428372030/image.png)

**3. Lalu klik simpan.**

### Periksa konfigurasi BebasDNS / BebasID DNS sudah berfungsi atau belum

**Untuk memperiksa bahwa konfigurasi sudah bekerja dengan baik, buka Command Prompt (CMD), lalu ketik:**
```
nslookup lamanlabuh.aduankonten.id
```
![cek](https://media.discordapp.net/attachments/1059052464919298049/1107658636001542154/image.png)

Maka hasil yang keluar adalah `0.0.0.0`, `127.0.0.1`, `::`, atau `Server Failed`, artinya **BebasDNS / BebasID DNS** sudah berfungsi dan sudah terpakai.

---

<p align="center">Semoga bermanfaat!</br></br>Share proyek ini!</p>
<div id="sosial">
 <p align="center">
  <a href="https://twitter.com/intent/tweet?text=https%3A//github.com/bebasid/bebasdns%20%23BlokirKominfo%20%23BlokirGakPakeMikir"><img src="https://img.shields.io/badge/Twitter-blue?style=flat&logo=twitter&logoColor=white"/></a>
  <a href="https://www.facebook.com/sharer/sharer.php?u=https%3A//github.com/bebasid/bebasdns"><img src="https://img.shields.io/badge/Facebook-1877F2?style=flat&logo=facebook&logoColor=white"/></a>
  <p align="center">
:coffee: Traktir kami kopi!
    </br>
<a href="https://trakteer.id/bebasidbykini"><img src="https://img.shields.io/static/v1?label=Trakteer&message=bebasidbykini&color=C02433"></a>
<a href="https://saweria.co/bebasid"><img src="https://img.shields.io/static/v1?label=Saweria&message=bebasid&color=FAAE2B"></a>
    </br>
    </p>
  <p align="center">
    <a href="https://github.com/bebasid/bebasdns#readme">BebasDNS / BebasID DNS</a> dilisensikan sebagai <a href="https://github.com/bebasid/bebasdns/blob/main/LICENSE">MPL-2.0</a>.
</p>
</div>
