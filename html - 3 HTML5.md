<!-- $theme: default -->

<link rel="stylesheet" type="text/css" href="C:/Users/NavcoreWindows10/Desktop/vito/slide/style.css" /> 

<!---------------------
	Module 3
----------------------->
<!---------------------
	Section 1
----------------------->

<h1 class="section"> &lt;HTML /&gt; <br /> </h1>

<h2 class="section"> Pengenalan HTML5 </h2>

---

# HTML5

Ketika menulis dokumen HTML5, salah satu fitur barunya adalah deklarasi doc type:

```html
<!DOCTYPE HTML>
```

Deklarasi karakter encoding (charset) juga disederhanakan:

```html
<meta charset="UTF-8">
```

**Elemen baru pada HTML5**
`<article>`, `<aside>`, `<audio>`, `<canvas>`, `<datalist>`, `<details>`, `<embed>`, `<footer>`, `<header>`, `<nav>`, `<output>`, `<progress>`, `<section>`, `<video>`, dan masih banyak yang lainnya.

> Default karakter encoding pada HTML5 adalah UTF-8.

---

# Yang Baru pada HTML5

**Forms**
- Spesifikasi Web Forms 2.0 memberikan form yang lebih powerful dan lebih bersahabat dengan user.
- Pemilih tanggal, warna, control numerik juga ditambahkan.
- Tipe field input sekarang memuat email, search, dan URL.
- PUT dan DELETE form method sekarang didukung.

**Integrated API** (Application Programming Interfaces)
<div style="float: left; width: 50%;">
	<ul>
		<li>Drag dan Drop</li>
		<li>Audio dan Video</li>
		<li>Offline Web Applications</li>
		<li>History</li>
	</ul>
</div>

<div style="float: right; width: 50%;">
	<ul>
    	<li>Local Storage</li>
       	<li>Geolocation</li>
       	<li>Web Messaging</li>
    </ul>
</div>

---



<!---------------------
	Section 2
----------------------->

<h1 class="section"> &lt;HTML /&gt; <br /> </h1>

<h2 class="section"> Content Models </h2>

---

# List dari Model Konten

Pada HTML, elemen biasanya berada pada model konten  block-level atau inline. HTML5 memperkenalkan **tujuh** model konten utama.

- Metadata
- Embedded
- Interactive
- Heading
- Phrasing
- Flow
- Sectioning

> Modek konten HTML5 didesain agar struktur markup menjadi lebih bermakna baik untuk browser maupun untuk web desainer.

---

# Model Konten

**Metadata**: Konten yang mengatur presentasi dan perilaku dari konten yang lainnya. Elemen ini berada pada **head** dokumen.
*Elemen*: `<base>`, `<link>`, `<meta>`, `<noscript>`, `<script>`, `<style>`, `<title>`.

**Embedded**: Konten yang meng-import resources ke dokumen.
*Elemen*: `<audio>`, `<video>`, `<canvas>`, `<iframe>`, `<img>`, `<math>`, `<object>`, `<svg>`.

**Interactive**: Konten yang digunakan untuk interaksi user.
*Elemen*: `<a>`, `<audio>`, `<video>`, `<button>`, `<details>`, `<embed>`, `<iframe>`, `<img>`, `<input>`, `<label>`, `<object>`, `<select>`, `<textarea>`.

---

# Model Konten

**Heading**: Mendefinisikan bagian header.
*Elemen*: `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>`, `<hgroup>`.

**Phrasing**: Model ini mempunyai beberapa elemen inline-level yang sama dengan HTML4.
*Elemen*: `<img>`, `<span>`, `<strong>`, `<label>`, `<br />`, `<small>`, `<sub>`,  dan lain-lain.

> Elemen yang sama dapat berada di dalam lebih dari satu model konten. 

---

# Model Konten

**Flow Content**: Memuat sebagian besar elemen HTML5 yang akan dimuat dalam flow normal dari dokumen.

**Sectioning Content**: Mendefinisikan bagian dari heading, konten, navigasi, dan footer. 
*Elemen*: `<article>`, `<aside>`, `<nav>`, `<section>`.

![](C:\Users\NavcoreWindows10\Desktop\vito\slide\model.png)

> Beberapa model konten menumpuk di beberapa bagian, tergantung bagaimana mereka digunakan.

---



<!---------------------
	Section 3
----------------------->

<h1 class="section"> &lt;HTML /&gt; <br /> </h1>

<h2 class="section"> HTML5 Page Structure </h2>

---

# Struktur Halaman di HTML5

Secara umum struktur halaman HTML5 seperti berikut:
![](C:\Users\NavcoreWindows10\Desktop\vito\slide\struktur.png)

> Kita mungkin tidak memerlukan beberapa elemen, tergantung dari struktur halaman kita.

---



<!---------------------
	Section 4
----------------------->

<h1 class="section"> &lt;HTML /&gt; <br /> </h1>

<h2 class="section"> Header, Nav &amp; Footer </h2>

---

# Elemen `<header>`

