# bebasdns

Membantumu berselancar dengan aman dan tidak terbatas!.

bebasdns mengimplementasikan sistem DNS sekaligus AdBlocker yang dijalankan menggunakan Virtual Private Server dengan uptime yang cukup stabil dan tentu saja tanpa log. 

Kami menonaktifkan fitur log dikarenakan privasi pengguna, selain itu juga tidak penting, dan tentu saja karena memakan resource. Kami sewaktu-waktu hanya akan mengaktifkan log apabila adanya laporan kutu misalnya tidak bisa mengakses sebuah website dengan tujuan untuk melacak sumber masalah dan mengatasi laporan kutu tersebut.

# Peladen

DoH: https://dns.bebasid.com/dns-query

DoT: dns.bebasid.com

DoQ: quic://dns.bebasid.com

iOS/macOS: [dns.mobileconfig](https://raw.githubusercontent.com/bebasid/bebasdns/main/dns.mobileconfig)

# Daftar Blokir DNS
| Daftar Blokir                                                                                                     | Status |
|-------------------------------------------------------------------------------------------------------------------|--------|
| [AdGuard](https://adguardteam.github.io/AdGuardSDNSFilter/Filters/filter.txt)                                     | ✓      |
| [NoTracking](https://raw.githubusercontent.com/notracking/hosts-blocklists/master/adblock/adblock.txt)            | ✓      |
| [ABPIndo](https://raw.githubusercontent.com/ABPindo/indonesianadblockrules/master/subscriptions/abpindo.txt)      | ✓      |
| [uBlock Origin](https://raw.githubusercontent.com/uBlockOrigin/uAssets/master/filters/filters.txt)                | ✓      |
| [uBlock Origin Filters](https://raw.githubusercontent.com/LanikSJ/ubo-filters/main/filters/combined-filters.txt)  | ✓      |
| [Peter Lowe’s list](http://pgl.yoyo.org/adservers/serverlist.php?hostformat=hosts&showintro=0&mimetype=plaintext) | ✓      |
| [EasyList](https://easylist.to/easylist/easylist.txt)                                                             | ✓      |
| [StevenBlack](https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts)                                   | ✓      |
| [AdAway](https://adaway.org/hosts.txt)                                                                            | ✓      |
| [MVPS](https://winhelp2002.mvps.org/hosts.txt)                                                                    | ✓      |
| [Dan Pollock's list](https://someonewhocares.org/hosts/hosts)                                                     | ✓      |
| [oisd](https://abp.oisd.nl/)                                                                                      | ✓      |
| [Cameleon](http://sysctl.org/cameleon/hosts)                                                                      | ✓      |
| [Adblock Plus](https://easylist-downloads.adblockplus.org/abp-filters-anti-cv.txt)                                | ✓      |
| [URLhaus](https://malware-filter.gitlab.io/malware-filter/urlhaus-filter-agh.txt)                                 | ✓      |
| [EasyPrivacy](https://easylist.to/easylist/easyprivacy.txt)                                                       | ✓      |
| [NoCoin](https://raw.githubusercontent.com/hoshsadiq/adblock-nocoin-list/master/nocoin.txt)                       | ✓      |
| [YouTube Ad Blocklist](https://raw.githubusercontent.com/Ewpratten/youtube_ad_blocklist/master/blocklist.txt)     | ✓      |
| [WindowsSpyBlocker](https://raw.githubusercontent.com/crazy-max/WindowsSpyBlocker/master/data/hosts/spy.txt)      | ✓      |
| [AdBlockID](https://raw.githubusercontent.com/realodix/AdBlockID/master/output/adblockid.txt)                     | ✓      |
| [iOSAdblockList](https://raw.githubusercontent.com/BlackJack8/iOSAdblockList/master/Hosts.txt)                    | ✓      |
| [Huawei Block List](https://raw.githubusercontent.com/deep-bhatt/huawei-block-list/master/huawei-block-host.txt)  | ✓      |
| [Energized](https://block.energized.pro/ultimate/formats/hosts)                                                   | X      |
| [Mahakala](http://adblock.mahakala.is/)                                                                           | X      |
| [Tiarapp](https://raw.githubusercontent.com/pengelana/blocklist/master/domain.txt)                                | X      |
| [blah](https://oooo.b-cdn.net/blahdns/lite_adblocker.txt)                                                         | X      |
| [Developerdan](https://www.github.developerdan.com/hosts/lists/ads-and-tracking-extended.txt)                     | X      |
| [1Hosts](https://raw.githubusercontent.com/badmojr/1Hosts/master/Lite/adblock.txt)                                | X      |
| [TheBlockListProject](https://blocklistproject.github.io/Lists/adguard/ads-ags.txt)                               | X      |

# Daftar Putih DNS
| Daftar Putih                                                                                                                      | Status |
|-----------------------------------------------------------------------------------------------------------------------------------|--------|
| [bebasdns Custom Filtering Rules](https://raw.githubusercontent.com/bebasid/bebasdns/main/custom-filtering-rules)                 | ✓      |
| [bebasdns Whitelist](https://raw.githubusercontent.com/bebasid/bebasdns/main/whitelist.txt)                                       | ✓      |
| [Filterlist for AdGuard](https://raw.githubusercontent.com/hl2guide/Filterlist-for-AdGuard-or-PiHole/master/filter_whitelist.txt) | ✓      |
| [AdGuard Home Whitelist](https://raw.githubusercontent.com/hg1978/AdGuard-Home-Whitelist/master/whitelist.txt)                    | ✓      |
| [AdGuard Home Filters](https://raw.githubusercontent.com/mmotti/adguard-home-filters/master/whitelist.txt)                        | ✓      |

# Status Peladen

Statistik kondisi peladen - [status](https://stats.uptimerobot.com/j5MjytjV8y)

# Cara Pengaplikasian

Untuk cara pengaplikasian, silahkan ikuti panduan yang diberikan teman kami, pengelana.

[DNS-over-HTTPS](https://github.com/pengelana/blocklist/wiki/DNS-over-HTTPS-(DoH))

[DNS-over-TLS](https://github.com/pengelana/blocklist/wiki/DNS-over-TLS-(DoT))

[DNS-over-QUIC](https://github.com/pengelana/blocklist/wiki/DNS-over-QUIC-(DoQ))

# Uji Keamanan

bebasdns telah diuji keamanannya dan mendapatkan nilai A+ pada website [ImmuniWeb](https://www.immuniweb.com/ssl/dns.bebasid.com/AjUEXAbS/).

# Donasi Kami

Bantu proyek ini tetap berjalan dengan cara berdonasi.

<div>
<details>
 <summary>:coffee: Traktir kita kopi</summary>

</br>

<a href="https://trakteer.id/bebasidbykini"><img src="https://img.shields.io/static/v1?label=Trakteer&message=bebasidbykini&color=C02433"></a>

<a href="https://saweria.co/bebasid"><img src="https://img.shields.io/static/v1?label=Saweria&message=bebasid&color=FAAE2B"></a>
 
</details>
</div>

# Syarat & Ketentuan

Dengan menggunakan layanan ini, Anda setuju mematuhi peraturan yang kami buat dan Anda menerima segala akibat yang ditimbulkan. Untuk selengkapnya, lihat [ATURAN](https://github.com/bebasid/bebasid/blob/master/dev/readme/RULES.md) nya.
