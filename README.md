<head>
    <meta name="google-site-verification" content="rMj01w-DUdd0GIucGjWQKzZV-w6IE0hYYCWJWYnvfSw">
    <meta name="keywords" content="dns bebas blokir, bypass internet positif, bypass lamanlabuh, buka reddit, buka vimeo, dns bebas, dns bebas akses, dns pribadi bebas blokir, bypass trustpositif, alternatif bebasid, cara buka reddit tanpa vpn, lamanlabuh" />
</head>
<p align="center">
    <b>Sponsored by Atharva</b><br><br>
        <img src="https://github.com/bebasid/bebasdns/blob/main/dev/resources/logo/sponsor/atharva.svg#gh-light-mode-only" width="250">
    <img src="https://github.com/bebasid/bebasdns/blob/main/dev/resources/logo/sponsor/atharva_white.svg#gh-dark-mode-only" width="250">
    </a><br>
    <i>A freedom oriented and neutral VPS provider for your need</i><br>
    <a href="https://delapan.click/store/vps-ssd-kvm">Starting from Rp 50k</a>
</p>
<hr>
<p align="center">
    <b>Untuk ISP yang memakai DPI, gunakan <a href="https://github.com/bebasid/bebasit">bebasit</a> untuk melewati DPI atau menyalakan IPv6 jika ISP-nya mendukung.</b>
    <br><sup>Ciri-Ciri ISP anda menggunakan DPI: HTTP mengalihkan ke <code><a href="http://lamanlabuh.aduankonten.id" target="_blank">lamanlabuh.aduankonten.id</a></code> atau HTTPS keluar <code>ERR_CONNECTION_RESET</code>/<code>PR_CONNECT_RESET_ERROR</code></sup><br>
    <b>Bypass DPI Kominfo di Modem/Router:</b><br>
    <a href="https://github.com/bebasid/bebasit/blob/master/docs/openwrt-tutorial.md">OpenWRT</a> |
    <a href="https://github.com/bebasid/bebasit/blob/master/docs/mikrotik-tutorial.md">MikroTik</a>
</p>
<p align="center">
    <img src="https://github.com/bebasid/bebasdns/blob/main/dev/resources/logo/logo-black.png#gh-light-mode-only" alt="bebasDNS Black Logo" width="330">
    <img src="https://github.com/bebasid/bebasdns/blob/main/dev/resources/logo/logo.png#gh-dark-mode-only" alt="bebasDNS White Logo" width="330">
</p>
<p align="center">
<a href="https://discord.gg/EKrxZyu"><img src="https://discordapp.com/api/guilds/630415907021389825/widget.png?style=banner2" alt="Join Discord BEBASID"></a>
 </p>
<p align="center">
<a href="#"><img src="https://img.shields.io/static/v1?label=tahun%20diluncurkan:&message=2020&color=yellowgreen&style=plastic%22"></a>
 <a href="https://ready.chair6.net/?url=dns.bebasid.com"><img src="https://img.shields.io/badge/ipv6-ready-blue"></a>
  <a href="https://stats.uptimerobot.com/j5MjytjV8y"><img src="https://img.shields.io/badge/status-up-brightgreen"></a>
 <a href='https://www.immuniweb.com/ssl/dns.bebasid.com/M07B3FiY'><img src="https://img.shields.io/badge/imuniweb-A%2B-brightgreen"></a>
<a href="#"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fbebasid%2Fbebasdns_fGHyh&count_bg=%234572CD&title_bg=%23555555&icon_color=%23E7E7E7&title=penonton%3A+%28hari%20ini%2Ftotal%29&edge_flat=false"/></a>
<a href="https://github.com/bebasid/bebasdns/blob/main/LICENSE"><img src="https://img.shields.io/badge/lisensi-MIT-green"></a>
</p>
<p align="center">Donasi kami:</br>
<a href="https://trakteer.id/bebasidbykini"><img src="https://img.shields.io/static/v1?label=Trakteer&message=bebasidbykini&color=C02433"></a>
<a href="https://saweria.co/bebasid"><img src="https://img.shields.io/static/v1?label=Saweria&message=bebasid&color=FAAE2B"></a>
 </p>