Pada HTML4, kita akan mendefinisikan header seperti berikut:

```html
<div id="header">
```
Pada HTML5, kita menggunakan tag yang lebih simpel, yaitu `<header>`.

Elemen `<header>` digunakan di dalam tag body.

```html
<!DOCTYPE html>
<html>
   <head></head>
   <body>
      <header>
        <h1> Heading yang Paling Penting </h1>
        <h3> Heading yang Kurang Penting </h3>
      </header>
   </body>
</html>
<
```

---

# Elemen `<header>`

Hasil:

![](C:\Users\NavcoreWindows10\Desktop\vito\slide\header.png)

> Perhatikan bahwa `<header>` sama sekali berbeda dengan `<head>`.

---

# Elemen `<footer>`

Elemen footer juga sering digunakan. Biasanya kita tempatkan pada bagian paling bawah halaman web kita.

```html
<footer> ... </footer>
```

Informasi berikut yang biasanya ditaruh dalam footer:
- Informasi kontak
- Privacy policy
- Ikon sosial media
- Terms of service
- Informasi copyright
- Sitemap dan dokumen yang berhubungan

---

# Elemen `<nav>`

Tag ini menggambarkan bagian dari halaman yang terkait ke halaman lain atau bagian lain dari halamannya. Ini merupakan bagian yang berisi link navigasi.

Berikut contoh blok link navigasi:

```html
<nav>
   <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">Services</a></li>
      <li><a href="#">About us</a></li>
   </ul>
</nav>
```

---

# Elemen `<nav>`

Hasil:
![](C:\Users\NavcoreWindows10\Desktop\vito\slide\nav.png)

> Tidak semua link harus diletakan di dalam elemen `<nav>`. Elemen `<nav>` digunakan untuk link navigasi yang major saja. Terkadang, elemen `<footer>` memuat link yang tidak ada dalam elemen `<nav>`.

---



<!---------------------
	Section 5
----------------------->

<h1 class="section"> &lt;HTML /&gt; <br /> </h1>

<h2 class="section"> Article, Section &amp; Aside </h2>

---

# Elemen `<article>`

**Article** merupakan bagian dari konten yang bebas dan self-contained yang dapat dibuat terpisah dari konten sisanya dari halaman web kita. Ini bisa postingan forum, majalah atau artikel koran, entri blog, komentar, gadget atau widget interaktif, atau konten bebas yang lainnya.

Elemen `<article>` menggantikan elemen `<div>` yang digunakan pada HTML4 dengan id dan class-nya.

```html
<article> 
   <h1>Judul Artikel</h1> 
   <p>Konten dari elemen article,</p>
</article>
```

> Ketika elemen `<article>` bersarang, maka elemen dalam merepresentasikan artikel yang berelasi dengan elemen luarnya. Contohnya adalah komentar postingan blog dalam postingan blog.

---

# Elemen `<section>`

`<section>` merupakan kontainer logikal dari halaman web atau artikel. `<section>` dapat digunakan untuk membagi konten di dalam artikel. Contohnya, homepage dapat memiliki bagian untuk pengenalan perusahaan, item lain yang baru, dan informasi kontak.

Setiap `<section>` harus diidentifikasi, biasanya mengandung heading (elemen h1-h6) sebagai anak dari elemen `<section>`.

```html
<article>
   <h1>Selamat Datang</h1>
   <section>
      <h1>Heading</h1>
      <p>Konten atau Gambar</p>
   </section>
</article>
```

> Jika kita ingin membagi elemen `<section>`, gunakan elemen `<article>`.

---

# Elemen `<aside>`

`<aside>` merupakan konten sekunder yang terpisah tetapi secara tidak langsung berhubungan dengan konten utama. Konten seperti ini biasanya diletakan di sidebar. Ketika tag `<aside>` digunakan didalam tag `<article>`, konten dari `<aside>` harus secara khusus terhubung ke artikel.

```html
<article>
   <h1> Hadiah untuk semua orang </h1>
   <p> Website ini merupakan tempat terbaik untuk memilih hadiah. </p>
   <aside>
      <p> Hadiah akan dikirimkan dalam waktu 24 jam. </p>
   </aside>
</article>
```

Ketika tag `<aside>` digunakan di luar tag `<article>`, kontennya harus berhubungan dengan konten di sekitarnya.

---



<!---------------------
	Section 6
----------------------->

<h1 class="section"> &lt;HTML /&gt; <br /> </h1>

<h2 class="section"> The Audio Element </h2>

---

# Audio pada Web

Sebelum HTML5, tidak ada standard untuk memainkan audio pada halaman web. Elemen HTML5 `<audio>` menspesifikasikan standard audio yang bisa disisipkan pada halaman web.

Ada dua cara untuk menspesifikasikan URL file sumber. Yang pertama menggunakan atribut:

```html
<audio src="audio.mp3" controls>
   Audio tidak disupport oleh browser.
</audio>
```

Yang kedua menggunakan elemen `<source>` di dalam elemen `<audio>`:

