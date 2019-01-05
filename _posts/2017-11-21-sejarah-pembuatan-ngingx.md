---
ID: 247
post_title: Sejarah pembuatan Ngingx
author: ilmanyazid
post_excerpt: ""
layout: post
permalink: >
  https://www.rumahkode.net/blog/sejarah-pembuatan-ngingx/
published: true
post_date: 2017-11-21 06:00:20
---
<h2>Apa itu Nginx?</h2>
eNgine X atau yang populer disebut nginx adalah salah satu web server open source seperti Apache, namun sangat ringan dan lebih cepat dalam proses nya. Berbeda dengan Apache yang memiliki fitur lengkap dengan berbagai macam modul yang tertanam di dalamnya, justru membuatnya lebih berat. Ibaratnya begini :
<blockquote>“Apache itu kaya Microsoft Word yang punya banyak banget fitur dan opsi tapi Anda cuma butuh 6 doang. Nginx punya keenam fitur itu, dan 5 dari 6 itu 50 kali lebih cepat dari pada Apache”</blockquote>
<h2>Sejarah Nginx</h2>
Pada tahun 2002, Igor Sysoev mulai mengembangkan webserver baru untuk mengatasi masalah C10K, yaitu tantangan pada web server untuk mulai menangani sepuluh ribu koneksi bersamaan (concurrent connection) sebagai persyaratan untuk web modern. Rilis umum nginx perdana dibuat pada tahun 2004, memenuhi tujuan ini dengan mengandalkan asynchronous dan arsitektur event-driven.

Perkembangan Nginx dan popularitasnya semakin meningkat sejak rilis karena pemanfaatan sumber daya yang ringan dan mampu digunakan pada skala hardware yang minim. Nginx sangat unggul dan cepat dalam melayani konten statis (static content), sementar itu nginx juga tidak kalah dalam melayani konten yang dinamis (dynamic content). Nginx sering dipilih oleh administrator untuk penggunaan sumber daya yang lebih efisien dan respon yang cepat.
<h2>Penggunaan Nginx</h2>
Tau kan website populer di Indonesia serperti Kaskus, Detik.com, Metrotvnews, Tempo, Liputan6, dan website dengan traffic monster lainnya. Seperti kita tau kalau website tersebut punya pengunjung yang luar biasa banyak (itu kenapa saya sebut traffic monster) dan tentunya butuh web server dengan kemampuan yang luar biasa untuk bisa menghandel traffic tersebut. Sudah pasti mereka menggunakan web server Nginx, bukannya Apache. Nah dari sini sudah ketahuan kan kehebatan dari web server Nginx.
<div>
<p style="text-align: left;"><img class="aligncenter wp-image-413 size-full" src="http://www.rumahkode.net/wp-content/uploads/2017/11/netcraft_web_server_data_jan15.jpg" alt="Web server data januari 2015" width="540" height="259" />Netcraft Web Server Survey 2015</p>

</div>
Pada tahun 2015 netcraft mengadakan survey penggunaan web server pada website-website paling sibuk dengan traffic tinggi di dunia. Dan hasilnya bisa Anda lihat sendiri, penguna Apache semakin tahun semakin menurun. Sementara pengguna Nginx semakin tahun semakin naik dengan cukup signifikan. Ini menunjukkan bahwa nginx sudah mulai naik daun dan banyak dilirik oleh banyak web master di dunia untuk menghandel traffic website mereka yang sangat tinggi.
<h2>Fitur Nginx</h2>
Nginx juga punya banyak sekali fitur dan bisa dijadikan berbagai macam Server, seperti :
<ul>
 	<li>Reverse proxy server untuk HTTP, HTTPS, SMTP, POP3, and IMAP protocol</li>
 	<li>Load balancer dan HTTP cache</li>
 	<li>Frontend proxy untuk Apache and web server lain, nggabungin flexibilitas dari Apache dengan static content performance nya Nginx yang mantap.</li>
