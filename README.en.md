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
    <b>For an ISP that uses DPI, use <a href="https://github.com/bebasid/bebasit">bebasit</a> to bypass the DPI or turn on IPv6 if the ISP supports it.</b>
    <br><sup>Signs that your ISP implemented DPI: HTTP redirected to<code><a href="http://lamanlabuh.aduankonten.id" target="_blank">lamanlabuh.aduankonten.id</a></code> or HTTPS responded with <code>ERR_CONNECTION_RESET</code>/<code>PR_CONNECT_RESET_ERROR</code></sup><br>
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
<p align="center">Donate us:</br>
<a href="https://trakteer.id/bebasidbykini"><img src="https://img.shields.io/static/v1?label=Trakteer&message=bebasidbykini&color=C02433"></a>
<a href="https://saweria.co/bebasid"><img src="https://img.shields.io/static/v1?label=Saweria&message=bebasid&color=FAAE2B"></a>
 </p>
<p align="center">
    <a href="README.md">Indonesia</a> | <b>English</b>
</p>

---

## Table of Content

- [bebasdns](#bebasdns)
  + [Server](#server)
    + [Alternative](#alternative)
      - [Malware](#malware)
   + [Filter](#filter)
      - [DNS Blocklist](#dns-blocklist)
      - [DNS Whitelist](#dns-whitelist)
  + [Maintenance](#maintenance)
    - [Server Status](#server-status)
    - [Security Test](#security-test) 
  + [List of Tutorials and Questions](#list-of-tutorials-and-questions)
    - [How to Use](#how-to-use)
    - [Contributing, Question and Request](#contributing-question-and-request)
    - [Frequently Asked Question](#frequently-asked-questions)
  + [Support Us](#donate-us)
  + [License](#license)
  + [Terms and Conditions](#terms-and-conditions)

---

# bebasdns

_Helping you surf securely and without limit!_

**bebasdns** implements a DNS resolver with an integrated ad-blocker that runs with moderately stable uptime on a VPS/VPN.

**bebasdns** disables the logging feature for user privacy because it is unimportant and consumes resources.

We only record queries if there is a bug report.
For example, if users can not access a website for troubleshooting purposes, and fixing that bug report.

## Server
| Protocol | Address | Port |
| -------- | ------- | :--: |
| DNS, IPv4 | ``103.87.68.24`` | ``53``, ``1753`` | 
| DNS, IPv6 | ``2a06:1287:1605:5353::beba:51d`` | ``53``,  ``1753`` |  
| DNS-over-HTTPS | ``https://dns.bebasid.com/dns-query`` | ``443`` |
| DNS-over-TLS | ``dns.bebasid.com`` | ``853`` |
| iOS | [dns.mobileconfig](https://raw.githubusercontent.com/bebasid/bebasdns/main/dev/resources/config/dns.mobileconfig) | |
| macOS | [dns-macos.mobileconfig](https://raw.githubusercontent.com/bebasid/bebasdns/main/dev/resources/config/dns-macos.mobileconfig) | |

|  DNSCrypt Protocol   |                                         Address                                            |
|----------------------|--------------------------------------------------------------------------------------------|
| DNSCrypt Stamp | ``sdns://AgMAAAAAAAAADDEwMy44Ny42OC4yNAAPZG5zLmJlYmFzaWQuY29tCi9kbnMtcXVlcnk`` |      


# Alternative

### <ins>Malware</ins> 
Specialized for malware blocking and without adblocking.

| Protocol | Address | Port |
| -------- | ------- | :--: |
| DNS, IPv4 | ``103.87.68.23`` | ``53``, ``1753`` | 
| DNS, IPv6 | ``2001:df1:7340:c::beba:51d`` | ``53``,  ``1753`` |
| DNS-over-HTTPS | ``https://antivirus.bebasid.com/dns-query`` | ``443`` |
| DNS-over-TLS | ``antivirus.bebasid.com`` | ``853`` |

|  DNSCrypt Protocol   |                                         Address                                            |
|----------------------|--------------------------------------------------------------------------------------------|
| DNSCrypt Stamp | ``sdns://AgMAAAAAAAAADDEwMy44Ny42OC4yMwAVYW50aXZpcnVzLmJlYmFzaWQuY29tCi9kbnMtcXVlcnk`` |   

## Filter

A filter is a mechanism for blocking access to certain content on the Internet. When going to a website, the browser sends the website name (for example, <code>google.com</code>) to a DNS server. The DNS server answers with the IP address of the server hosting this website.</br>

DNS Blocklists are used to block domains known to serve ads or trackers.</br>
DNS Whitelists are used to allow domains that blocklists would otherwise block.

### <ins>DNS Blocklist</ins>
| Blocklist                                                                                                         |
|-------------------------------------------------------------------------------------------------------------------|
| [bebasdns's Custom Filtering Blocklist Rules](https://raw.githubusercontent.com/bebasid/bebasdns/main/dev/resources/hosts/custom-filtering-rules-blocklist) | 
| [OISD Blocklist Full](https://raw.githubusercontent.com/deep-bhatt/huawei-block-list/master/huawei-block-host.txt)      | 
| [WindowsSpyBlocker](https://raw.githubusercontent.com/BlackJack8/iOSAdblockList/master/Hosts.txt)                       |
| [URLHaus's Maliclious](https://raw.githubusercontent.com/BlackJack8/iOSAdblockList/master/Hosts.txt)                    | 

### <ins>DNS Whitelist</ins>
| Whitelist                                                                                                                             |
|---------------------------------------------------------------------------------------------------------------------------------------|
| [bebasdns's Custom Filtering Wihtelist Rules](https://raw.githubusercontent.com/bebasid/bebasdns/main/dev/resources/hosts/custom-filtering-rules-whitelist) | 
| [bebasdns's Custom Filtering Whitelist Rules 2](https://raw.githubusercontent.com/bebasid/bebasdns/main/dev/resources/hosts/whitelist.txt) | 

## Maintenance

### <ins>Server Status</ins>

Public service status statistic:

• [UptimeRobot](https://stats.uptimerobot.com/j5MjytjV8y)

### <ins>Security Test</ins>

bebasdns has been tested for security and graded according to website:

• [ImmuniWeb](https://www.immuniweb.com/ssl/dns.bebasid.com/M07B3FiY/) (A+) (May 14th, 2023).

## List of Tutorials and Questions

### <ins>How to Use</ins>

Please follow the tutorial below:

• [Plain DNS (Alternative Port)](https://github.com/bebasid/bebasdns/blob/main/dev/readme/tutoraltport.en.md#how-to-use-alternative-port)

• [DNS-over-HTTPS](https://github.com/pengelana/blocklist/wiki/DNS-over-HTTPS-(DoH))

• [DNS-over-TLS](https://github.com/pengelana/blocklist/wiki/DNS-over-TLS-(DoT))

• [Pi-Hole](https://github.com/bebasid/bebasdns/blob/main/dev/readme/tutoraltport.md#pi-hole)

• [DNSCrypt](https://libreddit.eu.org/r/indonesia/comments/kyyxna/comment/gjjq578/)

• [GoodbyeDPI](https://github.com/bebasid/bebasdns/blob/main/dev/readme/tutoraltport.md#goodbyedpi)

• [MikroTik](https://github.com/bebasid/bebasdns/blob/main/dev/readme/tutoraltport.md#mikrotik)

• [iOS](https://libreddit.eu.org/r/indonesia/comments/kyyxna/comment/gjke3u7)/[macOS](https://translate.google.com/translate?hl=id&sl=en&u=https://simpledns.plus/kb/201/how-to-enable-dns-over-tls-dot-dns-over-https-doh-in-macos-v11&prev=search&pto=aue)

### <ins>Contributing, Question and Request</ins>

If you have any requests or bug reports, please [open a new issue](https://github.com/bebasid/bebasid/issues/new/choose).

### <ins>Frequently Asked Questions</ins>

If you have any problems using bebasdns, please head to [Discord](https://discord.gg/EKrxZyu).

Or you can email `dukungan@bebasid.com` with the subject **BebasDNS: [Your problem/question]**

## Donate us

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

bebasdns is licensed under [MPL-2.0 License](https://github.com/bebasid/bebasdns/blob/main/LICENSE).

---

# Terms and Conditions


By using this service, you are deemed to have read, understood, and agreed to all the rules that we have made and you accept all the consequences that will arise. If you do not agree to accept the existing rules, then you are not allowed to use this service. For more information about the rules, you can see them on the page [RULES](https://github.com/bebasid/bebasdns/blob/master/dev/readme/RULES.md).
