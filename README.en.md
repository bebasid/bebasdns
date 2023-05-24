<p align="center">
    <b>For ISP that uses DPI, use <a href="https://github.com/bebasid/bebasit">bebasit</a> to bypass the DPI or turn on IPv6 if the ISP supports it.</b>
    <br><sup>Signs if your ISP implemented DPI: HTTP redirected to<code><a href="http://lamanlabuh.aduankonten.id" target="_blank">lamanlabuh.aduankonten.id</a></code> or HTTPS responded with <code>ERR_CONNECTION_RESET</code>/<code>PR_CONNECT_RESET_ERROR</code></sup><br>
    <b>Bypass DPI on Modem/Router:</b><br>
    <a href="https://github.com/bebasid/bebasit/blob/master/docs/openwrt-tutorial.en.md">OpenWRT</a> |
    <a href="https://github.com/bebasid/bebasit/blob/master/docs/mikrotik-tutorial.en.md">MikroTik</a>
</p>
<p align="center">
    <img src="https://github.com/bebasid/bebasdns/blob/main/dev/resources/logo/logo-black.png#gh-light-mode-only" alt="bebasDNS Black Logo" width="330">
    <img src="https://github.com/bebasid/bebasdns/blob/main/dev/resources/logo/logo.png#gh-dark-mode-only" alt="bebasDNS White Logo" width="330">
</p>
<p align="center">
<a href="https://discord.gg/EKrxZyu"><img src="https://discordapp.com/api/guilds/630415907021389825/widget.png?style=banner2" alt="Join BEBASID Discord"></a>
 </p>
<p align="center">
<a href="#"><img src="https://img.shields.io/static/v1?label=year%20released:&message=2020&color=yellowgreen&style=plastic%22"></a>
 <a href="https://ready.chair6.net/?url=dns.bebasid.com"><img src="https://img.shields.io/badge/ipv6-ready-blue"></a>
  <a href="https://stats.uptimerobot.com/j5MjytjV8y"><img src="https://img.shields.io/badge/status-up-brightgreen"></a>
 <a href='https://www.immuniweb.com/ssl/dns.bebasid.com/M07B3FiY'><img src="https://img.shields.io/badge/imuniweb-A%2B-brightgreen"></a>
<a href="#"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fbebasid%2Fbebasdns_fGHyh&count_bg=%234572CD&title_bg=%23555555&icon_color=%23E7E7E7&title=watchers%3A+%28today%2Ftotal%29&edge_flat=false"/></a>
<a href="https://github.com/bebasid/bebasdns/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-green"></a>
</p>
<p align="center">
    <a href="README.md">Indonesia</a> | <b>English</b>
</p>

---

## Table of Content

