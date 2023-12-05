# DNS(Domain Name System)

<div align="center">
<img src="../../asset/minggu 16/dns.jpeg" />
</div>

## cara kerja :
1. Permintaan Resolusi

Saat pengguna memasukkan nama domain (seperti www.example.com) ke dalam browser, komputer pengguna mengirim permintaan resolusi ke server DNS

2. Caching

Server DNS lokal pertama kali memeriksa apakah informasi resolusi untuk domain tersebut sudah ada di cache-nya. Jika ada, informasi tersebut langsung diberikan ke pengguna tanpa harus melakukan pencarian lebih lanjut

3. Tahap Recursive

Jika informasi tidak ditemukan di cache, server DNS lokal akan memulai proses pencarian secara rekursif. Ini melibatkan melakukan pertanyaan kepada server DNS tingkat atas (root server) untuk menemukan server DNS yang bertanggung jawab atas domain tersebut.

4. Pertanyaan ke Server DNS Tingkat Atas

Server DNS lokal mengirim pertanyaan ke server DNS tingkat atas, yang memberikan informasi tentang server DNS otoritatif yang memiliki informasi lengkap tentang domain yang dicari.

5. Pertanyaan ke Server DNS Otoritatif

Server DNS lokal kemudian mengirim pertanyaan ke server DNS otoritatif yang diberikan oleh server DNS tingkat atas. Server otoritatif ini memiliki informasi lengkap tentang nama domain yang dicari.

6. Pengembalian Jawaban

Server DNS otoritatif memberikan jawaban ke server DNS lokal, yang kemudian menyimpan informasi tersebut di cache-nya dan mengirimkan jawaban ke komputer pengguna.

7. Tahap Akhir

Komputer pengguna menerima jawaban dan dapat menggunakan alamat IP yang dikembalikan oleh server DNS untuk membuat koneksi ke server web yang diinginkan.

# Email Server

<div align="center">
<img src="../../asset/minggu 16/email-server.jpeg" />
</div>

## Cara Kerja :
1.  Menerima Email:

Ketika seseorang mengirim email, server pengirim (SMTP) mengirimkan email ke server penerima (juga menggunakan protokol SMTP).

2.  Verifikasi Pengirim:

Server penerima melakukan verifikasi pengirim untuk memastikan bahwa email berasal dari sumber yang sah. Ini melibatkan pengecekan SPF (Sender Policy Framework) dan DKIM (DomainKeys Identified Mail).

3.  Penyaringan Spam:

Server penerima melakukan pengecekan terhadap pesan untuk menentukan apakah itu spam. Ini melibatkan penggunaan filter spam yang memeriksa berbagai atribut pesan.

4.  Penyimpanan Pesan:

Setelah email dianggap aman dan melewati filter spam, server menyimpan email di kotak surat penerima.

5.  Protokol Penerimaan:

Pengguna menggunakan protokol seperti POP3 (Post Office Protocol) atau IMAP (Internet Message Access Protocol) untuk mengakses dan mengunduh email dari server penerima ke perangkat mereka.

6.  Pengiriman Pesan:

Saat pengguna mengirim email, klien email mereka terhubung ke server pengirim menggunakan protokol SMTP, dan server pengirim bertanggung jawab untuk mengirim email ke server penerima.

7.  Pengambilan oleh Penerima:

Penerima mengakses email yang dikirimkan ke kotak surat mereka menggunakan klien email dan protokol seperti POP3 atau IMAP.

8.  Penyimpanan pada Server:

Beberapa email dapat disimpan di server, tergantung pada pengaturan dan kebijakan pengguna, memungkinkan akses dari berbagai perangkat.