```html
<audio controls>
   <source src="audio.mp3" type="audio/mpeg">
   <source src="audio.ogg" type="audio/ogg">
</audio>
```

> Beberapa elemen `<source>` dapat dihubungkan ke audio yang berbeda. Browser akan menggunakan format yang pertama dikenali.

---

# Audio pada Web

Elemen audio dapat membuat audio player dalam browser.

```html
<audio controls>
   <source src="audio.mp3" type="audio/mpeg">
   <source src="audio.ogg" type="audio/ogg">
   Audio tidak support oleh browser.
</audio>
```

hasil:
![](C:\Users\NavcoreWindows10\Desktop\vito\slide\audio.png)

> Teks diantara tag `<audio>` dan `</audio>` akan muncul ketika browser tidak support elemen `<audio>`

---

# Atribut dari `<audio>`

`controls`: Menspedifikasikan bahwa audio control harus ditampilkan (seperti tombol play/pause, dll.)

`autoplay`: Ketika atribut ini didefinisikan, audio akan langsung main ketika dia siap, tanpa meminta izin dari pengunjung.

```html
<audio controls autoplay>
```

`loop`: Atribut ini digunakan untuk audionya untuk langsung memainkan ulang ketika sudah selesai.

```html
<audio controls autoplay loop>
```

> Sekarang, ada tiga format yang disupport: MP3, WAV, dan OGG.

---



<!---------------------
	Section 7
----------------------->

<h1 class="section"> &lt;HTML /&gt; <br /> </h1>

<h2 class="section"> The Video Element </h2>

---

# Video pada HTML

Elemen video serupa dengan elemen audio. Kita dapat menspesifikasikan URL sumber video dengan menggunakan atribut pada elemen video, atau menggunakan elemen `<source>` di dalam elemen `<video>`:

```html
<video controls>
   <source src="video.mp4" type="video/mp4">
   <source src="video.ogg" type="video/ogg">
   Video tidak disupport oleh browser.
</video>
```

> Aspek lain yang dimiliki oleh audio dan video adalan sebagian besar browser tidak support file yang sama. Jika browser tidak support tipe video yang pertama, maka dia akan mencoba yang selanjutnya.

---

# Atribut pada `<audio>`

Aspek lain yang dimiliki oleh kedua elemen audio dan video adalah keduanya memiliki atribut controls, autoplay, dan loop.

Contohnya, videonya akan memainkan ulang setelah selesai:

```html
<video controls autoplay loop>
   <source src="video.mp4" type="video/mp4">
   <source src="video.ogg" type="video/ogg">
   Video tidak disupport oleh browser.
</video>
```

> Untuk sekarang, ada tiga format video yang disupport oleh elemen `<video>`: MP4, WebM, dan OGG.

---



<!---------------------
	Section 8
----------------------->

<h1 class="section"> &lt;HTML /&gt; <br /> </h1>

<h2 class="section"> The Progress Element </h2>

---

# Bar Progres

Elemen `<progress>` mendukung kemampuan untuk membuat bar progres pada web.
Elemen progres dapat digunakan di dalam heading, paragraf, atau tempat lain di dalam body.

**Atribut Elemen Progres**
`value`: Menspesifikasikan seberapa banyak tugas yang sudah selesai.
`max`: Menspesifikasikan banyaknya tugas total.

**Contoh:**

```html
Status: <progress min="0" max="100" value="35">
</progress>
```

---

# Bar Progress

**Hasil:**

![](C:\Users\NavcoreWindows10\Desktop\vito\slide\progres.png)

> Gunakan tag `<progress>` bersamaan dengan JavaScript untuk menampilkan progres secara dinamik.

---



<!---------------------
	Section 9
----------------------->

<h1 class="section"> &lt;HTML /&gt; <br /> </h1>

<h2 class="section"> Web Storage API </h2>

---

# HTML 5 Web Storage

Dengan menggunakan HTML5 web storage, website dapat menyimpan data pada komputer lokal user. Sebelum HTML5, kita harus menggunakan **JavaScript cookies** untuk bisa menggunakan fungsi ini.

**Keuntungan dari Web Storage**
- Lebih aman
- Lebih cepat
- Dapat menyimpan data yang besar
- Data yang disimpan tidak dikirmkan untuk setiap request dari server.

> Storage lokal untuk domainnya masing-masing. Semua halaman dari satu domain dapat menyimpan dan mengakses data yang sama.

---

# Tipe Objek Web Storage

Ada dua tipe objek web storage:
- **sessionStorage()**
- **localStorage()**

**Local vs. Session**
- Session Storage akan dihancurkan saat user menutup browser.
- Local Storage akan menyimpan data tanpa ada batas waktu.

> Kita harus familiar dengan dasar dari JavaScript untuk mengerti dan memahami API ini.

---

# Bekerja dengan Nilai

Sintaks untuk web storage baik storage lokal maupun session sangat sederhana dan sangat mirip (ganti localStorage menjadi sessionStorage.)

