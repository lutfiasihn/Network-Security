KRIPTOGRAFI

**Latar Belakang**

        Kriptografi di Indonesia disebut persandian yaitu secara singkat dapat berarti seni melindungi data dan informasi dari pihak-pihak yang tidak dikehendaki baik saat ditransmisikan maupun saat disimpan.

**Pembahasan**

        Adalah ilmu dan seni untuk menjaga keamanan pesan ketika pesan dikirim dari suatu tempat ke tempat lainnya (Dony,2008). Jenis dari kriptografi ada beberapa macam seperti  **enkripsi/deskripsi,encode/decode,hash/one way hash**.

**#enkripsi** =

mengubah plaintext jadi ciphertext. contoh:  **caesar cipher:**  jika key= 1 maka m menjadi n HEXA = m menjadi 6D DEC = m menjadi 109 Binary: m menjadi 01101101

**#dekripsi** =

mengembalikan ciphertext jadi plaintext

**#encoding** =

mengubah code menjadi code acak (kode yang di kodekan kembali) contoh: base64: m menjadi bQ== HTML encode: m tetap menjadi m atau m URL encode: m menjadi m, space menjadi %20

**#decoding** =

mengembalikan kode acak ke kode awal (mengembalikan ke kode asli)

**#hash** =

metode enkripsi yang tidak bisa dikembalikan ke nilai awal atau one way hash,. ex=md5,sha-1 dll.  ** **

Perbedaan Enkripsi, Dekripsi dan Encoding yaitu:

**Enkripsi:**

membutuhkan script/tool/alat bantu tambahan untuk membacanya. Jika kalian mengunakan enkripsi pada sistem kalian, maka kalian juga harus membuat decryptor nya juga. Hal ini karena program yang ada tidak bisa membaca enkripsi anda. Misal jika anda menggunakan caesar cipher pada PHP maka anda juga harus membuat decryptor nya, karena PHP tidak mengenali enkripsi model ini. Digunakan untuk menyimpan pesan rahasia misal: database intelejen, session, cookies

**Encoding:**

tidak membutuhkan alat bantu untuk membacanya. Karena biasanya sudah di include kan ke dalam program tersebut. Misal PHP yang langsung bisa membaca encoding base64 anda dengan hanya menggunakan fungsi base64\_decode().

**Hash:**

tidak digunakan untuk dijalankan/script tapi hanya untuk di baca / diketahui. Hanya digunakan untuk menyimpan data-data tertentu yang biasanya penting. Misal: password.

**Kesimpulan**

Dalam kondisi khusus, penerapan kriptografi membutuhkan operator kripto, seperti penyampaian berita rahasia dari satu tempat ke tempat lain (kurir), penyimpanan data dan informasi rahasia ke dalam database atau pengoperasian mesin-mesin khusus kripto.