---
ID: 610
post_title: >
  Cara Mengamankan Website Untuk Platform
  WordPress
author: ilmanyazid
post_excerpt: ""
layout: post
permalink: >
  https://www.rumahkode.net/blog/mengamankan-website-wordpresa/
published: true
post_date: 2018-05-31 09:58:27
---
<a href="https://www.rumahkode.net/blog/mengamankan-website-wordpresa/">Cara mengamankan situs WordPress</a> kamu. Sebagian besar teknik-teknik ini mudah untuk diterapkan untuk pemula atau memulihkan jika sesuatu yang tidak beres. Jika kamu baru mengguanakan WordPress lanjutkan membaca panduan dasar yang satu ini.
<div>
<h3>1. Delete login Admin</h3>
Default login admin adalah hal mutlak yang akan menjadi sasaran yang mudah untuk mengeksploitasi apapun. Kamu harus menghapus akun pengguna ini segera. Langkah-langkah:

1. login dengan default Admin account
2. membuat pengguna baru dengan nama unik dengan <b>hak Admin</b> &lt; — sangat penting
3. login dengan user "baru" dan menghapus Admin user.

Catatan: Langkah ini juga dapat dengan cepat dilakukan pada instalasi baru dengan mengubah default nama pengguna untuk sesuatu yang lain dari "Admin".
<h3></h3>
<h3>2. Mengubah WordPress Nick namemu</h3>
Bot atau hacker akan menelusur posting situs kamu mencari <b>penulis tag</b> dan kemudian menggunakan nama itu menemukan sebagai login username untuk kamu, ini adalah vektor serangan yang sangat efektif untuk menebak melalui hack. Di WP admin klik profil atau pengguna dan menambahkan julukan (atau nama) dan kemudian pilih "Tampilan nama publik sebagai" sesuatu yang berbeda dari sebenarnya login username untuk kamu!
<h3></h3>
<h3>3. Jadwal backup secara teratur</h3>
Backup secara teratur adalah suatu keharusan dan memiliki backup brkala lebih baik. Itu berarti back up WordPress database dan juga disk server kamu. Ada beberapa plugin backup dan layanan yang akan membuat data cadangan. Hal ini juga sangat dianjurkan untuk meminta host kamu tentang <b>disk berbasis backup</b> dan ingat untuk menjadwalnya.
<h5></h5>
<h3>4. Mendapatkan beberapa kunci keamanan WordPress</h3>
WordPress telah menerapkan kunci keamanan dienkripsi untuk informasi yang disimpan dalam cookie Anda.
Kunci ini terletak di <b><i>wp-config.php</i></b> dan kamu dapat menemukan <i>nomor acak generator kunci</i> di wordpress.org pada alamat URL situs di sini <span style="text-decoration: underline;">https://api.wordpress.org/secret-key/1.1/salt/</span>. Tekan refresh pada browser Anda untuk mendapatkan kunci baru dan copy/paste seluruh hal ke wp-config.php.
<h3></h3>
<h3>5. Mengubah nama awalan pra-instalasi database !</h3>
Ini hanya untuk pra-instalasi wordpress. Kami mencakup melakukan hal ini ke situs hidup dalam panduan lanjutan melakukan hal ini akan menjadikan fatal bagi situs yang sudah lama. Jika kamu baru memulai menginstal, kamu memiliki pilihan selama layar install untuk mengubah database awalan. Semua default WordPress menginstal menggunakan awalan database "wp_" yang membuat exploiter setiap pekerjaan jauh lebih mudah, mengubah awalan ini menjadi sesuatu yang unik.
<h3>6. Batasi penggunaan plugin dan tema dan Hapus yang tidak terpakai.</h3>
Tidak hanya ada banyak plugin dan tema yang tidak aman tetapi mereka dapat memperlambat situs kamu ke rating. Batasi penggunaan plugin kamu sebanyak yang kamu bisa, menghapus plugin yang tidak terpakai dan tema dan menjaga mereka diperbarui. Menjaga sistem website kamu bersih tidak hanya mengurangi sidik jari dan penipu kode dari dieksploitasi tetapi jika sesuatu terjadi untuk menginfeksi situs Anda, itu jauh lebih mudah untuk mengelola.
<h3></h3>
<h3>7. Kunci wp-config direktori</h3>
Wp-config.php file berisi semua kredensial database WordPress kamu, kamu dapat memindahkan file ini naik satu direktori pada server kamu, di luar web root yang bisa melindunginya dari serangan berbasis browser apapun. Hal ini juga ide yang baik untuk mengubah hak akses pada itu untuk 600.
<h3></h3>
<h3>8. Limit login attempts</h3>
Plugin digunakan untuk keamanan dan bergantung pada sesuatu untuk dilindungi. plugin <b>Limit Login Attempts</b> upaya di sisi lain sangat berguna seperti mencegah terlalu banyak gagal login ke situs kamu dan kunci keluar brute kekuatan serangan. Itu bahkan dapat log IP yang gagal masuk.
<h3></h3>
<h3>9. Periksa hak akses file dan direktori</h3>
Izin file dan direktori bisa rumit tergantung pada host. Dalam sebagian besar kasus, kamu ingin memiliki file diatur ke 644 atau 640 dan folder diatur ke 755 atau 750. kamu tidak harus memiliki untuk membuat apa-apa untuk 777 kecuali host kamu telah salah dikonfigurasi.
<h3>10. Sembunyikan version info</h3>
Bersembunyi versi WP info adalah langkah kecil untuk mencegah bot menjelajahi situs kamu, itu tidak mencegah sidik jari, tapi setiap sedikit membantu. Dalam functions.php tema kamu tambahkan berikut:
<div></div>
</div>
<div><code>// remove version info from head and feeds</code></div>
<code>function</code> <code>complete_version_removal() {</code>

<code>    </code><code>return</code> <code>''</code><code>;</code>

<code>}</code>