**Menyimpan Nilai:**
```html
localStorage.setItem("key1", "value1");
```

**Mendapatkan Nilai:**
```html
//ini akan menampilkan nilainya
alert(localStorage.getItem("key1")); 
```

**Membuang Nilai:**
```html
localStorage.removeItem("key1");
```

**Membuang Semua Nilai:**
```html
localStorage.clear();
```

---



<!---------------------
	Section 10
----------------------->

<h1 class="section"> &lt;HTML /&gt; <br /> </h1>

<h2 class="section"> Geolocation API </h2>

---

# Apa itu Geolocation API?

Pada HTML5, Geolocation API digunakan untuk memperoleh lokasi geografikal user.

Karena hal ini dapat mengganggu privasi user, maka pilihannya tidak akan bekerja sampai user mengizinkan.

> Geolocation akan lebih akurat untuk perangkat yang memiliki GPS, seperti smartphone, dan lainnya.

---

# Menggunakan Geolocation HTML

Method utama API Geolocation adalah `getCurrentPosition`, yang akan mengambil lokasi geografik perangkat user.

```html
navigator.geolocation.getCurrentPosition();
```

Parameter:
**showLocation (wajib)**: Mendefinisikan metode callback yang akan mengambil informasi lokasi.
**ErrorHandler (opsional)**: Mendefinisikan metode callback yang akan dipanggil ketika error terjadi saat proses asynchronous call.
**Options (optional):** Mendefinisikan pilihan untuk memperoleh informasi lokasi.

> Kita harus familiar dengan dasar dari JavaScript untuk mengerti dan memahami API ini.

---

# Menampilkan Data

Lokasi user dapat ditampilkan dalam dua cara: **Geodetic** dan **Civic**.
1. Cara geodetic untuk mendeskripsikan posisi secara langsung dari latitude dan longitude.
2. Representasi civic dari lokasi data menampilkan dalam format yang lebih mudah dibaca dan dimengerti oleh orang biasa.

Parameter berikut menampilkan geodetic dan civic:
![](C:\Users\NavcoreWindows10\Desktop\vito\slide\lokasi.png)
> Method `getCurrentPosition()` mengembalikan sebuah objek jika berhasil. Properties latitude, longitude, dan accuracy akan selalu dikembalikan.

---




<!---------------------
	Section 11
----------------------->

<h1 class="section"> &lt;HTML /&gt; <br /> </h1>

<h2 class="section"> Drag &amp; Drop API </h2>

---

# Membuat Elemen Draggable

Fitur drag and drop membuat kita dapat mengambil sebuah objek dan menggesernya ke lokasi lain. Untuk membuat elemen dapat digeser, pasang atribut `draggable` menjadi `true`.
```html
<img draggable="true" />
```

> Semua elemen HTML dapat digeser.

API untuk drag and drop adalah event-based.

---

Bagian script:
```html
<script>
function allowDrop(ev) {
    ev.preventDefault();
}

function drag(ev) {
    ev.dataTransfer.setData("text", ev.target.id);
}

function drop(ev) {
    ev.preventDefault();
    var data = ev.dataTransfer.getData("text");
    ev.target.appendChild(document.getElementById(data));
}
</script>
```

---

Bagian script:
```html
<body>

   <div id="box" ondrop="drop(event)"
   ondragover="allowDrop(event)"
   style="border:1px solid black; 
   width:200px; height:200px"></div>

   <img id="image" src="sample.jpg" draggable="true"
   ondragstart="drag(event)" width="150" height="50" alt="" />

</body>
```

---

**Apa yang Di-drag**
Ketika elemennya di-drag, atribut `ondragstart` memanggil sebuah fungsi, `drag(event)`, yang menspesifikasikan data apa yang akan di-drag.
Method dataTransfer.setData() menetapkan tipe data dan nilai dari data yang digeser:
```js
function drag(ev) {
    ev.dataTransfer.setData("text", ev.target.id);
}
```

Pada contoh kita, tipe datanya adalah "text" dan nilainya adalah ID dari elemen yang digeser ("image").

---

**Dimana untuk Drop**
Event `ondragover` menspesifikasikan dimana data yang digeser tadi dapat di-drop. Secara default, data dan elemen tidak dapat di-drop pada elemen yang lainnya. Untuk memperbolehkan drop, kita harus mengganti default handling dari elemen.
Hal ini bisa dilakukan dengan cara memanggil method `preventDefault()` untuk event  `ondragover`.

---

**Lakukan Drop**

Ketika data yang digeser tadi di-drop, maka event drop terjadi. Pada contoh diatas, atribut ondrop akan memanggil fungsi `drop(event)`:
```js
function drop(ev) {
    ev.preventDefault();
    var data = ev.dataTransfer.getData("text");
    ev.target.appendChild(document.getElementById(data));
}
```
Method `preventDefault()` menahan handling default dat dari browser. (defaultnya adalah membuka sebagai link saat drop).
Data yang digeser dapat diakses dengan menggunakan method `dataTransfer.getData()`. Method ini akan mengembalikan data yang bertipe sama dengan data yang sudah di-set oleh method `setData()`.
Data yang digeser adalah ID dari elemen yang digeser ("image").

