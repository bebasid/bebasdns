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


