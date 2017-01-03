**Latar Belakang**

        Snort merupakan salah satu aplikasi Linux yang dapat dipakai untuk meningkatkan keamanan computer. Snort bekerja seperti Wireshark, yaitu dapat menyimpan setiap paket yang di ambil kedalam media penyimpanan di modus packet logger mode.

**Pembahasan**

        Snort yaitu sebuah software ringkas yang sangat berguna untuk mengamati aktvitas dalam suatu jaringan computer. Snort dapat digunakan sebagai suatu Network Intrusion Detection System (NIDS) yang berskala ringan. Cara kerja snort hampir sama seperti wireshark, hanya saja snort dapat dipakai sebagai komponen NIDS dengan menjalankannya pada NIDS mode. Pada modus yag terakhir ini, snort akan menganalisa paket berdasarkan rule yang ada untuk mengenali adanya upaya serangan hacker.

Snort memiliki 3 mode pengoperasian yaitu:

1. Sniffer Mode ( dapat melihat paket yang lewat dalam jaringan computer dimana snort diletakan)
2. Packet Logger Mode ( dalam mode ini, selain melihat semua paket yang lewat dalam jaringan computer, snort juga dapat mencatat atau melakukan logging terhadap berbagai paket tersebut ke disk).
3. Network Intrusion Detection Mode (snort bertindak sebagai NIDS yang dapat mendeteksi dan melakukan logging tehadap macam serangan jaringan computer berdasarkan rule ssistem yang ditetapkan oleh pegguna snort).

        Sebelum instalasi, dipastikan bahwa pengguna telah login ke Win 2000 sebagai administrator jika tidak, maka instalasi tidak akan selesai karena user privilege 2. Untuk install snort pada CentOS, pertama buatlah folder download sementara untuk direktori home dan ketiklah perintah ini:

_mkdir -/snort\_src_

_cd -/snort\_src_

download paket terbaru DAQ dari website snort dan gantilah versi jika ada sumber yang lebih baru.

_wget_ [_https://www.snort.org/downloads/snort/daq-2.0.6.tar.gz_](https://www.snort.org/downloads/snort/daq-2.0.6.tar.gz)

setelah selesai download, ekstrak lah dan masukan perintsh berikut

_tar-xvzf daq-2.0.6.tar.gz_

_cd daq-2.0.6_

jalankan script dan gunakan untuk compile program dan akhirnya terpasang DAQ

_./configure_

_Make_

_Sudo make install_

Dengan DAQ yang sudah di install, snort sudah bisa digunakan

_cd-/snort\_src_

untuk mengganti kode snort terbaru dan menggantinya dapat menggunakan perintah berikut ini:

_wget_ [_https://www.snort.org/downloads/snort/snort-2.9.8.o.tar.gz_](https://www.snort.org/downloads/snort/snort-2.9.8.o.tar.gz)

setelah selesai, ekstrak dan ubah kedalam direktori baru:

_tar –xvzf snort-2.98o.tar.gz_

_cd snort-2.9.8.0_

konfigurasi instalasi dengan modus Sourcefire diaktifkan.

_./configure –enable-sourcefire_

_Make_

_Sudo make install_

**Penutup**

Snort merupakan aplikasi open source yang ringan dan menyediakan fitur-fitur gratis yang fleksibel dan menguntungkan bagi banyak user

**Saran**

Agar belajar lebih mendalam untuk mengetahui atau memperdalam ilmu keamanan jaringan computer.