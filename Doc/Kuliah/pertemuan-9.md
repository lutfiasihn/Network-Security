**Latar Belakang**

        Penggunaan internet saat ini merupakan suatu kebutuhan yang tidak dapat dihindari lagi. Dengan internet, segala sesuatunya akan menjadi lebih mudah. Keamanan Informasi merupakan salah satu kunci yang dapat mempengaruhi tingkat Reliability (termasuk performa dan availability) suatu jaringan. Untuk mengatasi masalah keamanan jaringan dan komputer ada banyak pendekatan yang dapat dilakukan. Salah satunya adalah dengan menggunakan sistem IDS (Intruction Detection System) dan IPS (Intrusion Prevention System).

**Pembahasan**

Instruction Detection System ( IDM )

IDS (Intrution Detection System) adalah sebuah sistem yang melakukan pengawasan terhadap lalulintas (traffic) jaringan dan pengawasan terhadap kegiatan-kegiatan yang mencurigakan didalam sebuah sistem jaringan. Jika ditemukan kegiatan-kegiatan yang mencurigakan berhubungan dengan lalulintas jaringan, maka IDS akan memberikan peringatan kepada sistem atau administrator jaringan. Ada 2 jenis IDS:

1. Network-based Intrusion Detection System (NIDS): Semua lalulintas yang mengalir ke sebuah jaringan akan dianalisis untuk mencari apakah ada percobaan serangan atau penyusupan ke dalam sistem jaringan. NIDS umumnya terletak di dalam segmen jaringan penting di mana server berada atau terdapat pada &quot;pintu masuk&quot; jaringan. Kelemahan NIDS adalah bahwa NIDS agak rumit diimplementasikan dalam sebuah jaringan yang menggunakan switch Ethernet, meskipun beberapa vendor switch Ethernet sekarang telah menerapkan fungsi IDS di dalam switch buatannya untuk memonitor port atau koneksi.
2. Host-based Intrusion Detection System (HIDS): Aktivitas sebuah host jaringan individual akan dipantau apakah terjadi sebuah percobaan serangan atau penyusupan ke dalamnya atau tidak. HIDS seringnya diletakkan pada server-server kritis di jaringan, seperti halnya firewall, web server, atau server yang terkoneksi ke Internet.

Cara Kerjanya.

Ada beberapa cara bagaimana IDS bekerja. Cara yang paling populer adalah dengan menggunakan pendeteksian berbasis signature (seperti halnya yang dilakukan oleh beberapa antivirus), yang melibatkan pencocokan lalu lintas jaringan dengan basis data yang berisi cara-cara serangan dan penyusupan yang sering dilakukan oleh penyerang. Sama seperti halnya antivirus, jenis ini membutuhkan pembaruan terhadap basis data signature IDS yang bersangkutan. Umumnya, dilakukan dengan menggunakan teknik statistik untuk membandingkan lalu lintas yang sedang dipantau dengan lalu lintas normal yang biasa terjadi. Metode ini menawarkan kelebihan dibandingkan signature-based IDS, yakni ia dapat mendeteksi bentuk serangan yang baru dan belum terdapat di dalam basis data signature IDS. Kelemahannya, adalah jenis ini sering mengeluarkan pesan false positive. Sehingga tugas administrator menjadi lebih rumit, dengan harus memilah-milah mana yang merupakan serangan yang sebenarnya dari banyaknya laporan false positive yang muncul.

Intruction Prevention System ( IPS )

Intrusion Prevention System (IPS) , adalah pendekatan yang sering digunakan untuk membangun system keamanan komputer, IPS mengkombinasikan teknik firewall dan metode IDS dengan baik. Teknologi ini dapat digunakan untuk mencegah serangan yang akan masuk ke jaringan lokal dengan memeriksa dan mencatat semua packet data serta mengenali paket data dengan sensor, disaat penyerangan telah teridentifikasi, IPS akan melakukan pemblokiran dan mencatat log semua paket data yang teridentifikasi tersebut.

Network-based Intrusion Prevention System (NIPS)

Network-based Intrusion Prevention System (NIPS) tidak melakukan pantauan secara khusus di satu host saja. Tetapi melakukan pantauan dan proteksi dalam satu jaringan secara global. NIPS menggabungkan fitur IPS dengan firewall dan kadang disebut sebagai In-Line IDS atau Gateway Intrusion Detection System (GIDS). Sistem kerja IPS yang populer yaitu pendeteksian berbasis signature, pendeteksian berbasis anomali, dan monitoring berkas-berkas pada sistem operasi host.

      Sistematika IPS yang berbasis signature adalah dengan cara mencocokkan lalu lintas jaringan dengan signature database milik IPS yang berisi attacking rule atau cara-cara serangan dan penyusupan yang sering dilakukan oleh penyerang. Sama halnya dengan antivirus, IPS berbasis signature membutuhkan update terhadap signature database untuk metode-metode penyerangan terbaru. IPS berbasis signature juga melakukan pencegahan terhadap ancaman intrusi sesuai dengan signature database yang bersangkutan. Teknik yang digunakan IPS untuk mencegah serangan ada dua, yaitu sniping dan shunning.

- Sniping: memungkinkan IPS untuk menterminasi serangan yang dicurigai melalui penggunaan paket TCP RST atau pesan ICMP Unreachable.
-   Shunning: memungkinkan IPS mengkonfigurasi secara otomatis firewall untuk drop traffic berdasar apa yang dideteksi oleh IPS. Untuk kemudian melakukan prevention terhadap koneksi tertentu.

      Perbedaan mendasar antara Intrusion Detection System (IDS) dan Intrusion Prevention System (IPS) dapat dilihat pada tabel berikut:

- Osi Layer

IDS Layer 3

IPS Layer 2, 3, dan 7

- Kegunaan

IDS di design hanya untuk mengidentifikasi dan meemriksa semua paket yang lewat, jika ditemukan keganjilan maka akan mentrigger alarm.

IPS mengkombinasikan firewall, policy, QoS dan IDS dengan baik, IPS memang dibuat untuk dapat mentrigger alarm dan melakukan allow, block , log.

- Aktivitas

IDS Mendeteksi serangan hanya disaat seragan tersebut telah masuk ke jaringan dan tidak akan melakukan sesuatu untuk menghentikannya.

IPS mencegah sedini mungkin attack masuk ke jaringan dan akan menghentikannya jika teridentifikasi.

- Komponen

IDS tidak dapat mendeteksi semua aktivitas malicious dan malware setiap saat yang akan mengakibatkan false negative yang sangat banyak.

IPS memungkinkan dapat mendeteksi new signature dan behavior attack dan mengakibatkan rendahnya false negative.

- Integrated

IDS tidak dapat menggunakan ACL / script dari komponen system keamanan yang lain.

IPS dapat diintegrasika dengan ACL dan perimeter DMZ lainnya.

?

**Kesimpulan**

        IDS ini bersifat pasif, artinya hanya mendeteksi intrusi dan membangkitkan alert saja tanpa disertai tindakan preventif. Untuk tindakan selanjutnya diserahkan kepada administrator apakah koneksi yang masuk tersebut harus diblokir atau tidak. IPS atau sistem pencegah intrusi merupakan IDS yang dikombinasikan dengan firewall. Jadi, apabila terdeteksi adanya serangan, IPS akan memerintahkan firewall untuk segera memblokir koneksi tersebut sebelum masuk ke jaringan. Dengan kata lain, IPS adalah IDS yang dilengkapi kemampuan firewall.