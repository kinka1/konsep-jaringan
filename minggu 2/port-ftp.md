## Pengertian FTP

FTP adalah singkatan dari File Transfer Protocol. FTP digunakan untuk mentransfer file antar komputer di jaringan. Kamu bisa menggunakan FTP untuk bertukar file antar akun komputer, mentransfer file antara akun dan komputer desktop, atau mengakses arsip perangkat lunak secara online. Menggunakan server FTP adalah solusi umum untuk bisnis yang ingin menjaga keamanan data mereka. Server FTP yang dihosting bisa menjadi jawaban untuk bisa mendapatkan keamanan data yang lebih baik.

## Mengapa bisa ada 2 protokol FTP yang sama yaitu TCP dan UDP?

Karena Protokol FTP didasarkan pada protokol TCP (Transmission Control Protocol), yang merupakan protokol koneksi yang handal dan terjamin. Berikut adalah penjelasan lebih rinci tentang mengapa FTP menggunakan TCP:

1. **Koneksi Terjamin** : TCP memastikan bahwa data yang dikirimkan dari satu titik ke titik lain tiba dengan aman dan dalam urutan yang benar. Ini sangat penting untuk transfer file, karena kita ingin memastikan bahwa data yang dikirimkan tidak hilang atau rusak selama perjalanan.

2. **Acknowledgment** : TCP menggunakan mekanisme acknowledgment, yang berarti bahwa setiap paket data yang dikirimkan akan diakui oleh penerima. Jika penerima tidak menerima acknowledgment, paket akan dikirim ulang untuk memastikan integritas data.

3. **Reliable** : Protokol TCP dapat membangun koneksi yang handal antara pengirim dan penerima. Ini termasuk mengelola kerusakan dan kesalahan yang mungkin terjadi selama transfer.

4. **Flow Control** : TCP juga mengatur aliran data antara pengirim dan penerima sehingga tidak ada overload atau pemborosan sumber daya.

5. **Port Numbers** : Setiap komunikasi melalui TCP menggunakan port number untuk mengidentifikasi jenis layanan yang dimaksudkan. FTP menggunakan port number 21 untuk menginisiasi koneksi kontrol dan pertukaran perintah, serta port number 20 untuk mentransfer data.

Ketika datang ke UDP (User Datagram Protocol), ini adalah protokol yang lebih ringan dan cepat daripada TCP. Namun, UDP tidak menawarkan kehandalan yang sama seperti TCP. Oleh karena itu, dalam kasus transfer file yang memerlukan integritas data yang tinggi, seperti yang ditemukan dalam protokol FTP, TCP lebih cocok karena memastikan bahwa data dikirim dan diterima dengan benar tanpa risiko kehilangan atau rusak.

Dalam kesimpulannya, FTP hanya menggunakan protokol TCP untuk transfer file karena protokol ini memberikan kehandalan dan integritas yang diperlukan untuk mentransfer data dengan sukses melalui jaringan. Tidak ada versi FTP yang menggunakan protokol UDP.

