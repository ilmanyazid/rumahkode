---
ID: 276
post_title: Mengenal web server litespeed
author: ilmanyazid
post_excerpt: ""
layout: post
permalink: >
  https://www.rumahkode.net/blog/web-server-litespeed/
published: true
post_date: 2017-11-26 01:10:58
---
<h1><a href="http://www.rumahkode.net/">Mengenal web server litespeed</a></h1>
<div></div>
<div>

Berbasis di New Jersey, USA, LiteSpeed teknologi didedikasikan untuk memungkinkan Internet cepat dan menurunkan biaya infrastruktur.

LiteSpeed teknologi didirikan pada awal tahun 2002 oleh sebuah tim insinyur yangdipimpin oleh George Wang. Tim pengembangan inti LiteSpeed yang mengkhususkan diri dalam desain perangkat lunak server dan telah bertahun-tahun pengalamandalam pengembangan perangkat lunak misi-kritis. LiteSpeed Technologies banggamasih menjadi mandiri dan swasta.

Internet juga tumbuh lebih cepat dari sebelumnya, dan banyak situs web yang besar dan penyedia hosting masih mencoba untuk mengurangi beban masalah hanya dengan membeli hardware tambahan. Taktik ini sia-sia dan sakit-siap untuk bertemuhari ini memiliki lalu lintas kebutuhan. LiteSpeed Web Server mendapat lebih kinerjadari infrastruktur yang ada. LSWS's ROI (Return on Investment) nilai adalah salah satu yang tertinggi di industri, memungkinkan pengguna untuk memperluas tanpa hambatan hardware baru.

LiteSpeed Web Server cepat telah menjadi pemimpin industri dalam hal kinerja, skalabilitas, dan keamanan. Paling penting, LSWS sepenuhnya kompatibel dengan Apache, memungkinkan transfer mulus untuk teknologi ini lebih efisien. Semakin banyakpengguna mulai menyadari manfaat yang membawa ini efisiensi dan kemudahan administrasi dan masyarakat LiteSpeed telah berkembang sangat selama bertahun-tahun.

Sekarang saatnya untuk membuat melompat ke LiteSpeed.

(diambil dari laman asli <a href="http://www.litespeedtech.com/">litespeed</a>)

</div>
&nbsp;

Baca juga :
<p style="padding-left: 30px;"><a href="http://www.rumahkode.net/blog/pengertian-web-server/">Pengertian web server</a></p>
<p style="padding-left: 30px;"><a href="http://www.rumahkode.net/blog/sejarah-terbentuknya-web-server-apache/">Web server Apache</a></p>
&nbsp;
<h2>Berikut 7 kelebihan Litespeed bagi layanan hosting</h2>
<div>1. 8-10x lebih cepat daripada Apache. Ini berarti keunggulan 800-1000%.
2. Skala yang tertangani lebih besar
3. Meningkatkan performa PHP hingga 50%
4. Memungkinkan penggunaan control panel pihak ketiga
5. Mendukung PHP4 dan PHP5
6. Small memory footprint
7. Instalasi mudah</div>
<div></div>
<h2>Cara instalasi Litespeed</h2>
<div>
<ol>
 	<li>Download binarynya di website <a href="http://www.litespeedtech.com/products/webserver/download/" target="_blank" rel="noopener">litespeed webserver</a>, ambil yang versi free, karena untuk enterprise, kita harus membayar. Litespeed tersedia untuk Linux dan sistem operasi lainnya.</li>
 	<li>Ekstrak paketnya, buka terminal dan masuk ke direktori hasil ekstrak (lsws-xxx)</li>
 	<li>Jalankan skrip instalasinya:
sudo ./install.sh</li>
 	<li>Ikuti langkah-langkah instalasinya, summary-nya:
- Menyetujui EULA dengan mengetik “Yes”, perhatikan huruf awalnya harus besar.
- Pilih direktori instalasi, saya menginstall di /opt/lsws
- Membuat user admin panelnya
- Memilih user dan grup untuk webservernya.
- Memilih alamat dan port untuk web servernya dan administration panelnya.</li>
 	<li>Jika instalasi selesai tanpa masalah, maka anda bisa mengakses http://localhost untuk website dan http://localhost:70 untuk administratornya.</li>
</ol>
Yang membingungkan adalah menemukan folder server rootnya. Kalau di apache, ada di /var/www/ maka si litespeed ini disatu<strong> folder /usr/local/lsws/DEFAULT/html/</strong>.

</div>