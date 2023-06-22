<p align="center">
  <img src="https://www.pngitem.com/pimgs/m/10-107139_confused-anime-girl-png-transparent-png.png" width="250px"><br>
  <i>Saya kok mau akses situs R**dit atau V*meo gak bisa walau pake BebasDNS / File Host BebasID?</i><br><br>
  <b>Itu dikarenakan provider internet anda menggunakan teknologi DPI untuk memaksa pemblokiran sehingga mengganti DNS atau pake file host tidak cukup.</b><br><br>
  <i>Apa itu DPI?</i><br><br>
  <b>Yok! Kita cari tahu!</b>
</p>

## Apa itu DPI?
<p align="center">
  <img src="https://media.discordapp.net/attachments/1117725697646014484/1121259982776717383/cLXczluYcjR4kkGH93X4.png?width=1080&height=222">
</p>
DPI adalah singkatan dari <b>Deep Packet Inspection</b> yang merupakan metode pengawasan dan analisis lalu lintas internet yang memeriksa paket data yang dikirim melalui jaringan komputer. DPI menganalisis konten dan informasi dalam paket data, termasuk header dan payload, untuk mengidentifikasi jenis aplikasi, protokol, atau layanan yang digunakan.

**Masih gak ngerti?**

Bayangkan jika jaringan komputer adalah jalan tol dan paket data adalah mobil yang mengantri untuk membayar di gerbang. Di tol pasti ada gerbang buat bayar kan? Gerbang itu adalah Firewall DPI dikarenakan disitu lah titik akhir mobil di tol sebelum keluar tol / kerute selanjutnya.

Dikarenakan mengantri inilah mengapa laju mobil menjadi lambat (Ini bisa dianalogikan kenapa internet kita tambah lambat terutama pada jam sibuk. Dikarenakan Firewall DPI yang ada di sisi provider harus membaca miliyaran trafik yang lewat sebelum dapat dikoneksikan sehingga menjadi delay alias macet)

Setiap mobil (Trafik yang anda coba kirim melalui ISP anda) harus membuktikan kalau mereka adalah pengendara yang sah di Jalan Tol tersebut dengan cara membayar (Dalam kasus ini, 'pengendara yang sah' adalah situs yang diperbolehkan untuk diakses sedangkan 'cara membayar' adalah perumpamaan dari trafik-trafik yang kita lewatkan di sisi provider yang harus memberi identifikasi kepada sang provider sebelum mereka bisa lewat)

## Apa Dampak dari ISP menggunakan DPI

DPI dapat membuat koneksi internet menjadi lambat dan mengganggu privasi pengguna dengan beberapa cara:
1. Penghentian dan pemeriksaan paket: DPI dapat memeriksa setiap paket yang dikirim melalui jaringan, yang membutuhkan waktu dan sumber daya yang signifikan. Hal ini dapat mengakibatkan penundaan (latency) dalam pengiriman paket, yang menyebabkan koneksi internet terasa lambat.
2. Filtering dan pemblokiran: DPI dapat digunakan untuk menerapkan kebijakan keamanan dan pembatasan akses. Ini berarti penyedia layanan internet (ISP), pemerintah, atau entitas lain yang mengimplementasikan DPI dapat memblokir atau membatasi akses ke situs web, aplikasi, atau layanan tertentu. Ini dapat mengurangi kecepatan dan membatasi akses internet pengguna, mempengaruhi privasi mereka dan mengganggu kebebasan internet.
3. Pemantauan privasi: Dengan menganalisis konten dalam paket data, DPI dapat mengumpulkan informasi pribadi pengguna, seperti detail browsing, aktivitas online, dan komunikasi pribadi. Jika tidak diatur dengan benar, praktik ini dapat melanggar privasi pengguna dan mengancam keamanan data mereka.

Dalam beberapa negara, pemerintah atau ISP menerapkan DPI sebagai bagian dari program pengawasan yang lebih luas untuk memantau atau mengendalikan lalu lintas internet. Namun, penggunaan DPI yang tidak terkelola dengan baik atau tanpa persetujuan pengguna yang jelas dapat mengakibatkan masalah privasi dan pembatasan kebebasan pengguna dalam mengakses dan menggunakan internet.

## Bagaimana DPI Nasional di Indonesia bekerja?

Cara Great Firewall of Indonesia bekerja adalah dengan mengirimkan paket RST ke client (dan terkadang servernya juga) jika mendeteksi user mengunjungi situs yang diblokir dengan melihat headernya. Ini mengapa mengganti DNS atau sebagainya tidak akan bekerja jika ISP anda memakai DPI untuk memblokir situs.

Header yang ditargetkan untuk memblokir website oleh DPI ialah
- Host header<br>
  Host header merupakan identifikasi pada header http yang mengandung informasi situs yang akan kita kunjungi dan dikirimkan tanpa enkripsi sehingga Great Firewall of Indonesia bisa membacanya, menyamar menjadi server tujuan, dan membelokan request ke `http://lamanlabuh.aduankonten.id` dikarenakan situs http tidak mempunyai pengecekan seperti https dengan certificate<br>
  
  ![image](https://github.com/bebasid/KominFudge/assets/115700386/848147a7-a296-4686-a83e-52a844aeaeaf)<br>
 
 - SNI (Server Name Indication)<br>
   SNI (Server Name Indication) merupakan identifikasi pada header https yang mengandung informasi situs yang kita kunjungi dan biasa dikirimkan dengan bentuk plaintext sehingga bisa dibaca. Dikarenakan https bersifat terenkripsi dan aman, maka untuk memblokir situs https hanya bisa mengirimkan paket RST agar tidak bisa diakses karena semua data yang lewat terenkripsi dengan sertifikat SSL
   
   ![image](https://github.com/bebasid/KominFudge/assets/115700386/1e774621-2495-4434-860c-6a3d747d47e0)<br>
   ![image](https://github.com/bebasid/KominFudge/assets/115700386/f0c4c87d-e172-44f6-8102-d3996b3e3669)<br>
