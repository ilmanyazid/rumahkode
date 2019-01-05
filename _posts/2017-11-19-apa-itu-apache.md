---
ID: 224
post_title: Memahami apa itu apache
author: ilmanyazid
post_excerpt: ""
layout: post
permalink: >
  https://www.rumahkode.net/blog/apa-itu-apache/
published: true
post_date: 2017-11-19 05:36:44
---
<div class="post-header">
<div class="post-header-line-1"><a href="http://www.rumahkode.net/blog/fungsi-dari-web-server/">Web server</a> apache ini dibuat versi pertamanya oleh <strong>Robert Mc Cool</strong> — yang terlibat di NCSA– pada tahun 1996. Ditulis dalam bahasa C, perkembangannya dilakukan bersama rekan-rekan melalui email. Dia mengerjakan proyek itu bersama Apache groupnya : <em>Brian Behlendorf, Roy T. Fielding, Rob Hartill, David Robinson, Cliff Skolnick, Randy Terbush, Robert S. Thau, Andrew Wilson, Eric Hagberg, Frank Peters and Nicolas Pioch</em>.</div>
</div>
<div id="post-body-2055728572481876641" class="post-body entry-content">
<div></div>
<h2>Kenapa diberi nama Apache?</h2>
<div></div>
<div>Kata yang mendirikan karena pertama mereka ingin menghargai penduduk asli Amerika Indian Apache yang dikenal ketahanan dan skilnya saat perang, dan kedua karena akar proyek si apche ini merupakan sebuah ‘a patchy server’. Alasan kedua sebenarnya dengan hoki ditemukan. Apache dikembangkan oleh komunitas terbuka yang di bawahi oleh Apache Software Foundation. Aplikasinya dapat digunakan untuk OS yang beragam( tidak bergantung pada vendor tertentu (cross platform)), sebut saja UNIX, FreeBSD, Linux, Novell netware, MacOS X, Windows.</div>
</div>
<div></div>
<div>(Baca juga : <a href="http://www.rumahkode.net/membangun-bisnis-sampingan/">Cara membangun usaha sampingan</a>)</div>
<div id="post-body-2055728572481876641" class="post-body entry-content">
<div class="fullpost">
<h2>Kelebihan dan kekurangan Apache</h2>
<div><b>Web server Apache mempunyai kelebihan dari beberapa pertimbangan di atas :</b></div>
<ol>
 	<li>Apache termasuk dalam kategori freeware.</li>
 	<li>Apache mudah sekali proses instalasinya jika dibanding web server lainnya seperti NCSA, IIS, dan lain-lain.</li>
 	<li>Mampu beroperasi pada berbagai paltform sistem operasi.</li>
 	<li>Mudah mengatur konfigurasinya. Apache mempunyai hanya empat file konfigurasi.</li>
 	<li>Mudah dalam menambahkan peripheral lainnya ke dalam <a href="http://www.rumahkode.net/">platform web</a> servernya.</li>
</ol>
&nbsp;
<div><b>Fasilitas atau ciri khas dari web server Apache adalah :</b></div>
<ol>
 	<li>Dapat dijadikan pengganti bagi NCSA web server.</li>
 	<li>Perbaikan terhadap kerusakan dan error pada NCSA 1.3 dan 1.4.</li>
 	<li>Apache merespon web client sangat cepat jauh melebihi NCSA.</li>
 	<li>Mampu di kopilasi sesuai dengan spesifikasi HTTP yang sekarang.</li>
 	<li>Apache menyediakan feature untuk multihomed dan virtual server.</li>
 	<li>Kita dapat menetapkan respon error yang akan dikirim web server dengan menggunkan file atau skrip.</li>
 	<li>Server apache dapat otomatis berkomunikasi dengan client browsernya untuk menampilkan tampilan terbaik pada client browsernya.
<strong>Misalnya</strong>, browser ingin menampilkan dalam bahasa spanyol, maka web server apache otomatis mencari dalam servicenya halaman-halaman dengan bahasa spanyol.</li>
 	<li>Web server Apache secara otomatis menjalankan file index.html, halaman utamanya, untuk ditampilkan secara otomatis pada clientnya.</li>
 	<li>Web server Apache mempunyai level-level pengamanan.</li>
 	<li>Apache mempunyai komponen dasar terbanyak di antara web server lain.</li>
 	<li>Ditinjau dari segi sejarah perkembangan dan prospeknya, Apache web server mempunyai prospek yang cerah. Apache berasal dari web server NCSA yang kemudian dikembangkan karena NCSA masih mempunyai kekurangan di bidang kompatibilitasnya dengan sistim operasi lain. Sampai saat ini, <a href="http://www.rumahkode.net/fungsi-dari-web-server/">web server</a> Apache terus dikembangkan oleh tim dari apache.org.</li>
 	<li>Performasi dan konsumsi sumber daya dari web server Apache tidak terlalu banyak, hanya sekitar 20 MB untuk file-file dasarnya dan setiap daemonnya hanya memerlukan sekitar 950 KB memory per child.</li>
 	<li><span style="line-height: 1.4em;">Mendukung transaksi yang aman (secure transaction) menggunakan SSL (secure socket layer).</span></li>
 	<li><span style="line-height: 1.4em;">Mempunyai dukungan teknis melalui web.</span></li>
 	<li><span style="line-height: 1.4em;">Mempunyai kompatibilitas platform yang tinggi.</span></li>
 	<li><span style="line-height: 1.4em;">Mendukung third party berupa modul-modul tambahan.</span></li>
</ol>
&nbsp;

<b>Kekuranga Apache :</b>

Setelah anda mengetahui beberapa kelebihan dari Apache, maka kali ini saya akan menjelaskan tentang beberapa kekurangan dari Apache, beberapa kekurangan dari Apache adalah :
<ol>
 	<li>Web server Apache tidak memiliki kemampuan mengatur load seperti IIS, sehingga akan terus mem-fork proses baru hingga nilai MaxClients tercapai atau hingga batas yang diizinkan oleh OS. Ini tentunya menguntungkan penyerang karena habisnya RAM akan lebih cepat tercapai.</li>
 	<li><span style="line-height: 1.4em;">Apache tidak memproses karakter kutip dalam string Referrer dan User-Agent yang dikirimkan oleh Client. Ini berarti Client dapat memformulasi inputnya secara hati-hati untuk merusak format baris log akses</span><span style="line-height: 1.4em;">.</span></li>
 	<li><span style="line-height: 1.4em;">Terganggunya proses upload data, yang bisa menyebabkan software salah dalam menerjemahkan ukuran data yang masuk. Dengan celah tersebut, hacker dikabarkan dapat mengeksploitasi kerentanan dengan cara mengirimkan request pada server Apache bersangkutan. Versi yang cacat tersebut adalah seluruh generasi Apache 1.3 dan versi 2 hingga 2.0.36. Server yang diserang hacker memanfaatkan kelemahan ini akan mengalami DoS, alias server itu tak bisa diakses. Dalam sejumlah kasus, penyerangnya dapat menjalankan pilihan kodenya.</span></li>
</ol>
</div>
</div>