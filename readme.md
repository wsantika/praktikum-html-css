**LAPORAN PRAKTIKUM**

**PEMBUATAN WEBSITE DENGAN MENGGUNAKAN HTML SEMANTIC LAYOUT**

**Dosen Pengampu: Ir. Gede Humaswara Prathama, S.T., M.T.**

<img width="225" height="225" alt="undiknas" src="https://github.com/user-attachments/assets/16fd02d1-2c87-46bc-8c76-d314dfaed981" />

Oleh:

  -----------------------------------------------------------------------
  Kadek Wahyu Santika Putra                              \(42430012\)
  ------------------------------------------------------ ----------------


**UNIVERSITAS PENDIDIKAN NASIONAL**

**FAKULTAS TEKNIK DAN INFORMATIKA**

**PROGRAM STUDI TEKNOLOGI INFORMASI**

**2025**

  -----------------------------------------------------------------------

1. Tujuan

a.  Menerapkan konsep Semantic HTML untuk struktur halaman web.

b.  Menggunakan berbagai selektor CSS untuk styling elemen HTML.

c.  Menerapkan properti CSS untuk meningkatkan visual halaman web.

d.  Memahami dan menggunakan Box Model dalam desain web.


2. Pendahuluan

Dalam pembuatan halaman web, pemahaman HTML dan CSS sangat penting. HTML
digunakan untuk menyusun struktur konten, sementara CSS berperan
mempercantik tampilan dari sebuah website. Melalui pembelajaran ini ,
mahasiswa mempelajari penerapan Semantic HTML, penggunaan selector CSS,
pemanfaatan properti CSS, serta pemahaman Box Model sebagai dasar
pengaturan desain web. Dengan menguasai hal tersebut, diharapkan mampu
membuat halaman web yang terstruktur, menarik, dan sesuai standar.

3. Pembahasan

index.html

<img width="1434" height="596" alt="code" src="https://github.com/user-attachments/assets/a4ba0d77-1511-4571-b2f4-f90d41ccf29c" />



-   \<!DOCTYPE html\> → Memberitahu browser bahwa ini adalah dokumen
    HTML5.

-   \<html lang=\"en\"\> → Membuka dokumen HTML dengan bahasa English.

-   \<head\> → Bagian kepala dokumen, berisi metadata, judul, dan link
    CSS.

-   \<meta charset=\"UTF-8\"\> → Supaya teks mendukung karakter
    internasional (misalnya huruf é, ñ, dll).

-   \<meta name=\"viewport\" content=\"width=device-width,
    initial-scale=1.0\"\> → Membuat halaman responsif di layar kecil
    (HP/tablet).

-   \<title\>Biodata\</title\> → Judul halaman, akan muncul di tab
    browser.

-   \<link rel=\"stylesheet\" href=\"../css/style-index.css\"\> →
    Menghubungkan file CSS yang ada di folder css.

-   \</head\> → Menutup bagian head.

<img width="1280" height="748" alt="code1" src="https://github.com/user-attachments/assets/8f686965-7dda-475f-bc25-95c51967f5e2" />


-   \<body\> → Bagian utama dari halaman web, semua konten ditaruh di
    sini.

-   \<header\> → Bagian kepala halaman, biasanya untuk logo dan menu
    navigasi.

-   \<h2 class=\"logo\"\>Wahyu Santika\</h2\> → Judul/teks besar untuk
    logo atau nama website.

-   \<nav\> → Tempat menu navigasi (link ke halaman lain).

-   \<ul class=\"nav-container\"\> → Membuat list tak berurut (unordered
    list) untuk menampung menu.

-   \<li\> → Item di dalam list, tiap menu ditaruh di sini.

-   \<a href=\"#\"\>Home\</a\> → Link menuju halaman lain (sementara \#
    artinya belum diarahkan ke mana-mana).

-   \<a href=\"#\"\>CV\</a\> → Link menu ke bagian/halaman CV.

