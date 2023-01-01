# bebasdns

Membantumu berselancar dengan aman dan tidak terbatas!.

**bebasdns** mengimplementasikan sistem DNS sekaligus Ad-Blocker yang dijalankan menggunakan Virtual Private Server dengan uptime yang cukup stabil dan tentu saja tanpa log. 

**bebasdns** juga support tld dari [OpenNIC](https://www.opennic.org/) sehingga pengalaman anda mengakses website menjadi lebih bebas.

Kami menonaktifkan fitur log dikarenakan privasi pengguna, selain itu juga tidak penting, dan tentu saja karena memakan resource. Kami sewaktu-waktu hanya akan mengaktifkan log apabila adanya laporan kutu misalnya tidak bisa mengakses sebuah website dengan tujuan untuk melacak sumber masalah dan mengatasi laporan kutu tersebut.

# Peladen
• Do53: ``47.254.192.66`` Port Alternatif: ``1753``

• DoH: ``https://dns.bebasid.com/dns-query``

• DoT: ``dns.bebasid.com``

• DoQ: ``quic://dns.bebasid.com``

• DNSCrypt: ``sdns://AgcAAAAAAAAADTQ3LjI1NC4xOTIuNjYAD2Rucy5iZWJhc2lkLmNvbQovZG5zLXF1ZXJ5`` atau [``bebasdns``](https://dnscrypt.info/public-servers/)

• iOS/macOS: [dns.mobileconfig](https://raw.githubusercontent.com/bebasid/bebasdns/main/dns.mobileconfig)

# Peladen Alternatif

### Malware (Khusus Pemblokiran Malware)
• DoH: ``https://dns.bebasid.com/dns-query/malware``

• DoT: **malware.dns.bebasid.com (Segera Tersedia)**

### Family (Khusus Pemblokiran Malware & Konten Dewasa)
• DoH: ``https://dns.bebasid.com/dns-query/family``

• DoT: **family.dns.bebasid.com (Segera Tersedia)**

### Unfiltered (Khusus Tanpa pemblokiran Iklan, Malware & Konten Dewasa)
• DoH: ``https://dns.bebasid.com/dns-query/unfiltered``

• DoT: **unfiltered.dns.bebasid.com (Segera Tersedia)**

# Daftar Blokir DNS ― (08/09/2022)
| Daftar Blokir                                                                                                     | Status |
|-------------------------------------------------------------------------------------------------------------------|--------|
| [AdGuard](https://adguardteam.github.io/AdGuardSDNSFilter/Filters/filter.txt)                                     | ✓      |
| [NoTracking](https://raw.githubusercontent.com/notracking/hosts-blocklists/master/adblock/adblock.txt)            | ✓      |
| [ABPIndo](https://raw.githubusercontent.com/ABPindo/indonesianadblockrules/master/subscriptions/abpindo.txt) + [Hosts](https://raw.githubusercontent.com/ABPindo/indonesianadblockrules/master/subscriptions/hosts.txt)      | ✓      |
| [uBlock Origin](https://raw.githubusercontent.com/uBlockOrigin/uAssets/master/filters/filters.txt)                | ✓      |
| [uBlock Origin Filters](https://raw.githubusercontent.com/LanikSJ/ubo-filters/main/filters/combined-filters.txt)  | ✓      |
| [Peter Lowe’s list](https://pgl.yoyo.org/adservers/serverlist.php?hostformat=hosts&showintro=0&mimetype=plaintext)| ✓      |
| [EasyList](https://easylist.to/easylist/easylist.txt)                                                             | ✓      |
| [StevenBlack](https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts)                                   | ✓      |
| [AdAway](https://adaway.org/hosts.txt)                                                                            | ✓      |
| [MVPS](https://winhelp2002.mvps.org/hosts.txt)                                                                    | ✓      |
| [Dan Pollock's list](https://someonewhocares.org/hosts/hosts)                                                     | ✓      |
| [ABP Oisd](https://abp.oisd.nl/)                                                                                  | ✓      |
| [Cameleon](https://sysctl.org/cameleon/hosts)                                                                     | ✓      |
| [Adblock Plus](https://easylist-downloads.adblockplus.org/abp-filters-anti-cv.txt)                                | ✓      |
| [URLhaus](https://malware-filter.gitlab.io/malware-filter/urlhaus-filter-agh.txt)                                 | ✓      |
| [EasyPrivacy](https://easylist.to/easylist/easyprivacy.txt)                                                       | ✓      |
| [NoCoin](https://raw.githubusercontent.com/hoshsadiq/adblock-nocoin-list/master/nocoin.txt)                       | ✓      |
| [YouTube Ad Blocklist](https://raw.githubusercontent.com/Ewpratten/youtube_ad_blocklist/master/blocklist.txt)     | ✓      |
| [WindowsSpyBlocker](https://raw.githubusercontent.com/crazy-max/WindowsSpyBlocker/master/data/hosts/spy.txt)      | ✓      |
| [AdBlockID](https://raw.githubusercontent.com/realodix/AdBlockID/master/output/adblockid.txt)                     | ✓      |
| [bebasdns Custom Filtering Rules Blocklist](https://raw.githubusercontent.com/bebasid/bebasdns/main/custom-filtering-rules-blocklist) | ✓      |
| [Huawei Block List](https://raw.githubusercontent.com/deep-bhatt/huawei-block-list/master/huawei-block-host.txt)  | X      |
| [iOSAdblockList](https://raw.githubusercontent.com/BlackJack8/iOSAdblockList/master/Hosts.txt)                    | X      |
| [Energized](https://block.energized.pro/ultimate/formats/hosts)                                                   | X      |
| [Mahakala](https://adblock.mahakala.is/)                                                                          | X      |
| [Tiarapp](https://raw.githubusercontent.com/pengelana/blocklist/master/domain.txt)                                | X      |
| [blah](https://oooo.b-cdn.net/blahdns/lite_adblocker.txt)                                                         | X      |
| [Developerdan](https://www.github.developerdan.com/hosts/lists/ads-and-tracking-extended.txt)                     | X      |
| [1Hosts](https://raw.githubusercontent.com/badmojr/1Hosts/master/Lite/adblock.txt)                                | X      |
| [TheBlockListProject](https://blocklistproject.github.io/Lists/adguard/ads-ags.txt)                               | X      |

| Daftar Blokir (Custom)                                                                                            | Status |
|-------------------------------------------------------------------------------------------------------------------|--------|
| [LDM-Simple Tracking](https://s3.amazonaws.com/lists.disconnect.me/simple_tracking.txt )                          | X      |
| [LDM-Simple Ad](https://s3.amazonaws.com/lists.disconnect.me/simple_ad.txt)                                       | X      |
| [FireBog AdguardDNS](https://v.firebog.net/hosts/AdguardDNS.txt)                                                  | X      |
| [MinimalHostsBlocker](https://reddestdream.github.io/Projects/MinimalHosts/etc/MinimalHostsBlocker/minimalhosts)  | X      |
| [StevenBlack's KADHosts](https://raw.githubusercontent.com/StevenBlack/hosts/master/data/KADhosts/hosts)          | X      |
| [StevenBlack's AddSpam](https://raw.githubusercontent.com/StevenBlack/hosts/master/data/add.Spam/hosts)           | X      |
| [FireBog's W3KBL](https://v.firebog.net/hosts/static/w3kbl.txt)                                                   | X      |
| [anudeepND's Blacklist AdServers](https://raw.githubusercontent.com/anudeepND/blacklist/master/adservers.txt)     | X      |
| [FireBog's EasyPrivacy](https://v.firebog.net/hosts/Easyprivacy.txt)                                              | X      |
| [Perflyst's SmartTV](https://raw.githubusercontent.com/Perflyst/PiHoleBlocklist/master/SmartTV.txt)               | X      |
| [Simple Malvertising](https://s3.amazonaws.com/lists.disconnect.me/simple_malvertising.txt)                       | X      |
| [MalwareDomainList](https://www.malwaredomainlist.com/hostslist/hosts.txt)                                        | X      |
| [DBL Oisd](https://dbl.oisd.nl/)                                                                                  | X      |

# Daftar Putih DNS ― (23/08/2022)
| Daftar Putih                                                                                                                          | Status |
|---------------------------------------------------------------------------------------------------------------------------------------|--------|
| [bebasdns Custom Filtering Rules Whitelist](https://raw.githubusercontent.com/bebasid/bebasdns/main/custom-filtering-rules-whitelist) | ✓      |
| [bebasdns Whitelist](https://raw.githubusercontent.com/bebasid/bebasdns/main/whitelist.txt)                                           | ✓      |
| [Filterlist for AdGuard](https://raw.githubusercontent.com/hl2guide/Filterlist-for-AdGuard-or-PiHole/master/filter_whitelist.txt)     | ✓      |
| [AdGuard Home Whitelist](https://raw.githubusercontent.com/hg1978/AdGuard-Home-Whitelist/master/whitelist.txt)                        | ✓      |
| [AdGuard Home Filters](https://raw.githubusercontent.com/mmotti/adguard-home-filters/master/whitelist.txt)                            | ✓      |

# Server Upstream ― (02/01/2023)
| DNS Default                                                                                                                           | Status |
|---------------------------------------------------------------------------------------------------------------------------------------|--------|
| [Quad9 DNS11](https://dns11.quad9.net/dns-query)                                                                                      | ✓      |
| MyRepublic Uncensored (TCP)                                                                                                           | ✓      |
| [CloudFlare Security](https://security.cloudflare-dns.com/dns-query)                                                                  | X      |


| DNS OpenNIC                                                                                                                                          | Status |
|------------------------------------------------------------------------------------------------------------------------------------------------------|--------|
| glue, cyb, geek, free, indy, parody, bbs, null, oss, ing, dyn, gopher, micro, neo, pirate, oz, epic, o, chan, libre, fur, bazar, coin, emc, lib      | ✓      |


# Status Peladen

Statistik kondisi peladen:

• [Status UptimeRobot](https://stats.uptimerobot.com/j5MjytjV8y)

# Cara Mengaplikasian

Untuk cara mengaplikasian, silahkan ikuti panduan yang diberikan teman kami, pengelana.

• [Plain DNS](https://github.com/bebasid/bebasdns/blob/main/tutoraltport.md)

• [DNS-over-HTTPS](https://github.com/pengelana/blocklist/wiki/DNS-over-HTTPS-(DoH))

• [DNS-over-TLS](https://github.com/pengelana/blocklist/wiki/DNS-over-TLS-(DoT))

• [DNS-over-QUIC](https://github.com/pengelana/blocklist/wiki/DNS-over-QUIC-(DoQ))

# Uji Keamanan

bebasdns telah diuji keamanannya dan mendapatkan nilai pada website: 

• [ImmuniWeb](https://www.immuniweb.com/ssl/dns.bebasid.com/zZEVpm0y/) (A+) (Sep 7th, 2022).

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

Dengan menggunakan layanan ini, anda setuju mematuhi peraturan yang kami buat dan menerima segala akibat yang ditimbulkan. Untuk selengkapnya, lihat [ATURAN](https://github.com/bebasid/bebasid/blob/master/dev/readme/RULES.md) nya.