Pada akhirnya, elemen yang digeser akan di-append ke drop element, menggunakan fungsi appendChild().

---




<!---------------------
	Section 12
----------------------->

<h1 class="section"> &lt;HTML /&gt; <br /> </h1>

<h2 class="section"> SVG </h2>

---

# Menggambar Bentuk

**SVG** merupakan singkatan dari **S**calable **V**ector **G**raphics, dan digunakan untuk menggambar bentuk dengan HTML-style.

Dia menawarkan beberapa method untuk menggambar jalur, kotak, lingkaran, teks, dan gambar grafik.

> SVG bukan pixel-based, sehingga dia dapat diperbesar sampai tak hingga kali tanpa kehilangan kualitasnya.

---

# Memasukkan Gambar SVG

Gambar SVG dapat ditambahkan ke code HTML dengan menggunakan tag `<img>`dengan atribut `src` yang menunjuk gambarnya:
```html
<img src="image.svg" alt="" height="300" />
```

---

# Menggambar Lingkaran

Untuk menggambar lingkaran dengan menggunakan SVG, pertama kita harus membuat elemen tag **SVG** dengan dua atribut, width dan height:
```html
<svg widht="1000" height="1000"></svg>
```

Untuk membuat lingkaran, tambahkan tag `<circle>`:
```html
<svg width="2000" height="2000">
   <circle cx="80" cy="80" r="50" fill="green" />
</svg>
```

---

- **cx** menentukan sejauh mana pusat lingkaran dari kiri browser
- **cy** menentukan sejauh mana pusat lingkaran dari atas browser
- **r** menentukan jari-jari lingkaran
- **fill** menentukan warna lingkaran
- **stroke** menambahkan outline pada lingkaran

Hasil:
![](C:\Users\NavcoreWindows10\Desktop\vito\slide\circle.png)

---

# Bentuk yang Lainnya

Tag `<rect>` membuat kotak:
```html
<svg width="2000" height="2000">
   <rect width="300" height="100" 
     x="20" y="20" fill="green" />
</svg>
```

Kode berikut akan menggambar kotak yang berwarna hijau.
![](C:\Users\NavcoreWindows10\Desktop\vito\slide\rect.png)

---

Tag `<line>` membuat garis:
```html
<svg width="400" height="410">
    <line x1="10" y1="10" x2="200" y2="100" 
        style="stroke:#000000; stroke-linecap:round; 
        stroke-width:20"  />
</svg>
```

`(x1,y1)` mendefinisikan koordinat awal, `(x2,y2)` mendefinisikan koordinat  akhir.
![](C:\Users\NavcoreWindows10\Desktop\vito\slide\line.png)

---
Tag `<polyline>` membuat bentuk dari beberapa garis:
```html
<svg width="2000" height="500">
    <polyline style="stroke-linejoin:miter; stroke:black; 
        stroke-width:12; fill: none;"
        points="100 100, 150 150, 200 100" />
</svg>
```

Titik-titiknya adalah koordinat polyline. Kode berikut akan menggambar tanda check berwarna hitam.
![](C:\Users\NavcoreWindows10\Desktop\vito\slide\polyline.png)

---

# `<ellipse>` dan `<polygon>`

**Elips**
Tag `<ellipse>` serupa dengan tag `<circle>`, tetapi dengan 1 pengecualian:
Kita dapat secara bebas menentukan jari-jari horizontal dan jari-jari vertikal dengan menggunakan atribut `rx` dan `ry`.
```html
<svg height="500" width="1000">
   <ellipse cx="200" cy="100" rx="150" ry="70" style="fill:green" />
</svg>
```
Hasil:
![](C:\Users\NavcoreWindows10\Desktop\vito\slide\elips.png)

---

**Polygon**
Elemen `<polygon>` digunakan untuk membuat gambar dengan minimal tiga sisi. Elemen polygon unik karena akan secara otomatis menutup bentuknya untuk kita.
```html
<svg width="2000" height="2000">
<polygon points="100 100, 200 200, 300 0" 
      style="fill: green; stroke:black;" />
</svg>
```
Hasil:
![](C:\Users\NavcoreWindows10\Desktop\vito\slide\polygon.png)

---




<!---------------------
	Section 13
----------------------->

<h1 class="section"> &lt;HTML /&gt; <br /> </h1>

<h2 class="section"> SVG Animations &amp; Paths </h2>

---

# Animasi Bentuk

Animasi SVG dapat dibuat dengan menggunakan elemen `<animate>`.

Contoh di bawah ini membuat kotak yang akan berpindah posisi dalam durasi 3 detik dan akan mengulangi animasinya sebanyak dua kali:
```html
<svg width="1000" height="250">
<rect width="150" height="150" fill="orange">
  <animate attributeName="x" from="0" to="300"
    dur="3s" fill="freeze" repeatCount="2"/> 
</rect>
</svg>
```

