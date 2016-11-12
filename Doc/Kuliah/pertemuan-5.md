1. Latar Belakang

IP spoofing adalah salah satu tekhnik yang banyak digunakan di internet untuk menyembunyikan atau memalsukan source IP address sehingga asal dari paket network tidak bisa terlacak ataupun untuk mengelabui komputer tujuan.

1.  Pembahasan

Spoofing yaitu melakukan penipuan dalam suatu jaringan dengan cara melakukan replikasi atau imitasi identitas. Metode yang dilakukan yaitu memberikan data alamat palsu yang tidak sesuai kepada korban. Contohnya yaitu:

1. A ingin berkomunikasi ke internet sehingga A harus melewati router R agar bisa menuju internet.
2. A bisa menuju ke router R dengan melihat table alamat di dirinya.
3. B ingin menipu A agar tidak sampai ke internet dengan memberikan table palsu.
4. Seingga A melihat table palsu kiriman B dan mengira B adalah router, otomatis aliran menuju internet terputus.

Cara menanggulangi atau counter measure agar tidak terjadi hal seperti itu yaitu:

1. Tidak menerima table dari siapapun
2. Membuat table statis yang tidak bisa diubah atau di update.

Contoh-contoh spoofing yaitu:

1. ARP Spoofing yaitu menipu dengan memberikan alamat fisik palsu.

| IP | MAC |
| --- | --- |
| 192.168.1.1 | 00-30-67-48-6E-EA |
|   |   |

1. DNS Spoofing yaitu menipu dengan memberikan alamat ip palsu.

| Domain | IP |
| --- | --- |
| Google.com | 108.79.5.93 |
|   |   |

1. Penutup

Kesimpulan

Tidak menerima table dari siapapun untuk menanggulangi agar tidak terjadi spoofing.

Saran

Harus lebih berhati-hati karena teknologi masa kini semakin canggih dan maju.