-   \<a href=\"#\"\>Project\</a\> → Link menu ke bagian/halaman Project.

-   \<a class=\"btn\" href=\"#\"\>\<button\>Contact Me\</button\>\</a\>
    → Tombol untuk menghubungi, dibungkus link supaya bisa diarahkan ke
    halaman/form kontak.

style-index.css

<img width="1002" height="2648" alt="code2" src="https://github.com/user-attachments/assets/9fcdb2ce-a3f1-41df-80f7-53470b431cb8" />


-   \* = selector universal, berlaku ke semua elemen.

-   box-sizing: border-box; → supaya padding & border ikut dihitung
    > dalam ukuran elemen.

-   margin: 0; → hapus jarak default luar.

-   padding: 0; → hapus jarak default dalam.

> Semua elemen li, a, dan button di dalam header:

-   font-family → pakai font Montserrat.

-   font-weight: 500; → ketebalan medium.

-   font-size: 16px; → ukuran tulisan standar.

-   color: #000000; → warna teks hitam.

-   text-decoration: none; → hilangkan garis bawah link.

> Semua elemen pada tag header:

-   display: flex; → membuat header pakai flexbox.

-   justify-content: flex-end; → elemen rata kanan.

-   position: sticky; → header menempel di atas saat discroll.

-   top: 0; → posisinya nempel di paling atas.

-   z-index: 1000; → memastikan header tampil di atas elemen lain.

-   align-items: center; → konten di tengah secara vertikal.

-   padding: 10px 10%; → jarak dalam: atas-bawah 10px, kiri-kanan 10%.

-   background-color: #FFFFFF; → warna putih.

-   box-shadow → kasih efek bayangan tipis di bawah header.

> Semua elemen pada kelas logo:

-   .logo → style untuk teks/logo.

-   cursor: pointer; → kursor berubah jadi tangan saat diarahkan.

-   margin-right: auto; → dorong logo ke kiri, sisanya terdorong ke
    > kanan.

-   color: #000000; → warna hitam.

> Style elemen pada kelas nav-container

-   .nav-container → style untuk daftar navigasi.

-   list-style: none; → hilangkan bullet/nomor pada list.

> Style elemen list pada kelas nav-container

-   display: inline-block; → item list sejajar horizontal.

-   padding: 0px 20px; → jarak kiri-kanan antar item.

> Style elemen pada list anchor kelas nav-container

-   Memberikan animasi halus saat link berubah state (misalnya hover).

-   0.3s → durasi animasi 0,3 detik.

-   ease → transisi halus.

-   0s → tanpa delay.

> Style elemen pada list anchor untuk di hover pada kelas nav-container

-   color: #00889a; → saat link di-hover, teks berubah jadi biru
    > kehijauan.

> Style elemen pada button:

-   margin-left: 20px; → jarak dari elemen di sebelah kiri.

-   padding: 9px 25px; → jarak dalam tombol.

-   background-color → warna biru transparan (solid karena 1).

-   border: none; → tanpa garis pinggir.

-   border-radius: 50px; → sudut bulat (tombol pill).

-   cursor: pointer; → kursor jadi tangan.

-   transition → efek animasi saat hover.

> Style elemen pada button untuk di hover

-   Saat tombol di-hover, background jadi lebih transparan (0.8).

> index.html
> 
<img width="1448" height="748" alt="code3" src="https://github.com/user-attachments/assets/73d821a4-40af-4277-9d85-ff0c52a0e3e5" />
>
<img width="1788" height="900" alt="code4" src="https://github.com/user-attachments/assets/daed27b2-4144-4429-9848-d3e340be3170" />

-   \<section\> → elemen untuk membungkus bagian tertentu dari halaman.

-   id=\"about-container\" → penanda unik agar bisa dipanggil di
    > CSS/JavaScript.