---


**attributeName**: Menspesifikasi atribut mana yang akan diberi animasi.
**from**: Menspesifikasi nilai awal atribut
**to**: Menspesifikasi nilai akhir atribut
**dur**: Menspesifikasi lamanya animasi (durasi)
**fill**: Menspesifikasi apakah nilai atribut harus kembali ke awal atau tidak saat animasi selesai (Nilai: `remove` mereset nilainya; `freeze` mempertahankan nilai `to`)
**repeatCount**: Menspesifikasi banyaknya pengulangan animasi.

Pada contoh diatas, kotaknya akan mengubah atribut `x` dari 0 menjadi 300 dalam waktu 3 detik.

> Untuk membuat animasinya berulang-ulang kali, gunakan nilai `indefinite` untuk atribut `repeatCount`.

---

# Jalur

Elemen `<path>` digunakan untuk membuat jalur.

Command berikut yang tersedia untuk data jalur.
**M**: moveto
**L**: lineto
**H**: horizontal lineto
**V**: vertical lineto
**C**: curveto
**S**: smooth curveto
**Q**: quadratic BÃ©zier curve
**T**: smooth quadratic BÃ©zier curveto
**A**: elliptical Arc
**Z**: closepath

---

Definisikan sebuah jalur menggunakan atribut `d`:
```html
<svg width="500" height="500">
<path d="M 0 0 L200 200 L200 0 Z" style="stroke:#000;  fill:none;" />
</svg>
```

M menempatkan "pulpen virtual" pada posisi `(0,0)`. Kemudian dia bergerak sejauh `200px` ke bawah kanan dan ke atas ke posisi `(200,0)`. Command Z menutup bentuknya sehingga hasilnya adalah segitiga siku-siku.

![](C:\Users\NavcoreWindows10\Desktop\vito\slide\path.png)

> Semua command dapat ditulis dalam huruf kecil. Huruf kapital menyatakan posisi absolut, sedangkan huruf kecil menyatakan posisi realtif.

---




<!---------------------
	Section 14
----------------------->

<h1 class="section"> &lt;HTML /&gt; <br /> </h1>

<h2 class="section"> Canvas </h2>

---

# Elemen `<canvas>`

Kanvas HTML digunakan untuk menggamnbar grafik dari garis sederhana sampai objek grafik yang kompleks.

Elemen `<canvas>` didefinisikan oleh:
```html
<canvas id="canvas1" width="200" height="100">
</canvas>
```

> Elemen `<canvas>` hanya sebuah container untuk grafik. Kita harus menggunakan script untuk menggambar. (biasanya JavaScript).

---

Elemen `<canvas>` harus mempunyai atribut `id` sehingga dia bisa dirujuk oleh JavaScript:
```html
<html>
   <head></head>
   <body>
     <canvas id="canvas1" 
   width="400" height="300"></canvas> 

   <script>
      var can = document.getElementById("canvas1"); 
      var ctx = can.getContext("2d");
   </script>

   </body>
</html>
```

`getContext()` mengembalikan drawing context pada kanvas.

> Dasar dari JavaScript diperlukan untuk memahami dan menggunakan kanvas.

---

# Koordinat Kanvas

Kanvas HTML menggunakan grid 2 dimensi. Pojok kiri atas kanvas merupakan koordinat `(0,0)`.

Koordinat X bertambah besar ke kanan.
Koordinat Y bertambah besar ke bawah kanvas.

![](C:\Users\NavcoreWindows10\Desktop\vito\slide\kanvas.png)

---

# Menggambar Bentuk

Method `fillRect(x,y,w,h)` menggambar persegi panjang yang berwarna, dengan `w` menyatakan lebar dan `h` menyatakan tinggi. Warna defaultnya adalah hitam.

Persegi hitam berukuran `100 x 100` digambar pada kanvas di posisi `(20, 20)`:
```js
var c=document.getElementById("canvas1");
var ctx=c.getContext("2d");
ctx.fillRect(20,20,100,100);
```

![](C:\Users\NavcoreWindows10\Desktop\vito\slide\fillrect.png)

---

Properti `fillStyle` digunakan untuk memilih warna, gradien, atau pola untuk mengisi gambarnya. Dengan menggunakan properti ini kita dapat membuat kotak berwarna hijau.
```js
var canvas=document.getElementById("canvas1");
var ctx=canvas.getContext("2d");
ctx.fillStyle ="rgba(0, 200, 0, 1)";
ctx.fillRect (36, 10, 22, 22);
```

![](C:\Users\NavcoreWindows10\Desktop\vito\slide\fillstyle.png)

---

Kanvas juga support method-method lain untuk menggambar:

**Menggambar Garis**
`moveTo(x,y)`: Mendefinisikan titik awal garis.
`lineTo(x,y)`: Mendefinisikan titik akhir garis.

