**Latar Belakang**

        RADIUS (Remote Authentification  Dial In User Service ) adalah sebuah protokol keamanan komputer yang digunakan untuk melakukan autentikasi, otorisasi, dan pendaftaran akun pengguna secara terpusat untuk mengakses jaringan.

**Pembahasan**

        RADIUS (Remote Authentication Dial-In User Service) adalah sebuah protokol keamanan komputer yang digunakan untuk melakukan autentikasi, otorisasi, dan pendaftaran akun pengguna secara terpusat untuk mengakses jaringan. Radius diterapkan dalam jaringan dengan model client-server.

        RADIUS kini telah diimplementasikan untuk melakukan autentikasi terhadap akses jaringan secara jarak jauh dengan menggunakan koneksi selain dial-up, seperti halnya Virtual Private Networking (VPN), access point nirkabel, switch Ethernet, dan perangkat lainnya.

        RADIUS mula-mula dikembangkan oleh perusahan Livingston. Pada awal pengembangannya, RADIUS menggunakan port 1645, yang ternyata bentrok dengan layanan &quot;datametrics&quot;. Sekarang, port yang dipakai RADIUS adalah port 1812.

Beberapa karakteristik dari RADIUS adalah sebagai berikut:

1. Berbasis UDP Protocol
2. Bisa ditempatkan dimana saja di internet dan dapat membuat autentikasi (PPP, PAP, CHAP, MS-CHAP, EAP) antara Network Access Server (NAS) dan server itu sendiri
3. RADIUS menggunakan Remote Access Server (RAS) Secure ID untuk membuat autentikasi yang kuat dalam pengontrolan akses

**Kesimpulan**

        Server Radius menyediakan mekanisme keamanan dengan menangani otentikasi dan otorisasi koneksi yang dilakukan user. Pada saat komputer client akan menghubungkan diri dengan jaringan maka server Radius akan meminta identitas user (username dan password) untuk kemudian dicocokkan dengan data yang ada dalam database server Radius untuk kemudian ditentukan apakah user diijinkan untuk menggunakan layanan dalam jaringan komputer.