* [bebasdns](#bebasdns)
  + [Server](#server)
  + [Alternative Servers](#altervative-servers)
    - [Unfiltered](#unfiltered)
    - [Malware](#malware)
    - [Family](#family)
  + [DNS Blocklist](#dns-blocklist)
  + [DNS Whitelist](#dns-whitelist)
  + [Upstream DNS Server](#upstream-dns-server)
  + [Server Status](#server-status)
  + [Security Test](#security-test)
  + [How to Use](#how-to-use)
  + [Contributing, Question and Request](#contributing-question-and-request)
  + [Frequently Asked Question](#frequently-asked-question)
  + [Support Us!](#donate-us)
  + [License](#license)
  + [Terms and Conditions](#terms-and-conditions)

---

# bebasdns

_Helping you surf securely and without limit!_

**bebasdns** implements a DNS resolver and integrated ad-blocker that runs with moderately stable uptime on a VPS/VPN and does not record queries.

**bebasdns** also supports top-level domain from [OpenNIC](https://www.opennic.org/), so you can enjoy a more liberating website access experience.
**bebasdns** disabling logging feature for user privacy, also it is not important, and because it consumes resources. 

We only record queries if there is a bug report.
For example, if users can not access a website for troubleshooting purposes, and fixing that bug report.

# Server
| Protocol | Address | Port |
| -------- | ------- | :--: |
| DNS, IPv4 | ``147.139.211.126`` (CGK),  ``47.254.192.66`` (KUL) | ``53``, ``1753`` | 
| DNS, IPv6 | ``2001:470:36:9be:ba5::1d`` (CGK),  ``2001:470:36:b90:beba:5::1d`` (KUL) | ``53``,  ``1753`` |  
| DNS-over-HTTPS | ``https://dns.bebasid.com/dns-query/`` | |
| DNS-over-TLS | ``dns.bebasid.com`` | |
| DNS-over-QUIC | ``quic://dns.bebasid.com`` |
| iOS | [dns.mobileconfig](https://raw.githubusercontent.com/bebasid/bebasdns/main/dev/resources/config/dns.mobileconfig) | |
| macOS | [dns-macos.mobileconfig](https://raw.githubusercontent.com/bebasid/bebasdns/main/dev/resources/config/dns-macos.mobileconfig) | |

|  DNSCrypt Protocol   |                                         Address                                            |
|----------------------|--------------------------------------------------------------------------------------------|
| IPv4, DNS-over-HTTPS | ``sdns://AgcAAAAAAAAADzE0Ny4xMzkuMjExLjEyNgAPZG5zLmJlYmFzaWQuY29tCi9kbnMtcXVlcnk`` (CGK), ``sdns://AgcAAAAAAAAADTQ3LjI1NC4xOTIuNjYAD2Rucy5iZWJhc2lkLmNvbQovZG5zLXF1ZXJ5`` (KUL) |           
| IPv6, DNS-over-HTTPS | ``sdns://AgcAAAAAAAAAGVsyMDAxOjQ3MDozNjo5YmU6YmE1OjoxZF0AD2Rucy5iZWJhc2lkLmNvbQovZG5zLXF1ZXJ5`` (SIN), ``sdns://AgcAAAAAAAAAHFsyMDAxOjQ3MDozNjpiOTA6YmViYTo1OjoxZF0AD2Rucy5iZWJhc2lkLmNvbQovZG5zLXF1ZXJ5`` (KUL) | 



# Alternative Servers

### Unfiltered 
Without adblocking, malware blocking, and adult content blocking.

| Protocol | Address |
|----------|---------|
| DNS-over-HTTPS | ``https://dns.bebasid.com/dns-query/unfiltered/`` | 
| DNS-over-TLS   | ``unfiltered.dns.bebasid.com`` |
| DNS-over-QUIC  | ``quic://unfiltered.dns.bebasid.com`` | 

|  DNSCrypt Protocol   |                                         Address                                                                |
|----------------------|----------------------------------------------------------------------------------------------------------------|
|IPv4, DNS-over-HTTPS  | ``sdns://AgcAAAAAAAAADzE0Ny4xMzkuMjExLjEyNgAPZG5zLmJlYmFzaWQuY29tFS9kbnMtcXVlcnkvdW5maWx0ZXJlZA`` (CGK)        |
|IPv6, DNS-over-HTTPS  | ``sdns://AgcAAAAAAAAAGVsyMDAxOjQ3MDozNjo5YmU6YmE1OjoxZF0AD2Rucy5iZWJhc2lkLmNvbRUvZG5zLXF1ZXJ5L3VuZmlsdGVyZWQ`` (CGK) |

### Malware 
Specialized for malware blocking and without adblocking.

| Protocol       |                                         Address                                            |
|----------------|--------------------------------------------------------------------------------------------| 
| DNS-over-HTTPS | ``https://dns.bebasid.com/dns-query/malware/``                                             | 
| DNS-over-TLS   | ``malware.dns.bebasid.com``                                                                |
| DNS-over-QUIC  | ``quic://malware.dns.bebasid.com``                                                         | 

|  DNSCrypt Protocol   |                                                  Address                                                    |
|----------------------|-------------------------------------------------------------------------------------------------------------|
|IPv4, DNS-over-HTTPS  | ``sdns://AgcAAAAAAAAADzE0Ny4xMzkuMjExLjEyNgAPZG5zLmJlYmFzaWQuY29tEi9kbnMtcXVlcnkvbWFsd2FyZQ`` (CGK)         |
|IPv6, DNS-over-HTTPS  | ``sdns://AgcAAAAAAAAAGVsyMDAxOjQ3MDozNjo5YmU6YmE1OjoxZF0AD2Rucy5iZWJhc2lkLmNvbRIvZG5zLXF1ZXJ5L21hbHdhcmU`` (CGK)  |

### Family
Specialized for malware blocking, adult content blocking and without adblocking.

| Protocol       |                                         Address                                            |
|----------------|--------------------------------------------------------------------------------------------|
| DNS-over-HTTPS | ``https://dns.bebasid.com/dns-query/family/``                                              | 
| DNS-over-TLS   | ``family.dns.bebasid.com``                                                                 |
| DNS-over-QUIC  | ``quic://family.dns.bebasid.com``                                                          | 

|  DNSCrypt Protocol   |                                                Address                                                    |
|----------------------|-----------------------------------------------------------------------------------------------------------|
|IPv4, DNS-over-HTTPS  | ``sdns://AgcAAAAAAAAADzE0Ny4xMzkuMjExLjEyNgAPZG5zLmJlYmFzaWQuY29tES9kbnMtcXVlcnkvZmFtaWx5`` (CGK)         |
|IPv6, DNS-over-HTTPS  | ``sdns://AgcAAAAAAAAAGVsyMDAxOjQ3MDozNjo5YmU6YmE1OjoxZF0AD2Rucy5iZWJhc2lkLmNvbREvZG5zLXF1ZXJ5L2ZhbWlseQ`` (CGK) |

# DNS Blocklist
| Blocklist                                                                                                         |
|-------------------------------------------------------------------------------------------------------------------|
| [AdGuard](https://adguardteam.github.io/AdGuardSDNSFilter/Filters/filter.txt)                                     | 
| [NoTracking](https://raw.githubusercontent.com/notracking/hosts-blocklists/master/adblock/adblock.txt)            | 
| [ABPIndo](https://raw.githubusercontent.com/ABPindo/indonesianadblockrules/master/subscriptions/abpindo.txt)      | 
| [uBlock Origin](https://raw.githubusercontent.com/uBlockOrigin/uAssets/master/filters/filters.txt)                | 
| [uBlock Origin Filters](https://raw.githubusercontent.com/LanikSJ/ubo-filters/main/filters/combined-filters.txt)  | 
| [EasyList](https://easylist.to/easylist/easylist.txt)                                                             | 
| [AdAway](https://adaway.org/hosts.txt)                                                                            | 
| [MVPS](https://winhelp2002.mvps.org/hosts.txt)                                                                    | 
| [ABP Oisd](https://abp.oisd.nl/)                                                                                  | 
| [Cameleon](https://sysctl.org/cameleon/hosts)                                                                     | 
| [Adblock Plus](https://easylist-downloads.adblockplus.org/abp-filters-anti-cv.txt)                                | 
| [URLhaus](https://malware-filter.gitlab.io/malware-filter/urlhaus-filter-agh.txt)                                 | 
| [EasyPrivacy](https://easylist.to/easylist/easyprivacy.txt)                                                       | 
| [NoCoin](https://raw.githubusercontent.com/hoshsadiq/adblock-nocoin-list/master/nocoin.txt)                       | 
| [YouTube Ad Blocklist](https://raw.githubusercontent.com/Ewpratten/youtube_ad_blocklist/master/blocklist.txt)     | 
| [WindowsSpyBlocker](https://raw.githubusercontent.com/crazy-max/WindowsSpyBlocker/master/data/hosts/spy.txt)      |
| [bebasdns's Custom Filtering Blocklist Rules](https://raw.githubusercontent.com/bebasid/bebasdns/main/dev/resources/hosts/custom-filtering-rules-blocklist) | 
| [OISD Blocklist Full](https://raw.githubusercontent.com/deep-bhatt/huawei-block-list/master/huawei-block-host.txt)      | 
| [WindowsSpyBlocker](https://raw.githubusercontent.com/BlackJack8/iOSAdblockList/master/Hosts.txt)                       |
| [URLHaus's Maliclious](https://raw.githubusercontent.com/BlackJack8/iOSAdblockList/master/Hosts.txt)                    | 

# DNS Whitelist
| Whitelist                                                                                                                             |
|---------------------------------------------------------------------------------------------------------------------------------------|
| [bebasdns's Custom Filtering Wihtelist Rules](https://raw.githubusercontent.com/bebasid/bebasdns/main/dev/resources/hosts/custom-filtering-rules-whitelist) | 
| [bebasdns's Custom Filtering Whitelist Rules 2](https://raw.githubusercontent.com/bebasid/bebasdns/main/dev/resources/hosts/whitelist.txt) | 
| [Filterlist for AdGuard](https://raw.githubusercontent.com/hl2guide/Filterlist-for-AdGuard-or-PiHole/master/filter_whitelist.txt)     | 
| [AdGuard Home Whitelist](https://raw.githubusercontent.com/hg1978/AdGuard-Home-Whitelist/master/whitelist.txt)                        | 
| [AdGuard Home Filters](https://raw.githubusercontent.com/mmotti/adguard-home-filters/master/whitelist.txt)                            | 

# Upstream DNS Server
| Default                                                                                                                               |
|---------------------------------------------------------------------------------------------------------------------------------------|
| [Cloudflare](https://www.cloudflare.com)                                                                                              | 

| [OpenNIC](https://www.opennic.org/)                                                                                                                  |
|------------------------------------------------------------------------------------------------------------------------------------------------------|
| glue, cyb, geek, free, indy, parody, bbs, null, oss, ing, dyn, gopher, micro, neo, pirate, oz, epic, o, chan, libre, fur, bazar, coin, emc, lib      |


# Server Status

Public service status statistic:

• [UptimeRobot](https://stats.uptimerobot.com/j5MjytjV8y)

# Security Test

bebasdns has been tested for security and graded according to website:

• [ImmuniWeb](https://www.immuniweb.com/ssl/dns.bebasid.com/M07B3FiY/) (A+) (May 14th, 2023).

# How to Use

Please follow the tutorial below:

• [Plain DNS (Alternative Port)](https://github.com/bebasid/bebasdns/blob/main/dev/readme/tutoraltport.md#cara-memakai-port-alternatif)

• [DNS-over-HTTPS](https://github.com/pengelana/blocklist/wiki/DNS-over-HTTPS-(DoH))

• [DNS-over-TLS](https://github.com/pengelana/blocklist/wiki/DNS-over-TLS-(DoT))

• [DNS-over-QUIC](https://github.com/pengelana/blocklist/wiki/DNS-over-QUIC-(DoQ))

• [Pi-Hole](https://github.com/bebasid/bebasdns/blob/main/dev/readme/tutoraltport.md#pi-hole)

• [DNSCrypt](https://libreddit.eu.org/r/indonesia/comments/kyyxna/comment/gjjq578/)

• [GoodbyeDPI](https://github.com/bebasid/bebasdns/blob/main/dev/readme/tutoraltport.md#goodbyedpi)

• [MikroTik](https://github.com/bebasid/bebasdns/blob/main/dev/readme/tutoraltport.md#mikrotik)

• [iOS](https://libreddit.eu.org/r/indonesia/comments/kyyxna/comment/gjke3u7)/[macOS](https://translate.google.com/translate?hl=id&sl=en&u=https://simpledns.plus/kb/201/how-to-enable-dns-over-tls-dot-dns-over-https-doh-in-macos-v11&prev=search&pto=aue)

# Contributing, Question and Request

If you have any request or bug report, please [open a new issue](https://github.com/bebasid/bebasid/issues/new/choose).

# Frequently Asked Question

If you have any problems using bebasdns, please head to [Discord](https://discord.gg/EKrxZyu).

Or you can email `dukungan@bebasid.com` with the subject **BebasDNS: [Your problem/question]**

# Support Us!

Help us maintain this project by donating.

<div>
<details>
 <summary>:coffee: Buy us a coffee</summary>

</br>

<a href="https://trakteer.id/bebasidbykini"><img src="https://img.shields.io/static/v1?label=Trakteer&message=bebasidbykini&color=C02433"></a>

<a href="https://saweria.co/bebasid"><img src="https://img.shields.io/static/v1?label=Saweria&message=bebasid&color=FAAE2B"></a>

</details>
</div>

## License

bebasdns is licensed under [MIT License](https://github.com/bebasid/bebasdns/blob/main/LICENSE).

---

# Terms and Conditions


By using this service, you are deemed to have read, understood, and agreed to all the rules that we have made and you accept all the consequences that will arise. If you do not agree to accept the existing rules, then you are not allowed to use this service. For more information about the rules, you can see them on the page. [RULES](https://github.com/bebasid/bebasdns/blob/master/dev/readme/RULES.md).