<p align="center">
    <b>Indonesia</b> | <a href="README.en.md">English</a>
</p>

---

## Daftar Isi

- [bebasdns](#bebasdns)
  + [Peladen](#peladen)
    - [Alternatif](#peladen-alternatif)
      + [Unfiltered](#unfiltered)
      + [Malware](#malware)
      + [Family](#family)
  + [Penyaring](#penyaring)
    - [Daftar Blokir DNS](#daftar-blokir-dns)
    - [Daftar Putih DNS](#daftar-putih-dns)
  + [Server Upstream DNS](#server-upstream-dns)
  + [Pemeliharaan](#pemeliharaan)
    - [Status Peladen](#status-peladen)
    - [Uji Keamanan](#uji-keamanan)
  + [Isi Tutorial dan Bertanya](#isi-tutorial-dan-bertanya)
    - [Cara Mengaplikasikan](#cara-mengaplikasikan)
    - [Cara Melaporkan, atau Permintaan](#cara-melaporkan-atau-permintaan)
    - [Soal Sering Ditanya](#soal-sering-ditanya)
  + [Donasi Kami](#donasi-kami)
  + [Lisensi](#lisensi)
  + [Syarat dan Ketentuan](#syarat-dan-ketentuan)

---

# bebasdns

_Membantumu berselancar dengan aman dan tidak terbatas!_

**bebasdns** mengimplementasikan sistem DNS sekaligus ad-blocker yang dijalankan dengan menggunakan VPS/VPN uptime yang cukup stabil dan tidak menyimpan kueri. 

**bebasdns** juga support top-level domain dari [OpenNIC](https://www.opennic.org/) sehingga pengalaman sebagai mengakses website menjadi lebih bebas.
**bebasdns** menonaktifkan fitur log dikarenakan privasi pengguna, selain itu juga tidak penting, dan tentu saja karena memakan resource. 

Sewaktu-waktu hanya akan mengaktifkan menyimpan kueri apabila jika adanya laporan bug. 
Misalnya, tidak bisa mengakses sebuah website dengan tujuan untuk melacak sumber masalah dan mengatasi laporan bug tersebut.

## Peladen
| Protocol | Address | Port |
| -------- | ------- | :--: |
| DNS, IPv4 | ``103.87.68.24`` | ``53``, ``1753`` | 
| DNS, IPv6 | ``2a06:1287:1605:5353::beba:51d`` | ``53``,  ``1753`` |  
| DNS-over-HTTPS | ``https://dns.bebasid.com/dns-query`` | ``443`` |
| DNS-over-TLS | ``dns.bebasid.com`` | ``853`` |
| DNS-over-QUIC | ``quic://dns.bebasid.com`` | ``853`` |
| iOS | [dns.mobileconfig](https://raw.githubusercontent.com/bebasid/bebasdns/main/dev/resources/config/dns.mobileconfig) | |
| macOS | [dns-macos.mobileconfig](https://raw.githubusercontent.com/bebasid/bebasdns/main/dev/resources/config/dns-macos.mobileconfig) | |

|  DNSCrypt Protocol   |                                         Address                                            |
|----------------------|--------------------------------------------------------------------------------------------|
| IPv4, DNS-over-HTTPS | ``sdns://AgcAAAAAAAAADzE0Ny4xMzkuMjExLjEyNgAPZG5zLmJlYmFzaWQuY29tCi9kbnMtcXVlcnk`` (CGK), ``sdns://AgcAAAAAAAAADTQ3LjI1NC4xOTIuNjYAD2Rucy5iZWJhc2lkLmNvbQovZG5zLXF1ZXJ5`` (KUL) |           
| IPv6, DNS-over-HTTPS | ``sdns://AgcAAAAAAAAAGVsyMDAxOjQ3MDozNjo5YmU6YmE1OjoxZF0AD2Rucy5iZWJhc2lkLmNvbQovZG5zLXF1ZXJ5`` (CGK), ``sdns://AgcAAAAAAAAAHFsyMDAxOjQ3MDozNjpiOTA6YmViYTo1OjoxZF0AD2Rucy5iZWJhc2lkLmNvbQovZG5zLXF1ZXJ5`` (KUL) | 



## Peladen Alternatif

### <ins>Malware</ins> 
Khusus pemblokiran malware dan tanpa memblokir iklan.

| Protocol | Address | Port |
| -------- | ------- | :--: |
| DNS-over-HTTPS | ``https://malware.dns.bebasid.com/dns-query`` | ``443`` |
| DNS-over-TLS | ``malware.dns.bebasid.com`` | ``853`` |
| DNS-over-QUIC | ``quic://malware.dns.bebasid.com`` | ``853`` |

### <ins>Family</ins> 
Khusus pemblokiran family dan malware.

| Protocol | Address | Port |
| -------- | ------- | :--: |
| DNS-over-HTTPS | ``https://family.dns.bebasid.com/dns-query`` | ``443`` |
| DNS-over-TLS | ``family.dns.bebasid.com`` | ``853`` |
| DNS-over-QUIC | ``quic://family.dns.bebasid.com`` | ``853`` |

## Penyaring

Penyaring adalah sistem untuk memblokir akses ke konten tertentu di Internet. Saat membuka situs web, browser mengirimkan nama situs web (misalnya, <code>google.com</code>) ke server DNS. Server DNS menjawab dengan alamat IP server yang menyimpan situs web ini.</br>

Daftar Blokir DNS digunakan untuk memblokir domain yang diketahui menjalankan iklan atau pelacak.</br>
Daftar Putih DNS digunakan untuk membolehkan domain yang seharusnya diblokir oleh daftar blokir.</br>

### <ins>Daftar Blokir DNS</ins>
| Blocklist                                                                                                         |
|-------------------------------------------------------------------------------------------------------------------|
| [AdGuard](https://adguardteam.github.io/AdGuardSDNSFilter/Filters/filter.txt)                                     | 
| [WindowsSpyBlocker](https://raw.githubusercontent.com/crazy-max/WindowsSpyBlocker/master/data/hosts/spy.txt)      |
| [bebasdns's Custom Filtering Blocklist Rules](https://raw.githubusercontent.com/bebasid/bebasdns/main/dev/resources/hosts/custom-filtering-rules-blocklist) | 
| [OISD Blocklist Full](https://raw.githubusercontent.com/deep-bhatt/huawei-block-list/master/huawei-block-host.txt)      | 
| [WindowsSpyBlocker](https://raw.githubusercontent.com/BlackJack8/iOSAdblockList/master/Hosts.txt)                       |
| [URLHaus's Maliclious](https://raw.githubusercontent.com/BlackJack8/iOSAdblockList/master/Hosts.txt)                    | 

### <ins>Daftar Putih DNS</ins>
| Whitelist                                                                                                                             |
|---------------------------------------------------------------------------------------------------------------------------------------|
| [bebasdns's Custom Filtering Wihtelist Rules](https://raw.githubusercontent.com/bebasid/bebasdns/main/dev/resources/hosts/custom-filtering-rules-whitelist) | 
| [bebasdns's Custom Filtering Whitelist Rules 2](https://raw.githubusercontent.com/bebasid/bebasdns/main/dev/resources/hosts/whitelist.txt) | 
| [Filterlist for AdGuard](https://raw.githubusercontent.com/hl2guide/Filterlist-for-AdGuard-or-PiHole/master/filter_whitelist.txt)     | 
| [AdGuard Home Whitelist](https://raw.githubusercontent.com/hg1978/AdGuard-Home-Whitelist/master/whitelist.txt)                        | 
| [AdGuard Home Filters](https://raw.githubusercontent.com/mmotti/adguard-home-filters/master/whitelist.txt)                            | 

## Server Upstream DNS
| Default                                                                                                                               |
|---------------------------------------------------------------------------------------------------------------------------------------|
| [Cloudflare](https://www.cloudflare.com)                                                                                              | 

| [OpenNIC](https://www.opennic.org/)                                                                                                                  |
|------------------------------------------------------------------------------------------------------------------------------------------------------|
| glue, cyb, geek, free, indy, parody, bbs, null, oss, ing, dyn, gopher, micro, neo, pirate, oz, epic, o, chan, libre, fur, bazar, coin, emc, lib      |


## Pemeliharaan

### <ins>Status Peladen</ins>

Statistik kondisi servis pelayanan publik:

• [UptimeRobot](https://stats.uptimerobot.com/w66Jkc0zm7)

### <ins>Uji Keamanan</ins>

bebasdns telah diuji keamanannya dan mendapatkan nilai pada website: 

• [ImmuniWeb](https://www.immuniweb.com/websec/dns.bebasid.com/TzfTp42V/) (A+) (May 14th, 2023).

## Isi Tutorial dan Bertanya

### <ins>Cara Mengaplikasikan</ins>

Silahkan ikuti panduan yang diberikan di bawah ini:

• [Plain DNS (Port Alternatif)](https://github.com/bebasid/bebasdns/blob/main/dev/readme/tutoraltport.md#cara-memakai-port-alternatif)

• [DNS-over-HTTPS](https://github.com/pengelana/blocklist/wiki/DNS-over-HTTPS-(DoH))

• [DNS-over-TLS](https://github.com/pengelana/blocklist/wiki/DNS-over-TLS-(DoT))

• [DNS-over-QUIC](https://github.com/pengelana/blocklist/wiki/DNS-over-QUIC-(DoQ))

• [Pi-Hole](https://github.com/bebasid/bebasdns/blob/main/dev/readme/tutoraltport.md#pi-hole)

• [DNSCrypt](https://libreddit.eu.org/r/indonesia/comments/kyyxna/comment/gjjq578/)

• [GoodbyeDPI](https://github.com/bebasid/bebasdns/blob/main/dev/readme/tutoraltport.md#goodbyedpi)

• [MikroTik](https://github.com/bebasid/bebasdns/blob/main/dev/readme/tutoraltport.md#mikrotik)

• [iOS](https://libreddit.eu.org/r/indonesia/comments/kyyxna/comment/gjke3u7)/[macOS](https://translate.google.com/translate?hl=id&sl=en&u=https://simpledns.plus/kb/201/how-to-enable-dns-over-tls-dot-dns-over-https-doh-in-macos-v11&prev=search&pto=aue)

### <ins>Cara Melaporkan, atau Permintaan</ins>

Untuk melakukan permintaan dan melaporkan adanya kutu (_bug_), silahkan [membuka isu baru](https://github.com/bebasid/bebasdns/issues/new/choose).

### <ins>Soal Sering Ditanya</ins>

Jika mengalami permasalahan saat menggunakan bebasid, silahkan lanjut menanyakannya di [Discord](https://discord.gg/EKrxZyu).

Atau anda bisa email ke `dukungan@bebasid.com` dengan subject **BebasDNS: [Masalah/pertanyaan anda]**

## Donasi Kami

Bantu proyek ini agar tetap berjalan dengan cara berdonasi.

<div>
<details>
 <summary>:coffee: Traktir kita kopi.</summary>

</br>

<a href="https://trakteer.id/bebasidbykini"><img src="https://img.shields.io/static/v1?label=Trakteer&message=bebasidbykini&color=C02433"></a>

<a href="https://saweria.co/bebasid"><img src="https://img.shields.io/static/v1?label=Saweria&message=bebasid&color=FAAE2B"></a>
 
</details>
</div>

## Lisensi

bebasdns dilisensikan di bawah [Lisensi MPL-2.0](https://github.com/bebasid/bebasdns/blob/main/LICENSE).

---

# Syarat dan Ketentuan

Dengan menggunakan layanan ini, anda setuju mematuhi peraturan yang kami buat dan menerima segala akibat yang ditimbulkan. Untuk selengkapnya, lihat [ATURAN](https://github.com/bebasid/bebasdns/blob/main/dev/readme/RULES.md) nya.
