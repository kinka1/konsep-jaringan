# Praktikum Wireshark

pada percobaamn kali ini kita menggunakan sample http.cap yang sudah kita download.
<div>
    <img src="../asset/http1.png"/>
</div>


Untuk memeriksa semua data yang mengalir dalam sesi HTTP (Protokol Transfer HyperText) yang telah direkam dalam paket jaringan, Anda dapat memanfaatkan fitur "Follow HTTP Stream." Ini membantu dalam melihat keseluruhan permintaan dan tanggapan HTTP dalam format yang lebih mudah dibaca

<div>
    <img src="../asset/http2.png"/>
</div>

warna merah merupakan sebuah "request" yang mana mencakup permintaan yang dikirimkan oleh klien keserver. Anda akan melihat detail seperti metode (GET, POST, dll.), URI, dan header permintaan.

<div>
    <img src="../asset/http3.png"/>
</div>

sedangkan warna biru merupakan sebuah respon dari server ke klien, yang mana akan menampilkan kode status HTTP, header respons, dan body data.

<div>
    <img src="../asset/http4.png"/>
</div>

jika kedua warba digabung maka akan menjadi 

<div>
    <img src="../asset/http5.png"/>
</div>

Lalu kita juga dapat melihat berbagai informasi dari source yang kita inginkan. Semisalnya kita dapat melihat Source Port, dan Destination Portnya

<div>
    <img src="../asset/http6.png"/>
</div>

Sekarang mari ubah sample menjadi telnet-cooked.pcap

<div>
    <img src="../asset/http7.png"/>
</div>

Saat kita menggunakan Stream dari Telnet, kita dapat melihat bahwa request dan responsenya berbeda dari HTML, dari sini kita melihat bahwa request dan responsenya bertipe TCP yang berupa ThreeWay-Handshake.

<div>
    <img src="../asset/telnet8.png"/>
</div>

mari kita ubah lagi sample menjadi dns.cap dan lihat UDP Stream

<div>
    <img src="../asset/dns1.png"/>
</div>

Ada beberapa hal yang bisa kita amati di dns.cap:
- Domain yang di-query.
- Tipe query yang di-request.
- IP Address yang dikembalikan oleh respons.
- Kesalahan apa pun yang terjadi selama sesi query DNS.