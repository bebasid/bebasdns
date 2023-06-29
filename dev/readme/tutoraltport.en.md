## Table of Content:

- [How to Use Alternative Port](#how-to-use-alternative-port)
  + [MikroTik](#mikrotik)
  + [GoodbyeDPI](#goodbyedpi)
  + [Pi-Hole](#pi-hole)
- [Check if BebasDNS / BebasID DNS configuration is running](#check-if-bebasdns--bebasid-dns-configuration-is-running)

---

# How To Use Alternative Port
If the ISP is using a Transparent DNS Proxy, it will not be able to use **bebasdns** via Do53 IPv4/6.<br>
Let's spoof, by using an alternative port so we can use **bebasdns**.

### MikroTik

Copy and paste this script to the terminal:


<b>CHOOSE ONE</b>

<b>Default DNS</b>


``` 
/ip firewall nat add action=dst-nat chain=dstnat comment="BebasID DNS" dst-port=53 protocol=tcp to-addresses=103.87.68.24 to-ports=1753
/ip firewall nat add action=dst-nat chain=dstnat comment="BebasID DNS" dst-port=53 protocol=udp to-addresses=103.87.68.24 to-ports=1753
```


```
/ipv6 firewall nat add action=dst-nat chain=dstnat comment="BebasID DNS" dst-port=53 protocol=tcp to-address=2a06:1287:1605:5353::beba:51d to-ports=1753
/ipv6 firewall nat add action=dst-nat chain=dstnat comment="BebasID DNS" dst-port=53 protocol=udp to-address=2a06:1287:1605:5353::beba:51d to-ports=1753
```
<b>Malware Blocking Only</b>

``` 
/ip firewall nat add action=dst-nat chain=dstnat comment="BebasID DNS" dst-port=53 protocol=tcp to-addresses=103.87.68.23 to-ports=1753
/ip firewall nat add action=dst-nat chain=dstnat comment="BebasID DNS" dst-port=53 protocol=udp to-addresses=103.87.68.23 to-ports=1753
```

```
/ipv6 firewall nat add action=dst-nat chain=dstnat comment="BebasID DNS" dst-port=53 protocol=tcp to-address=2001:df1:7340:c::beba:51d to-ports=1753
/ipv6 firewall nat add action=dst-nat chain=dstnat comment="BebasID DNS" dst-port=53 protocol=udp to-address=2001:df1:7340:c::beba:51d to-ports=1753
```

### GoodbyeDPI

**1. Choose ``2_any_country_dnsredir.cmd``, click Edit or open with __Notepad++__** *(If third-party program is available)*

![tutorialygy](https://media.discordapp.net/attachments/1059052464919298049/1107666667732992130/image.png)

**2. Add this part into ``start "" goodbyedpi.exe -5``**
<b><ins>CHOOSE ONE</ins>.</b></br></br>
<b>Default DNS:</b></br>
>  --dns-addr 103.87.68.24 --dns-port 1753 --dnsv6-addr 2a06:1287:1605:5353::beba:51d --dnsv6-port 1753

</br>

<b>Antivirus (Malware) Blocking Only</b>:</br>
>  --dns-addr 103.87.68.23 --dns-port 1753 --dnsv6-addr 2001:df1:7340:c::beba:51d --dnsv6-port 1753

</br>

![goodbyedpi](https://media.discordapp.net/attachments/1059052464919298049/1107664890761580574/image.png)

**3. Then, save ``2_any_country_dnsredir.cmd`` file.**

### Pi-Hole
**1. Add these lines to Custom DNS and enable them**

Custom 1 (IPv4): ``103.87.68.24#53`` or ``103.87.68.24#1753`` [For Default DNS]

Custom 2 (IPv4): ``103.87.68.23#1753`` or ``103.87.68.23#1753`` [For Antivirus (Malware) DNS]

![Pi-Hole](https://media.discordapp.net/attachments/1059052464919298049/1059052488428372030/image.png)

**2. If there is IPv6 support, add these lines to the (IPv6) section of Custom DNS and enable them (Optional choice or you can skip to step 3 if your ISP does not support IPv6).**

Custom 3 (IPv6): ``2a06:1287:1605:5353::beba:51d#53`` or ``2a06:1287:1605:5353::beba:51d#1753`` [For Default DNS]

Custom 4 (IPv6): ``2001:df1:7340:c::beba:51d#1753`` or ``2001:df1:7340:c::beba:51d#1753`` [For Antivirus (Malware) DNS]

**3. Then click save.**

### Check if BebasDNS / BebasID DNS configuration is running

**To make sure that the configuration is already running properly, open Command Prompt then type:**
```
nslookup lamanlabuh.aduankonten.id
```
![cek](https://media.discordapp.net/attachments/1059052464919298049/1107658636001542154/image.png)

If the result is either `0.0.0.0`, `127.0.0.1`, `::`, or `Server Failed`, **bebasdns** is already running and working properly.

---

<p align="center">Thank you for using <a href="#bebasdns--bebasid-dns">BebasDNS / BebasID DNS</a> service.</br> Enjoy your internet access freedom, forever!</br></br>Share our project!</br></br>
    <img src="https://github.com/bebasid/bebasdns/blob/main/dev/resources/logo/logo-black.png#gh-light-mode-only" alt="bebasDNS Black Logo" width="160">
    <img src="https://github.com/bebasid/bebasdns/blob/main/dev/resources/logo/logo.png#gh-dark-mode-only" alt="bebasDNS White Logo" width="160">
</p>
</br>
    </p>
  <p align="center">
    <a href="https://github.com/bebasid/bebasdns#readme">BebasDNS / BebasID DNS</a> is licensed under <a href="https://github.com/bebasid/bebasdns/blob/main/LICENSE">MPL-2.0</a>.
</p>
</div>