-   \<h1\> → judul utama dari section, isinya teks: *Where Every Story
    > Sparks A Journey*.

-   \<div\> → wadah umum.

-   class=\"options\" → untuk styling kelompok pilihan/konten.

-   \<div\> → wadah lagi untuk satu item.

-   class=\"option\" → supaya bisa diatur secara individual di CSS.

-   \<img\> → menampilkan gambar.

-   src=\"foto/foto-ganteng.jpg\" → lokasi file gambar.

-   alt=\"My Photo\" → teks alternatif kalau gambar tidak tampil (juga
    > berguna untuk SEO dan aksesibilitas).

-   \<div\> → wadah isi konten dari satu *option*.

-   class=\"option-content\" → untuk style teks dan link yang menyertai
    > gambar.

-   \<h2\> → sub-judul. Teks: *I\'m continuing to do research into biker
    > culture.*

-   \<a\> → link (walau belum ada href, jadi hanya teks bergaya link).
    > Teks link: *Heaven on the Street*.

> style-index.css
>
<img width="1002" height="2306" alt="code5" src="https://github.com/user-attachments/assets/c99ef38a-7275-4610-9521-75d369b71a4a" />

-   #about-container { \... } → Mendefinisikan gaya untuk kontainer
    > utama bagian \"tentang\".

-   max-width: 1200px; → Menetapkan lebar maksimum kontainer adalah 1200
    > piksel, mencegahnya menjadi terlalu lebar pada layar besar.

-   margin: 0 auto; → Menetapkan margin atas/bawah 0 dan margin
    > kiri/kanan otomatis, yang berfungsi untuk memposisikan kontainer
    > di tengah halaman (horizontal).

-   text-align: center; → Meratakan teks di dalam kontainer ke tengah
    > (horizontal).

-   padding: 20px; → Memberikan jarak/bantalan 20 piksel di sekeliling
    > konten di dalam kontainer.

-   #about-container h1 { \... } → Mendefinisikan gaya untuk elemen
    > \<h1\> (biasanya judul utama) di dalam #about-container.

-   font-size: 24px; → Menetapkan ukuran font judul menjadi 24 piksel

-   margin-bottom: 20px; → Memberikan jarak 20 piksel di bawah judul
    > (margin bawah).

-   display: flex; → Mengubah kontainer menjadi kontainer Flexbox,
    > memungkinkan penataan elemen anak yang fleksibel (opsi-opsi).

-   flex-wrap: wrap; → Memungkinkan elemen anak (opsi) melipat (wrap) ke
    > baris baru jika lebar kontainer tidak cukup.

-   justify-content: center; → Memposisikan item Flexbox (opsi) di
    > tengah kontainer Flex (horizontal).

-   gap: 20px; → Menetapkan jarak (gap) 20 piksel di antara setiap item
    > Flexbox (opsi).

-   .option { \... } → Mendefinisikan gaya untuk setiap elemen opsi
    > individual.

-   background-color: white; → Menetapkan warna latar belakang opsi
    > menjadi putih.

-   border-radius: 8px; → Memberikan sudut membulat (radius) 8 piksel
    > pada opsi.

-   box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); → Menambahkan bayangan
    > kotak dengan pergeseran vertikal 4px, blur 6px, dan warna hitam
    > transparan (opacity 0.1).

-   overflow: hidden; → Menyembunyikan konten di dalam opsi yang mungkin
    > meluap, penting untuk memastikan border-radius bekerja dengan baik
    > pada gambar di dalamnya.

-   text-align: left; → Meratakan teks di dalam opsi ke kiri.

-   width: 300px; → Menetapkan lebar tetap untuk setiap opsi menjadi 300
    > piksel.

-   .option img { \... } → Mendefinisikan gaya untuk elemen gambar
    > (\<img\>) di dalam .option.

-   width: 100%; → Menetapkan lebar gambar 100% dari elemen induknya
    > (.option).

