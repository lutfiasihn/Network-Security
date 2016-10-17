OSI (Open System Interconnection) merupakan konsep ideal bagaimana interkoneksi jaringan dilakukan supaya bisa melakukan interkoneksi.  Kenapa ada layernya? Karena untuk memudahkan dalam pembelajaran. Jadi tidak mungkin kita bisa langsung membaca bit tanpa &quot;dibungkus&quot;.  Jadi &quot;bungkusan&quot; bit itu yang disebut layer. Ini adalah koneksi paling ideal, saking idealnya sampai susah diimplementasikan di dunia nyata. Jadi OSI Layer itu merupakan suatu kondisi interkoneksi yang ideal yang susah untuk diimplementasikan ke dalam dunia nyata. Yang kita gunakan sekarang bukan OSI, layer yang kita gunakan sekarang adalah TCP/IP. TCP/IP adalah kondisi pada saat ini dimana kita terhubung dengan dunia melalui internet. Jika OSI memiliki layer yang lengkap yaitu :

Physical Layer (Lapisan 1)

Data Link Layer (Lapisan 2)

Network Layer (Lapisan 3)

Transport Layer (Lapisan 4)

Session Layer (Lapisan 5)

Presentation Layer (Lapisan 6)

Application Layer (Lapisan 7)

Sedangkan  TCP/IP mempunyai 4 layer yaitu :

Application

Transport (TCP/IP)

Internet (IP)

Network Acces Layer (eth)

1. Aplplication ini contohnya yang kita pakai seperti browser, http,gmail,dll.
2. Transport ada 2 yaitu TCP/UDP. Perbedaan TCP dan UDP yaitu jika TCP harus komplit datanya, contohnya yaitu jika data yang dikirimkan 10 maka yang sampai juga harus 10. Fungsinya untuk mengecek data yang dibawa itu ada berapa. Jika UDP tidak komplit, contohnya jika kita mengirimkan data 10 maka hanya 6 yang sampai sana. Kenapa demikian? Karena ini untuk kepentingan fungsional aplikasinya. Jika menggunakan UDP maka aplikasi yang di download akan failed. Contoh aplikasi yang menggunakan UDP yaitu aplikasi untuk video call, Skype,Youtube ( Streaming Youtube menggunakan UDP, dan websitenya menggunakan TCP).
3. IP (Internet Protocol) yaitu bagaimana cara berkomunikasi antar network. Pada dasarnya komputer kita terhubung dengan komputer lain dalam satu ruangan dari satu subnet. Subnet yaitu kelas atau batasan/jumlah komputer. Contohnya : 192.168.1.0/24

Keterangan:

192 = kelas a, 1 blok = 8 bit

168 = kelas b, 1 blok = 8 bit

1 = kelas c, 1 blok = 8 bit

0/24 = kelas d ( karena ada 3 blok, jadi 8 bit x 3 = 24)

Dalam 1 subnet berkomunikasi lewat Mac Address, satu subnet terdapat broadcast dari Mac Address.