**Mengambar Lingkaran**
`beginPath()`: Memulai menggambar.
`arc(x,y,r,start,stop)`: Memberikan parameter pada lingkaran.
`stroke()`: Mengakhiri menggamber.

**Gradien**
`createLinearGradient(x,y,x1,y1)`: Membuat gradien linier.
`createRadialGradient(x,y,r,x1,y1,r1)`: Membuat gradien radial/sirkular.

**Menggambar Teks pada Kanvas**
`Font`: Mendefinisikan properti font pada teks.
`fillText(text,x,y)`: Menggambar teks yang "terisi" pada kanvas.
`strokeText(text,x,y)`: Menggambar teks pada kanvas (no fill).

> Masih banyak method yang digunakan untuk menggambar pada kanvas.

---




<!---------------------
	Section 15
----------------------->

<h1 class="section"> &lt;HTML /&gt; <br /> </h1>

<h2 class="section"> SVG vs. Canvas </h2>

---

# Canvas vs. SVG

**Canvas**
- Elemen digambar secara program
- Menggambar menggunakan pixel
- Animasi tidak bulit in
- Performa tinggi untuk operasi menggambar berbasiskan pixel
- Bergantung resolusi
- Tidak support event handler
- Bisa kita simpan hasil gambarnya sebagai .png atau .jpg
- Cocok untuk graphic-intensive games

---

**SVG**
- Elemen merupakan bagian dari halaman DOM (Document Object Model)
- Menggambar menggunakan vektor
- Efek dan animasi sudah built in
- Berdasarkan sintaks standard XML, sehingga lebih mudah diakses
- Tidak bergantung resolusi
- Support event handler
- Tidak cocok untuk aplikasi game
- Cocok untuk aplikasi dengan area render yang luas (contohnya Google Maps)

> Kita dapat menggunakan SVG dan kanvas pada halaman yang sama. Tapi kita tidak dapat menggambar SVG pada kanvas, atau sebaliknya.

---




<!---------------------
	Section 16
----------------------->

<h1 class="section"> &lt;HTML /&gt; <br /> </h1>

<h2 class="section"> Canvas Transformations </h2>

---

# Bekerja dengan Kanvas

Elemen kanvas dapat ditransformasi. Contohnya, teks ditulis pada kanvas di posisi `(20,10)`.
```js
ctx.font="bold 22px Tahoma";
ctx.textAlign="start";
ctx.fillText("start", 10, 30);
```

Hasil:
![](C:\Users\NavcoreWindows10\Desktop\vito\slide\transformasi1.png)

---

Method `translate(x,y)` digunakan untuk memindahkan kanvas. `x` menyatakan seberapa jauh berpindah secara horizontal, dan `y` menyatakan seberapa jauh berpindah secara vertikal.
```js
ctx.translate(100, 150);
ctx.fillText("after translate", 10, 30);
```

Pada contoh ini, kanvasnya bergerak ke kanan sejauh `100px` dan ke bawah sejauh `150px`.
![](C:\Users\NavcoreWindows10\Desktop\vito\slide\transformasi2.png)

---

# Method `rotate()`

Method `rotate()` digunakan untuk memutar kanvas HTML5. Nilainya harus dalam radian, tidak boleh derajat.

Berikut contoh yang menggambar kotak yang sama sebelum dan sesudah rotasi diberikan:
```js
ctx.fillStyle = "#FF0000";
ctx.fillRect(10,10, 100, 100);
ctx.rotate( (Math.PI / 180) * 25);  //rotate 25 degrees.
ctx.fillStyle = "#0000FF";
ctx.fillRect(10,10, 100, 100);
```

![](C:\Users\NavcoreWindows10\Desktop\vito\slide\rotate.png)

---

# Method `scale()`

Method `scale()` digunakan untuk mengubah skala gambar kita. Terdapat dua parameter:
- Berapa skala untuk arah X.
- Berapa skala untuk arah Y.

```js
var canvas = document.getElementById('canvas1');
ctx =canvas.getContext('2d');
ctx.font="bold 22px Tahoma";
ctx.textAlign="start";
ctx.fillText("start", 10, 30);
ctx.translate(100, 150);
ctx.fillText("after translate", 0, 0);
ctx.rotate(1);
ctx.fillText("after rotate", 0, 0);
ctx.scale(1.5, 4);
ctx.fillText("after scale", 0,20);
```

---

Ini akan mengubah skala 1.5 kali ke arah X dan 4 kali ke arah Y.

![](C:\Users\NavcoreWindows10\Desktop\vito\slide\scale.png)

---




<!---------------------
	Section 17
----------------------->

<h1 class="section"> &lt;HTML /&gt; <br /> </h1>

<h2 class="section"> HTML5 Forms, Part 1 </h2>

---

# Formulir HTML5

HTML5 memberikan banyak fitur dan pembaharuan untuk pembuatan formulir web. Terdapat atribut baru dan tipe input yang diperkenalkan untuk membantu menciptakan pengalaman yang lebih baik bagi user.
Membuat formulir pada HTML5 sama dengan HTML4.
```html
<form>
   <label>Your name:</label>
   <input id="user" name="username" type="text" />
</form>
```

