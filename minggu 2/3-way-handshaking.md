## 3 WAY HANDSHAKING

<div>
    <img src="../asset/3-WAY-HANDSHAKING.png"/>
</div>

Three-way handshake adalah proses fundamental dalam jaringan dan digunakan terutama untuk membangun koneksi yang andal dan aman antara dua perangkat melalui jaringan dengan menggunakan Transmission Control Protocol (TCP). Ini adalah proses tiga langkah yang memastikan bahwa pengirim dan penerima siap untuk pertukaran data. Berikut adalah cara tiga langkah handshake bekerja:

1. **SYN (Synchronize)**       
- Klien mengirim paket SYN ke server
-  Pesan ini berisi nomor urutan awal yang akan digunakan untuk mengidentifikasi data yang dikirim. Langkah ini menunjukkan bahwa klien ingin menginisiasi koneksi. 
2. **SYN-ACK (Synchronize-Acknowledge)**
- Server menerima pesan dari klien kemudian mengirimkan balasan SYN-ACK (synchronize-acknowledge) kembali ke pihak yang memulai koneksi
- Pesan SYN-ACK mengandung nomor urutan acak yang dihasilkan oleh server dan nomor urutan awal yang diterima dari klien
3. **ACK (Acknowledge)**
- Klien menerima pesan SYN-ACK, kemudian mengirimkan balasan ACK (acknowledge) kembali ke pihak tujuan (server)
- Pesan ACK mengandung nomor urutan yang diinkremen untuk mengonfirmasi bahwa pihak klien telah menerima pesan SYN-ACK
- Dengan demikian, koneksi sudah dapat terjalin.

## FUNGSI 3 WAY HANDSHAKING
Proses ini memiliki beberapa fungsi utama:

1. **Menginisiasi Koneksi** : Salah satu fungsi utama tiga langkah handshake adalah untuk menginisiasi koneksi antara dua perangkat atau komputer dalam jaringan. Ketika sebuah perangkat ingin berkomunikasi dengan perangkat lain melalui TCP, langkah pertama handshake memungkinkannya untuk mengirimkan permintaan koneksi.
2. **Verifikasi dan Sinkronisasi** : memastikan bahwa kedua perangkat, pengirim dan penerima, siap dan dapat berkomunikasi. Dalam langkah pertama, pengirim mengirimkan pesan SYN (Synchronize) kepada penerima. Dalam langkah kedua, penerima merespons dengan pesan SYN-ACK (Synchronize-Acknowledge), yang menunjukkan bahwa penerima menerima permintaan dan bersedia untuk mengatur koneksi. Dalam langkah ketiga, pengirim mengonfirmasi dengan mengirimkan pesan ACK (Acknowledge). Ini memastikan bahwa keduanya memiliki informasi yang sesuai untuk memulai pertukaran data.
3. **Mencegah Duplikasi** : Dengan menggunakan nomor urutan (sequence number) dalam tiga langkah handshake, TCP dapat mencegah duplikasi atau pengiriman ganda paket data. Nomor urutan ini membantu memastikan bahwa data yang dikirim oleh pengirim akan diterima dalam urutan yang benar oleh penerima.
4. **Memulai Pertukaran Data Aman** : Setelah tiga langkah handshake selesai, koneksi TCP dianggap telah didirikan dengan aman. Keduanya sekarang dapat mulai bertukar data secara andal dan dengan jaminan bahwa data akan dikirim dan diterima dengan benar.
5. **Menjaga Keandalan Koneksi** : Dalam proses handshake ini, baik pengirim maupun penerima memiliki pemahaman yang jelas tentang status koneksi, dan jika ada masalah dalam proses ini, koneksi tidak akan dibangun atau akan diulang.

Secara keseluruhan, tiga langkah handshake adalah proses kunci dalam TCP yang digunakan untuk memulai dan memastikan koneksi yang aman, andal, dan terkoordinasi antara dua perangkat dalam jaringan. Hal ini penting dalam memastikan bahwa data yang dikirim melalui jaringan TCP dapat diandalkan dan diterima dengan benar oleh penerima.