-   height: auto; → Memastikan tinggi gambar menyesuaikan secara
    > proporsional dengan lebarnya.

-   display: block; → Mengubah gambar menjadi elemen blok, yang membantu
    > menghilangkan ruang kosong di bawah gambar yang terkadang muncul
    > pada elemen inline.

-   .option-content { \... } → Mendefinisikan gaya untuk kontainer
    > konten teks/tautan di dalam .option.

-   padding: 15px; → Memberikan jarak/bantalan 15 piksel di sekeliling
    > konten teks di dalam .option.

-   .option-content h2 { \... } → Mendefinisikan gaya untuk elemen
    > \<h2\> (biasanya subjudul/judul opsi) di dalam .option-content.

-   font-size: 18px; → Menetapkan ukuran font subjudul menjadi 18
    > piksel.

-   margin: 0 0 10px; → Menetapkan margin atas dan kiri/kanan 0, dan
    > margin bawah 10 piksel untuk memberikan jarak di bawah subjudul.

-   .option-content a { \... } → Mendefinisikan gaya untuk elemen tautan
    > (\<a\>) di dalam .option-content.

-   color: #007bff; → Menetapkan warna teks tautan menjadi biru cerah
    > (#007bff).

-   text-decoration: none; → Menghapus dekorasi teks (seperti garis
    > bawah) dari tautan.

-   font-weight: bold; → Membuat teks tautan menjadi tebal.

-   .option-content a:hover { \... } → Mendefinisikan gaya saat kursor
    > mengarah (hover) ke elemen tautan (\<a\>) di dalam
    > .option-content.

-   text-decoration: underline; → Menambahkan garis bawah pada tautan
    > saat kursor mengarah padanya, sebagai indikasi interaksi.

indext.html

<img width="1664" height="672" alt="code6" src="https://github.com/user-attachments/assets/39d58fe5-bc18-42b2-92f1-a3a907505743" />

<img width="1094" height="824" alt="code7" src="https://github.com/user-attachments/assets/be5f7466-8990-4a37-bd54-ceffe0ae2f14" />

-   \<footer\> → Mendefinisikan bagian footer (kaki) dari dokumen atau
    bagian. Biasanya berisi informasi hak cipta, informasi kontak, atau
    tautan terkait.

-   \<div\> → Mendefinisikan bagian atau wadah dalam dokumen. Tag ini
    sering digunakan untuk mengelompokkan elemen dan menerapkan gaya
    CSS.

-   \<h2\> → Mendefinisikan judul tingkat 2. Dalam kode ini, digunakan
    sebagai judul untuk bagian kontak (\"CONTACT US\").

-   \<ul\> → Mendefinisikan daftar tak berurutan (unordered list).
    Item-item di dalamnya biasanya ditandai dengan poin atau simbol.

-   \<li\> → Mendefinisikan item daftar (list item). Digunakan untuk
    setiap entri dalam daftar \<ul\> atau \<ol\>.

-   \<a\> → Mendefinisikan tautan hyperlink. Digunakan untuk menautkan
    ke dokumen lain atau, seperti dalam kasus ini, untuk membuat tautan
    email dengan atribut href=\"mailto:\...\".

<img width="1018" height="1888" alt="code8" src="https://github.com/user-attachments/assets/fc39e7d3-dec9-438e-bc2f-e1321818ea55" />

-   footer → Mengatur gaya dasar untuk seluruh elemen kaki halaman
    (footer): memberikan latar belakang hitam, warna teks putih,
    bantalan (padding) 20px, dan perataan teks ke kiri.

-   .footer-container → Mengatur wadah utama di dalam footer menggunakan
    Flexbox (display: flex) untuk tata letak. Ini akan: membentangkan
    item (space-between), membuat item sejajar vertikal ke tengah
    (align-items: center), dan memungkinkan item melipat ke baris baru
    (flex-wrap: wrap).

-   .footer-column → Mengatur gaya dasar untuk setiap kolom di dalam
    footer. Memberi margin 10px di sekelilingnya, memisahkan kolom satu
    sama lain.

-   .footer-column h4 → Mengatur gaya untuk judul (h4) di dalam setiap
    kolom: membuat ukuran font 20px dan memberikan margin bawah 1.2rem
    untuk jarak dengan konten di bawahnya.

-   .footer-column ul → Mengatur gaya untuk daftar tak berurutan (ul) di
    dalam kolom: menghapus simbol poin (list-style: none) dan menghapus
    bantalan (padding: 0) bawaan.

-   .footer-column ul li → Memberikan margin vertikal 5px pada setiap
    item daftar (li) di dalam ul, menciptakan jarak antar baris.

-   .footer-column ul li a → Mengatur gaya untuk tautan (a) di dalam
    item daftar: menghapus garis bawah (text-decoration: none),
    menetapkan warna putih, dan mengatur ukuran font menjadi 0.9rem
    (sedikit lebih kecil).

-   .footer-column ul li a:hover → Mengatur efek saat kursor mengarah
    (hover) ke tautan: menambahkan garis bawah (text-decoration:
    underline) sebagai indikasi interaksi.

-   footer p Mengatur gaya untuk elemen paragraf (p) yang langsung
    berada di dalam

> cv.html
>
<img width="1448" height="748" alt="code9" src="https://github.com/user-attachments/assets/5c3fdbb3-8183-474d-ae58-cf71f6ab306f" />

-   \<!DOCTYPE html\> Deklarasi yang memberi tahu browser bahwa dokumen
    ini adalah dokumen HTML5.

-   \<html lang=\"en\"\> Elemen akar (root) dari halaman HTML. Atribut
    lang=\"en\"

-   \<head\> Wadah untuk meta-informasi tentang dokumen HTML data
    tentang HTML \--ditampilkan langsung di halaman.

-   \<meta charset=\"UTF-8\"\> Menentukan pengkodean karakter dokumen.
    UTF-8 adalah standar universal yang mendukung hampir semua karakter.

-   \<meta name=\"viewport\" \...\> Penting untuk responsivitas.
    Menginstruksikan browser agar lebar halaman sesuai dengan lebar
    layar perangkat (width=device-width) dan skala awal adalah 1.0.

-   \<title\>My-CV\</title\> Menetapkan judul yang akan muncul di bilah
    judul browser atau di tab halaman.

-   \<link rel=\"stylesheet\" \...\> Menautkan dokumen HTML ini ke file
    CSS eksternal (style-cv.css). Atribut rel=\"stylesheet\" menunjukkan
    hubungannya, dan href menunjukkan lokasi filenya.

-   \<body\> Wadah untuk semua konten yang akan ditampilkan kepada
    pengguna, seperti teks, gambar, tautan, dan elemen visual lainnya.

-   \</body\> Tag penutup untuk elemen \<body\>.

-   \</html\> Tag penutup untuk elemen \<html\>.

<img width="1588" height="672" alt="code10" src="https://github.com/user-attachments/assets/a8ccf851-8513-4773-bfb9-916ee83d8d54" />

-   \<body\> Tag pembuka untuk konten utama yang akan ditampilkan di
    halaman web.

-   \<div class=\"profile-container\"\> Wadah utama yang mengelompokkan
    seluruh konten profil. Kelas profile-container digunakan untuk
    menerapkan gaya CSS spesifik pada bagian ini.

-   \<div class=\"profile-header\"\> Wadah bagian header (kepala) dari
    profil, biasanya berisi foto dan info dasar yang diletakkan
    bersebelahan.

-   \<img src=\"\...\" class=\"profile-avatar\"\> Elemen untuk
    menampilkan gambar. Atribut src menentukan lokasi file gambar
    (\"foto/profile.png\"), alt memberikan teks alternatif, dan kelas
    profile-avatar digunakan untuk menata gaya foto profil.

-   \<div class=\"profile-info\"\> Wadah yang mengelompokkan informasi
    teks dari profil (nama, pekerjaan, email).

-   \<h2\>\...\</h2\> Mendefinisikan judul tingkat 2, digunakan di sini
    untuk menampilkan Nama Lengkap.

-   \<p\>\...\</p\> Mendefinisikan paragraf. Digunakan di sini untuk
    menampilkan Status/Pekerjaan (\"Student of Undiknas University\").

-   \<p\>\...\</p\> Mendefinisikan paragraf. Digunakan di sini untuk
    menampilkan Alamat Email.

-   \</div\> Tag penutup untuk elemen \<div class=\"profile-info\"\>.

-   \</div\> Tag penutup untuk elemen \<div
    class=\"profile-container\"\> dan juga elemen \<div
    class=\"profile-header\"\>. (Catatan: Ada satu tag penutup \</div\>
    yang hilang di antara baris 9 dan 10 untuk menutup \<div
    class=\"profile-header\"\>.)

<img width="1756" height="976" alt="code11" src="https://github.com/user-attachments/assets/7e9b2c77-8c2c-44d3-8918-d43314d92d26" />
<img width="1728" height="634" alt="code12" src="https://github.com/user-attachments/assets/14747027-b615-4b4d-a09f-4376077984cc" />

-   profil (Tentang, Pendidikan, Hobi). Kelas profile-details digunakan
    untuk penerapan gaya CSS.

-   \<h3\>About\</h3\> Mendefinisikan judul tingkat 3 untuk bagian
    \"Tentang\" (About).

-   \<p\>\...\</p\> Mendefinisikan paragraf yang berisi deskripsi diri
    singkat (\"Creative beginner, loves to learn, diligent, persistent,
    always developing.\").

-   \<h3\>Education\</h3\> Mendefinisikan judul tingkat 3 untuk bagian
    \"Pendidikan\" (Education).

-   \<ul\> Mendefinisikan daftar tak berurutan untuk item-item
    pendidikan.

-   \<li\>\...\</li\> Mendefinisikan item daftar yang berisi entri
    riwayat pendidikan (Universitas dan Sekolah Menengah Atas).

-   \</ul\> Tag penutup untuk daftar pendidikan.

-   \<h3\>Hobby\</h3\> Mendefinisikan judul tingkat 3 untuk bagian
    \"Hobi\" (Hobby).

-   \<ul\> Mendefinisikan daftar tak berurutan untuk item-item hobi.

-   \<li\>\...\</li\> Mendefinisikan item daftar yang berisi entri-entri
    hobi (\"Fishing,\" \"Racing,\" \"Pangling\").

-   \</ul\> Tag penutup untuk daftar hobi.

-   \</div\> Tag penutup untuk elemen \<div class=\"profile-details\"\>.

-   \</div\> Tag penutup untuk elemen wadah yang lebih besar (tidak
    terlihat di kode ini, mungkin dari file sebelumnya).

-   \</body\> Tag penutup untuk bagian isi utama dokumen.

-   \</html\> Tag penutup untuk seluruh dokumen HTML.

<img width="1034" height="1052" alt="code13" src="https://github.com/user-attachments/assets/34e926be-3103-4165-8f7f-3ffa6fb78314" />

-   font-family → Mengatur font utama halaman menjadi Segoe UI, jika
    tidak ada maka pakai Arial, jika tidak ada juga maka fallback ke
    sans-serif.

-   background → Memberi warna latar belakang halaman dengan warna
    abu-abu sangat muda (#f6f8fa).

-   margin: 0; → Menghilangkan jarak bawaan browser di sekitar body.

-   padding: 0; → Menghilangkan padding default body.

-   max-width: 600px; → Lebar maksimum kontainer adalah 600px (supaya
    tidak terlalu lebar di layar besar).

-   margin: 40px auto; → Memberi jarak 40px di atas dan bawah, serta
    auto kiri dan kanan untuk memposisikan kontainer di tengah
    horizontal.

-   background: #fff; → Latar belakang kontainer berwarna putih.

-   border-radius: 12px; → Membuat sudut kotak menjadi tumpul dengan
    radius 12px.

-   box-shadow → Menambahkan bayangan halus (shadow) di bawah kontainer
    untuk efek mengambang.

-   padding: 32px; → Memberi ruang dalam (padding) antara isi dan tepi
    kontainer sebesar 32px.

-   display: flex; → Mengubah elemen anak dalam header agar menggunakan
    flexbox layout.

-   align-items: center; → Semua item di dalam flex container
    disejajarkan vertikal di tengah.

-   gap: 24px; → Memberi jarak antar item dalam flex container sebesar
    24px.

-   margin-bottom: 24px; → Memberi jarak bawah header terhadap elemen
    berikutnya.

<img width="832" height="2306" alt="code14" src="https://github.com/user-attachments/assets/aa1bf3ae-597b-4ff9-a533-6c58efb3e611" />

-   width & height → Ukuran avatar 120x120 piksel.

-   border-radius: 50%; → Membuat avatar berbentuk lingkaran.

-   object-fit: cover; → Jika avatar berupa gambar, gambar akan
    di-*crop* agar penuh menutupi kotak tanpa distorsi.

-   border → Membuat garis pinggir 2px berwarna abu terang.

-   background → Warna latar belakang abu-abu muda untuk placeholder
    jika gambar tidak ada

-   margin → Menghapus margin atas & samping, hanya memberi 8px di
    bawah.

-   font-size: 2rem; → Ukuran huruf besar, cocok untuk nama user.

-   color: #222; → Warna teks hampir hitam.

-   margin: 0; → Menghilangkan jarak bawaan.

-   color: #555; → Warna teks abu-abu sedang.

-   font-size: 1.1rem; → Ukuran huruf sedang, lebih kecil dari judul.

-   margin-top: 24px; → Memberi jarak antara info profil dan detail
    tambahan.

-   margin-bottom → Jarak bawah judul detail 12px.

-   color → Warna abu gelap.

-   font-size: 1.2rem; → Ukuran judul bagian detail.

-   border-bottom → Garis bawah tipis abu terang sebagai pemisah.

-   padding-bottom: 6px; → Jarak isi teks ke garis bawah.

-   list-style: none; → Menghilangkan bullet list.

-   padding & margin: 0; → Menghapus spasi bawaan list.

-   margin-bottom → Memberi jarak antar item list.

-   color → Warna abu agak gelap.

-   font-size: 1rem; → Ukuran teks standar.

-   \@media (max-width: 700px) → Aturan hanya berlaku di layar kecil
    (≤700px, misalnya mobile/tablet).

-   padding: 16px; → Mengurangi padding container agar lebih hemat ruang
    di layar kecil.

-   flex-direction: column; → Header ditumpuk vertikal (bukan
    horizontal).

-   align-items: flex-start; → Elemen di header disejajarkan ke kiri.

-   gap: 16px; → Jarak antar item diperkecil.

-   width & height → Avatar diperkecil menjadi 90x90px agar proporsional
    di layar kecil.

4.  Kode Hasil Program
<img width="1920" height="1020" alt="halaman-utama1" src="https://github.com/user-attachments/assets/e91039a9-4012-4d17-8a40-56bb0b1010b8" />
<img width="1920" height="1020" alt="halaman-utama2" src="https://github.com/user-attachments/assets/74460268-fc77-412e-85f5-94309211cdc2" />
<img width="1920" height="1020" alt="halaman-css" src="https://github.com/user-attachments/assets/cd7dd7c8-a3dd-4c6c-a328-7d623856e578" />