</ul>
Nginx support FastCGI dan SCGI handlers untuk ngelayanin konten yang dinamis kayak PHP dan Phyton. Selain itu, Nginx juga punya bundlingan Kayak LAMP (Linux Apache MySQL PHP) yaitu LEMP (Linux ENgin x MySQL PHP).
<h2>Kenapa Harus Pilih Nginx?</h2>
<h4>1. Arsitektur Nginx yang Lebih Unggul</h4>
Salah satu hal yang bikin nginx menjadi web server yang sangat cepat adalah jenis arsitektur nginx itu sendiri. Jika di bandingkan dengan apache yang process based, nginx jauh lebih unggul karena event-based nya. Sehingga mampu memanfaatkan thread seminimal mungkin untuk memproses request dari user. Hal ini membuat memori yang terpakai oleh Nginx menjadi minimal. Oleh karena memori yang digunakan sangat kecil, web server menjadi lebih ringan dan lebih responsif (memiliki respon super cepat).
<h4>2. Performa Nginx yang Sangat Mantap</h4>
Untuk menangani siatic content (konten statis), performa Nginx sekitar 2,5 kali lebih cepat dari Apache berdasarkan hasil tes benchmark yang dilakukan oleh Mister Kevin Schroeder. Dalam tes ini dia jalankan 1000 concurrent connection (koneksi bersamaan). Hasil tes benchmark lain dari speedemy.com menggunakan 512 concurrent connection  juga menunjukkan bahwa performa Nginx 2x lebih cepat dari Apache dan memori yang dipakai  sekitar 4% lebih sedikit daripada Apache. Disini udah jelas kelihatan kalau performa nginx pada konten static jauh lebih cepat daripada Apache.
<h4>3. Fitur Nginx yang Cukup Lengkap</h4>
Seperti yang saya sebutkan di atas tentang fitur dan gambarannya, sudah bisa Anda bayangin sendiri lah gimana fitur-fitur nya. Walaupun secara fitur lebih sedikit dari Apache, tapi kalau bicara soal modul, Nginx dan Apache sama-sama punya modul yang komplit kok. Dalam wikivs tercatat bahwa nginx pun memiliki fitur-fitur yang lengkap sesuai kebutuhan sehari-hari, menangani trafik yang sangat padat. Berikut adalah daftar fitur yang memang sesuai kebutuhan :
<ul>
 	<li>Static file serving.</li>
 	<li>SSL/TLS support.</li>
 	<li>Virtual hosts.</li>
 	<li>Reverse proxying.</li>
 	<li>Load balancing.</li>
 	<li>Compression.</li>
 	<li>Access controls.</li>
 	<li>URL rewriting.</li>
 	<li>Custom logging.</li>
 	<li>Server-side includes.</li>
 	<li>Limited WebDAV.</li>
 	<li>FLV streaming.</li>
 	<li>FastCGI.</li>
</ul>
<h4>4. Nginx Support Banyak Sistem Operasi</h4>
Sama seperti Apache yang support banyak Sistem Operasi, Nginx juga gak kalah kok. Nginx support modern UNIX operating system (seperti Linux Distro Debian, Redhat, Slackware dll) dan juga bisa digunakan di Windows loh. Tapi performa Nginx untuk windows masih kurang greget kalau dibandingkan dengan yang Linux.
<h4>5. Nginx Punya Keamanan (Security) yang Mantap</h4>
Baik Nginx dan Apache keduanya memiliki track record keamanan yang sangat baik untuk basis kode C. Basis kode nginx, jauh lebih kecil beberapa kali lipat dari Apache. Selain itu, Nginx juga punya panduan untuk menangani serangan DDOS loh.

Saya sudah sering memakain Apache web server untuk menangani Website lokal (localhost). Website yang saya gunakan yaitu WordPress yang diinstall di XAMPP atau LAMP. Dan setelah mencoba menggunakan Nginx, perbedaan nya cukup signifikan. Akses ke Website nya jadi lebih kenceng dibandingkan dengan Apache, sekitar 2x lebih cepat.

Jadi saya sarankan untuk menggunakan web server nginx untuk membangun website Anda sebelum menyesal kemudian, hehe… untuk Tutorial Cara Instalasi Nginx untuk WordPress akan saya share di artikel selanjutnya.