---

# Atribut Baru

HTML5 memperkenalkan atribut baru disebut `placeholder`. Pada elemen `<input>` dan `<textarea>` atribut ini memberikan hint kepada user informasi apa yang harus dimasukkan ke dalam field.
```html
<form>
   <label for="email">Your e-mail address: </label> 
   <input type="text" name="email" placeholder="email@example.com" /> 
</form>
```

Hasil:
![](C:\Users\NavcoreWindows10\Desktop\vito\slide\placeholder.png)

---

Atribut `autofocus` membuat input yang bersangkutan menjadi fokus saat form-nya di-load:
```html
<form>
   <label for="e-mail">Your e-mail address: </label> 
   <input type="text" name="email" autofocus/>
</form>
```

Hasil:

![](C:\Users\NavcoreWindows10\Desktop\vito\slide\autofocus.png)

---

# Formulir dengan Field yang Perlu Diisi

Atribut `required` digunakan untuk elemen input perlu diisi.

```html
<form autocomplete="off">
   <label for="e-mail">Your e-mail address: </label>
   <input name="Email" type="text" required />
   <input type="submit" value="Submit"/>
</form>
```

Formulir tidak akan bisa dikumpul sampai field yang perlu diisi diisi.
Hasil:
![](C:\Users\NavcoreWindows10\Desktop\vito\slide\required.png)

> Atribut `autocomplete` menspesifikasi apakah formulir atau input field memiliki autocomplete yang on atau off.
> Ketika autocomplete on, browser akan secara otomastis melengkapi nilai berdasarkan nilai yang sudah diinput oleh user sebelumnya.

---

**Beberapa tipe input baru HTML5**
<div style="float: left; width: 25%;">
    <ul>
		<li>color</li>
		<li>date</li>
		<li>datetime</li>
        <li>datetime-local</li>
	</ul>
</div>

<div style="float: left; width: 25%;">
    <ul>
        <li>email</li>
        <li>month</li>
        <li>number</li>
        <li>range</li>
	</ul>
</div>

<div style="float: left; width: 25%;">
    <ul>
        <li>search</li>
        <li>tel</li>
        <li>time</li>
        <li>url</li>
	</ul>
</div>

<div style="float: right; width: 25%;">
	<ul>
        <li>week</li>
	</ul>	
</div>

<p style="clear: both"> </p>

**Atribut input yang baru di HTML5**
<div style="float: left; width: 25%;">
    <ul>
		<li>autofocus</li>
		<li>form</li>
		<li>formaction</li>
		<li>formenctype</li>
	</ul>
</div>

<div style="float: left; width: 25%;">
    <ul>
		<li>formmethod</li>
        <li>formtarget</li>
        <li>height</li>
        <li>weight</li>
	</ul>
</div>

<div style="float: left; width: 25%;">
    <ul>
        <li>list</li>
        <li>min</li>
        <li>max</li>
        <li>multiple</li>
	</ul>
</div>

<div style="float: right; width: 25%;">
	<ul>
        <li>pattern (regexp)</li>
        <li>placeholder</li>
        <li>required</li>
        <li>step</li>
	</ul>	
</div>

<p style="clear: both"> </p>

> Input types that are not supported by old web browsers, will behave as input type text.

---






<!---------------------
	Section 18
----------------------->

<h1 class="section"> &lt;HTML /&gt; <br /> </h1>

<h2 class="section"> HTML5 Forms, Part 2 </h2>

---

# Membuat Search Box

Tipe input baru `search` dapat digunakan untuk membuat search box:
```html
<input id="mysearch" name="searchitem" type="search" />
```

Hasil:
![](C:\Users\NavcoreWindows10\Desktop\vito\slide\search.png)

---

# Opsi Search

Tag `<datalist>` dapat digunakan untuk mendefinisikan list opsi pilihan yang sudah terdefinisi:

```html
<input id="car" type="text" list="colors" />
<datalist id="colors">
   <option value="Red">
   <option value="Green">
   <option value="Yellow">
</datalist>
```

Hasil:
![](C:\Users\NavcoreWindows10\Desktop\vito\slide\datalist.png)

`<option>` mendefinisikan opsi di drop-down list untuk user pilih.

> ID pada elemen datalist harus cocok dengan atribut list pada box input.

---

# Membuat Lebih Banyak Field

Beberapa tipe input baru termasuk `email`, `url`, dan `tel`:

```httml
<input id="email" name="email" type="email" placeholder="example@example.com" />
<br />
<input id="url" name="url" type="url" placeholder="example.com" />
<br />
<input id="tel" name="tel" type="tel" placeholder="555.555.1211" />
```

Hal ini berguna jika halamannya dibuka di perangkat mobile, yang akan mengenali tipe inputnya dan akan membuka keyboard yang bersesuaian dengan tipe fieldnya.

> Tipe baru ini membuat lebih mudah untuk membuat struktur dan memvalidasi formulir HTML.