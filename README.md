# bebasdns

_Membantumu berselancar dengan aman dan tidak terbatas!_

**bebasdns** mengimplementasikan sistem DNS sekaligus ad-blocker yang dijalankan dengan menggunakan VPS/VPN uptime yang cukup stabil dan tidak menyimpan kueri. 

**bebasdns** juga support top-level domain dari [OpenNIC](https://www.opennic.org/) sehingga pengalaman sebagai mengakses website menjadi lebih bebas.
**bebasdns** menonaktifkan fitur log dikarenakan privasi pengguna, selain itu juga tidak penting, dan tentu saja karena memakan resource. 

Sewaktu-waktu hanya akan mengaktifkan menyimpan kueri apabila jika adanya laporan bug. 
Misalnya, tidak bisa mengakses sebuah website dengan tujuan untuk melacak sumber masalah dan mengatasi laporan bug tersebut.

# Peladen
| Protocol | Address | Port |
| -------- | ------- | ---- |
| DNS, IPv4 | **1:** ``147.139.211.126`` (CGK), ㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤ    ㅤㅤㅤ        **2:** ``47.254.192.66`` (KUL) | **1:** ``53``, ㅤㅤㅤㅤ**2:** ``1753`` | 
| DNS, IPv6 | **1:** ``2001:470:36:9be:ba5::1d`` (SIN), ㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤ        **2:** ``2001:470:36:b90:beba:5::1d`` (KUL) | **1:** ``53``, ㅤㅤㅤ   **2:** ``1753`` |  
| DNS-over-HTTPS | ``https://dns.bebasid.com/dns-query/`` | |
| DNS-over-TLS | ``dns.bebasid.com`` | |
| DNS-over-QUIC | ``quic://dns.bebasid.com`` |
| iOS/macOS | [dns.mobileconfig](https://raw.githubusercontent.com/bebasid/bebasdns/main/dns.mobileconfig) | |

|  DNSCrypt Protocol   |                                         Address                                            |
|----------------------|--------------------------------------------------------------------------------------------|
| IPv4, DNS-over-HTTPS | **1:** ``sdns://AgcAAAAAAAAADzE0Ny4xMzkuMjExLjEyNgAPZG5zLmJlYmFzaWQuY29tCi9kbnMtcXVlcnk`` (CGK), ㅤㅤㅤ**2:** ``sdns://AgcAAAAAAAAADTQ3LjI1NC4xOTIuNjYAD2Rucy5iZWJhc2lkLmNvbQovZG5zLXF1ZXJ5`` (KUL) |           
| IPv6, DNS-over-HTTPS | **1:** ``sdns://AgcAAAAAAAAAGVsyMDAxOjQ3MDozNjo5YmU6YmE1OjoxZF0AD2Rucy5iZWJhc2lkLmNvbQovZG5zLXF1ZXJ5`` (SIN),ㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤ      **2:** ``sdns://AgcAAAAAAAAAHFsyMDAxOjQ3MDozNjpiOTA6YmViYTo1OjoxZF0AD2Rucy5iZWJhc2lkLmNvbQovZG5zLXF1ZXJ5`` (KUL) | 



# Peladen Alternatif

### Unfiltered 
Khusus tanpa pemblokiran iklan, malware dan konten dewasa.

| Protocol | Address |
|----------|---------|
| DNS-over-HTTPS | ``https://dns.bebasid.com/dns-query/unfiltered/`` | 
| DNS-over-TLS   | ``unfiltered.dns.bebasid.com`` |
| DNS-over-QUIC  | ``quic://unfiltered.dns.bebasid.com`` | 

|  DNSCrypt Protocol   |                                         Address                                                                |
|----------------------|----------------------------------------------------------------------------------------------------------------|
|IPv4, DNS-over-HTTPS  | ``sdns://AgcAAAAAAAAADzE0Ny4xMzkuMjExLjEyNgAPZG5zLmJlYmFzaWQuY29tFS9kbnMtcXVlcnkvdW5maWx0ZXJlZA``              |
|IPv6, DNS-over-HTTPS  | ``sdns://AgcAAAAAAAAAGVsyMDAxOjQ3MDozNjo5YmU6YmE1OjoxZF0AD2Rucy5iZWJhc2lkLmNvbRUvZG5zLXF1ZXJ5L3VuZmlsdGVyZWQ`` |

### Malware 
Khusus pemblokiran malware dan tanpa mmeblokir iklan.

| Protocol       |                                         Address                                            |
|----------------|--------------------------------------------------------------------------------------------| 
| DNS-over-HTTPS | ``https://dns.bebasid.com/dns-query/malware/``                                             | 
| DNS-over-TLS   | ``malware.dns.bebasid.com``                                                                |
| DNS-over-QUIC  | ``quic://malware.dns.bebasid.com``                                                         | 

|  DNSCrypt Protocol   |                                                  Address                                                    |
|----------------------|-------------------------------------------------------------------------------------------------------------|
|IPv4, DNS-over-HTTPS  | ``sdns://AgcAAAAAAAAADzE0Ny4xMzkuMjExLjEyNgAPZG5zLmJlYmFzaWQuY29tEi9kbnMtcXVlcnkvbWFsd2FyZQ``               |
|IPv6, DNS-over-HTTPS  | ``sdns://AgcAAAAAAAAAGVsyMDAxOjQ3MDozNjo5YmU6YmE1OjoxZF0AD2Rucy5iZWJhc2lkLmNvbRIvZG5zLXF1ZXJ5L21hbHdhcmU``  |

### Family
Khusus pemblokiran malware dan konten dewasa.

| Protocol       |                                         Address                                            |
|----------------|--------------------------------------------------------------------------------------------|
| DNS-over-HTTPS | ``https://dns.bebasid.com/dns-query/family/``                                              | 
| DNS-over-TLS   | ``family.dns.bebasid.com``                                                                 |
| DNS-over-QUIC  | ``quic://family.dns.bebasid.com``                                                          | 

|  DNSCrypt Protocol   |                                                Address                                                    |
|----------------------|-----------------------------------------------------------------------------------------------------------|
|IPv4, DNS-over-HTTPS  | ``sdns://AgcAAAAAAAAADzE0Ny4xMzkuMjExLjEyNgAPZG5zLmJlYmFzaWQuY29tES9kbnMtcXVlcnkvZmFtaWx5``               |
|IPv6, DNS-over-HTTPS  | ``sdns://AgcAAAAAAAAAGVsyMDAxOjQ3MDozNjo5YmU6YmE1OjoxZF0AD2Rucy5iZWJhc2lkLmNvbREvZG5zLXF1ZXJ5L2ZhbWlseQ`` |

# Daftar Blokir DNS
| Blocklist                                                                                                         | Enabled |
|-------------------------------------------------------------------------------------------------------------------|---------|
| [AdGuard](https://adguardteam.github.io/AdGuardSDNSFilter/Filters/filter.txt)                                     | ✓       |
| [NoTracking](https://raw.githubusercontent.com/notracking/hosts-blocklists/master/adblock/adblock.txt)            | ✓       |
| [ABPIndo](https://raw.githubusercontent.com/ABPindo/indonesianadblockrules/master/subscriptions/abpindo.txt)      | ✓       |
| [uBlock Origin](https://raw.githubusercontent.com/uBlockOrigin/uAssets/master/filters/filters.txt)                | ✓       |
| [uBlock Origin Filters](https://raw.githubusercontent.com/LanikSJ/ubo-filters/main/filters/combined-filters.txt)  | ✓       |
| [Peter Lowe’s list](https://pgl.yoyo.org/adservers/serverlist.php?hostformat=hosts&showintro=0&mimetype=plaintext)| X       |
| [EasyList](https://easylist.to/easylist/easylist.txt)                                                             | ✓       |
| [AdAway](https://adaway.org/hosts.txt)                                                                            | ✓       |
| [MVPS](https://winhelp2002.mvps.org/hosts.txt)                                                                    | ✓       |
| [Dan Pollock's list](https://someonewhocares.org/hosts/hosts)                                                     | X       |
| [ABP Oisd](https://abp.oisd.nl/)                                                                                  | ✓       |
| [Cameleon](https://sysctl.org/cameleon/hosts)                                                                     | ✓       |
| [Adblock Plus](https://easylist-downloads.adblockplus.org/abp-filters-anti-cv.txt)                                | ✓       |
| [URLhaus](https://malware-filter.gitlab.io/malware-filter/urlhaus-filter-agh.txt)                                 | ✓       |
| [EasyPrivacy](https://easylist.to/easylist/easyprivacy.txt)                                                       | ✓       |
| [NoCoin](https://raw.githubusercontent.com/hoshsadiq/adblock-nocoin-list/master/nocoin.txt)                       | ✓       |
| [YouTube Ad Blocklist](https://raw.githubusercontent.com/Ewpratten/youtube_ad_blocklist/master/blocklist.txt)     | ✓       |
| [WindowsSpyBlocker](https://raw.githubusercontent.com/crazy-max/WindowsSpyBlocker/master/data/hosts/spy.txt)      | ✓       |
| [AdBlockID](https://raw.githubusercontent.com/realodix/AdBlockID/master/output/adblockid.txt)                     | X        |
| [bebasdns Custom Filtering Rules Blocklist](https://raw.githubusercontent.com/bebasid/bebasdns/main/custom-filtering-rules-blocklist) | ✓      |
| [OISD Blocklist Full](https://raw.githubusercontent.com/deep-bhatt/huawei-block-list/master/huawei-block-host.txt)      | ✓      |
| [WindowsSpyBlocker](https://raw.githubusercontent.com/BlackJack8/iOSAdblockList/master/Hosts.txt)                       | ✓      |
| [URLHaus's Maliclious](https://raw.githubusercontent.com/BlackJack8/iOSAdblockList/master/Hosts.txt)                    | ✓      |

# Daftar Putih DNS
| Whitelist                                                                                                                             | Enabled |
|---------------------------------------------------------------------------------------------------------------------------------------|---------|
| [bebasdns Custom Filtering Rules Whitelist](https://raw.githubusercontent.com/bebasid/bebasdns/main/custom-filtering-rules-whitelist) | ✓       |
| [bebasdns Whitelist](https://raw.githubusercontent.com/bebasid/bebasdns/main/whitelist.txt)                                           | ✓       |
| [Filterlist for AdGuard](https://raw.githubusercontent.com/hl2guide/Filterlist-for-AdGuard-or-PiHole/master/filter_whitelist.txt)     | ✓       |
| [AdGuard Home Whitelist](https://raw.githubusercontent.com/hg1978/AdGuard-Home-Whitelist/master/whitelist.txt)                        | ✓       |
| [AdGuard Home Filters](https://raw.githubusercontent.com/mmotti/adguard-home-filters/master/whitelist.txt)                            | ✓       |

# Server Upstream DNS
| Default                                                                                                                               |
|---------------------------------------------------------------------------------------------------------------------------------------|
| [Cloudflare](https://www.cloudflare.com)                                                                                              | 

| [OpenNIC](https://www.opennic.org/)                                                                                                                  |
|------------------------------------------------------------------------------------------------------------------------------------------------------|
| glue, cyb, geek, free, indy, parody, bbs, null, oss, ing, dyn, gopher, micro, neo, pirate, oz, epic, o, chan, libre, fur, bazar, coin, emc, lib      |


# Status Peladen

Statistik kondisi servis pelayanan publik:

• [UptimeRobot](https://stats.uptimerobot.com/j5MjytjV8y)

# Cara Mengaplikasian

Silahkan ikuti panduan yang diberikan di bawah ini:

• [Plain DNS](https://github.com/bebasid/bebasdns/blob/main/tutoraltport.md)

• [DNS-over-HTTPS](https://github.com/pengelana/blocklist/wiki/DNS-over-HTTPS-(DoH))

• [DNS-over-TLS](https://github.com/pengelana/blocklist/wiki/DNS-over-TLS-(DoT))

• [DNS-over-QUIC](https://github.com/pengelana/blocklist/wiki/DNS-over-QUIC-(DoQ))

# Uji Keamanan

bebasdns telah diuji keamanannya dan mendapatkan nilai pada website: 

• [ImmuniWeb](https://www.immuniweb.com/ssl/dns.bebasid.com/M07B3FiY/) (A+) (May 14th, 2023).

# Donasi Kami

Bantu proyek ini agar tetap berjalan dengan cara berdonasi.

<div>
<details>
 <summary>:coffee: Traktir kita kopi.</summary>

</br>

<a href="https://trakteer.id/bebasidbykini"><img src="https://img.shields.io/static/v1?label=Trakteer&message=bebasidbykini&color=C02433"></a>

<a href="https://saweria.co/bebasid"><img src="https://img.shields.io/static/v1?label=Saweria&message=bebasid&color=FAAE2B"></a>
 
</details>
</div>

# Syarat dan Ketentuan

Dengan menggunakan layanan ini, anda setuju mematuhi peraturan yang kami buat dan menerima segala akibat yang ditimbulkan. Untuk selengkapnya, lihat [ATURAN](https://github.com/bebasid/bebasid/blob/master/dev/readme/RULES.md) nya.
