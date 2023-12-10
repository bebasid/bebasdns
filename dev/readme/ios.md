<p align="center">
  <img src="https://developer.apple.com/assets/elements/icons/ios-17-num/ios-17-num-96x96_2x.png" width="320px"><br>
</p>

<h2 align="center">Tutorial Pemasangan BebasDNS/BebasID DNS di Apple iOS</h2>

### Langkah-langkah:
-  [Membuat Profile DoH/DoT dns.mobileconfog di Apple iOS](#Membuat-Profile-DoH-DoT-dns.mobileconfog-di-Apple-iOS)

## Membuat Profile DoH/DoT dns.mobileconfog di Apple iOS
1. Buka Web di bawah ini. (Wajib memakai browser Safari!)
> https://dns.notjakob.com/tool.html

2. Isi-kan dibagian **"MyCoolSecureProvider"** dengan BebasDNS/BebasID DNS.

3. Pilih Protokol **DNS-Over-HTTPS** atau **DNS-Over-TLS** _(yang anda gunakan)_.

4. Langsung scroll paling bawah, isi-kan di bagian **DoT/DoH Server URL** dengan URL yang sudah sedia dari dokumentasi GitHub.
   > Contoh: ``dns.bebasid.com``
   untuk <ins>DoH/DoT</ins>.

5. Klik **"Download Profile"**.

6. Setelah di download, klik file <b><ins>DNS DoH/DoT</ins></b>-nya dari Download Manager Safari, klik <b>"lihat gambar"</b> / <b>"kaca pembesar"</b> supaya langsung diarahkan ke <ins>Files</ins>.

7. Klik file **"DNS"** _(Umumnya nama filenya otomastis **dns** atau **dns1** disitu)_.

8. Sesudah di-klik, akan muncul notifikasi **"Profile Downloaded"**, review profil-nya di Aplikasi **"Pengaturan"**, dkk.

9. Buka ``Settings > General > Profile``, langsung klik **"Profile DNS"** yang sudah di download tadi.

10. Klik **"Install"** di pojok kanan atas. 

Voila! 
Sudah langsung terhubung dan bisa di cek ke website [dnsleaktest.com](https://dnsleaktest.com), pilih standar test dan hasil-nya akan muncul server DNS **"ID-ATHARVA-MINT"**.