<code>add_filter(</code><code>'the_generator'</code><code>, </code><code>'complete_version_removal'</code><code>);</code>
<h3>11. Enable ssl login</h3>
Mengaktifkan ssl login jika situs kamu memiliki sertifikat ssl. Untuk mengaktifkan ssl situs kamu harus dapat dicapai dengan menggunakan https. kamu dapat mengaktifkan ini hanya untuk login atau seluruh Admin dalam wp-config.php. SSL login akan mengenkripsi data yang kamu kirimkan ke WordPress dan sangat membantu untuk menggagalkan serangan pra di tengah.
<div><code>// this goes in your wp-config.php file</code></div>
<code>//</code>

<code>//for just the login</code>

<code> </code><code>define(</code><code>'FORCE_SSL_LOGIN'</code><code>, true);</code>

<code>//for the whole admin</code>

<code>define(</code><code>'FORCE_SSL_ADMIN'</code><code>, true);</code>
<h3>12. Jangan biarkan bot pencarian untuk menelusuri direktori</h3>
Pencarian Google dapat merangkak URL yang tidak diinginkan dan mengekspos mereka ke hacker. Terbaik untuk mencegah Google bot dan bot lain yang mengikuti robots.txt (tidak semua dari mereka melakukan) dari pengindeksan apa-apa tapi konten kamu. Robot.txt berjalan di folder root situs kamu dan adalah hanya file teks.
<div>setting di robot.txt</div>
<div><code>User-agent: *</code></div>
<code>Disallow: /feed/</code>

<code>Disallow: /trackback/</code>

<code>Disallow: /wp-admin/</code>

<code>Disallow: /wp-content/</code>

<code>Disallow: /wp-includes/</code>

<code>Disallow: /xmlrpc.php</code>

<code>Disallow: /wp-</code>
<h3>13. Menonaktifkan pendaftaran pengguna.</h3>
Ya kamu dapat menonaktifkan pendaftaran pengguna di Admin, jadi jika kamu menjalankan sebuah blog kecil atau CMS dan tidak memiliki beberapa orang berbagi, pergi ke depan dan menonaktifkan registrasi user sepenuhnya di bawah pengaturan umum.
<h3></h3>
<h3>14. Menonaktifkan tema dan plugin suntingan/update</h3>
Mencegah pengguna mampu mengedit atau memperbarui file sensitif melalui admin.
<div></div>
<div><code>define(</code><code>'DISALLOW_FILE_EDIT'</code><code>,true); </code><code>//edits</code></div>
<code>define(</code><code>'DISALLOW_FILE_MODS'</code><code>,true); </code><code>//updates</code>
<h3>15. Aturan dasar .htaccess</h3>
Beberapa aturan dasar yang dapat kamu tambahkan ke file .htaccess root kamu, yang lebih maju aturan diliputi dalam panduan lanjutan seperti main-main di sini dapat menghancurkan situs kamu, tetapi ini tidak akan banyak selain melindungi kamu.
<div></div>
<div><code>//limit indexing of directories</code></div>
<code>Options All -Indexes</code>

<code>//protect the htaccess file,</code>

<code>//this is done by default with apache config file,</code>

<code>// but you never know.</code>

<code>order allow,deny</code>

<code>deny from all</code>

<code>//disable the server signature</code>

<code>ServerSignature Off</code>

<code>//limit file uploads to 10mb</code>

<code>LimitRequestBody 10240000</code>

<code>// protect wpconfig.php.</code>

<code>//If you followed step 6 this is not necessary.</code>

<code>order allow,deny</code>

<code>deny from all</code>
<h3>16. Hapus readme dan setiap file yang tidak perlu.</h3>
WordPress memiliki readme.html standar, dan banyak plugin dan tema juga datang dengan ini. Cara terbaik hanya menghapus mereka karena mereka dapat digunakan untuk sidik jari atau snooping Umum dan sering mengandung versi. Juga menyimpan folder kamu bersih dari file sampah.

Sekian <a href="https://www.rumahkode.net/blog/mengamankan-website-wordpresa/">Cara mengamankan website untuk platform wordpress</a> ala <a href="https://www.rumahkode.net/">rumahkode.net</a>