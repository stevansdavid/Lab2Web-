

A. Jawaban Pertanyaan
1. Apa fungsi <table>, <tr>, <th>, dan <td>?
<table> digunakan untuk membuat struktur tabel pada HTML.
<tr> digunakan untuk membuat baris pada tabel.
<th> digunakan untuk membuat sel header atau judul kolom.
<td> digunakan untuk membuat sel yang berisi data.
2. Apa perbedaan <th> dan <td>?

<th> digunakan sebagai sel header atau judul pada tabel, sedangkan <td> digunakan sebagai sel yang berisi data. Secara default, teks pada <th> biasanya ditampilkan tebal dan berada di tengah.

3. Apa fungsi colspan pada tabel?

colspan digunakan untuk menggabungkan beberapa kolom menjadi satu sel. Jumlah kolom yang digabungkan ditentukan berdasarkan nilai yang diberikan pada atribut colspan.

Contoh:

<td colspan="2">Rata-rata</td>

Artinya satu sel tersebut menggunakan ruang dari dua kolom.

4. Apa fungsi <form> dalam HTML?

<form> digunakan untuk membuat formulir yang berfungsi menerima input atau data dari pengguna, seperti nama, email, alamat, pilihan, dan data lainnya.

5. Apa perbedaan radio button dan checkbox?

Radio button digunakan ketika pengguna hanya boleh memilih satu pilihan dari beberapa pilihan yang tersedia.

Checkbox digunakan ketika pengguna dapat memilih satu atau lebih pilihan secara bersamaan.

6. Mengapa <label> sebaiknya terhubung dengan id input melalui atribut for?

Atribut for pada <label> yang memiliki nilai sama dengan id pada input akan menghubungkan label dengan input tersebut.

Contoh:

<label for="nama">Nama</label>
<input type="text" id="nama" name="nama">

Dengan hubungan tersebut, pengguna dapat mengklik label untuk memfokuskan input. Hal ini juga membantu meningkatkan aksesibilitas dan memudahkan pengguna memahami fungsi setiap input.

7. Apa perbedaan <textarea> dengan input type text?

<input type="text"> digunakan untuk memasukkan teks dalam satu baris.

Sedangkan <textarea> digunakan untuk memasukkan teks yang lebih panjang dan dapat terdiri dari beberapa baris, seperti alamat, deskripsi, atau keterangan.

8. Apa fungsi semantic HTML seperti <header>, <nav>, <main>, <section>, <article>, <aside>, dan <footer>?

Semantic HTML digunakan untuk memberikan makna yang jelas pada struktur halaman web.

<header> digunakan sebagai bagian kepala halaman atau bagian tertentu.
<nav> digunakan untuk navigasi.
<main> digunakan untuk konten utama halaman.
<section> digunakan untuk mengelompokkan konten berdasarkan bagian atau topik.
<article> digunakan untuk konten yang berdiri sendiri.
<aside> digunakan untuk konten tambahan atau pelengkap.
<footer> digunakan sebagai bagian kaki halaman atau bagian tertentu.
9. Apa fungsi required, min, max, dan minlength?
required membuat input wajib diisi.
min menentukan nilai minimum yang diperbolehkan.
max menentukan nilai maksimum yang diperbolehkan.
minlength menentukan jumlah karakter minimum yang harus dimasukkan.

Contoh:

<input type="text" required minlength="3">
<input type="number" min="17" max="60" required>
10. Apa perbedaan elemen <audio> dan <video>?

<audio> digunakan untuk menampilkan dan memutar file suara atau audio pada halaman web.

<video> digunakan untuk menampilkan dan memutar file video pada halaman web.

Contoh:

<audio controls>
    <source src="media/audio.mp3" type="audio/mpeg">
</audio>

<video controls width="480">
    <source src="media/video.mp4" type="video/mp4">
</video>

# A. Langkah-Langkah Pengerjaan

## 1. Membuat Tabel Data Mahasiswa

Pada tahap pertama dibuat tabel data mahasiswa menggunakan elemen `<table>`, `<tr>`, `<th>`, dan `<td>`.

```html
<table border="1">
    <tr>
        <th>NIM</th>
        <th>Nama</th>
        <th>Program Studi</th>
    </tr>
    <tr>
        <td>31241001</td>
        <td>Andi</td>
        <td>Teknik Informatika</td>
    </tr>
</table>
```

Screenshot:

![Tahap 1](Screenshot%202026-09-30%20100745.png)

---

## 2. Mengembangkan Tabel dengan `thead`, `tbody`, dan `tfoot`

Pada tahap kedua tabel dikembangkan menggunakan `<thead>`, `<tbody>`, dan `<tfoot>`. Pada bagian footer juga digunakan `colspan` untuk menggabungkan kolom.

```html
<table border="1">
    <caption>Data Mahasiswa</caption>

    <thead>
        <tr>
            <th>NIM</th>
            <th>Nama</th>
            <th>Nilai</th>
        </tr>
    </thead>

    <tbody>
        <tr>
            <td>31241001</td>
            <td>Andi</td>
            <td>85</td>
        </tr>
        <tr>
            <td>31241002</td>
            <td>Budi</td>
            <td>90</td>
        </tr>
    </tbody>

    <tfoot>
        <tr>
            <td colspan="2">Rata-rata</td>
            <td>87.5</td>
        </tr>
    </tfoot>
</table>
```

![Tahap 2](Screenshot%202026-09-30%20101043.png)

---

## 3. Membuat Form Registrasi Mahasiswa

Pada tahap ketiga dibuat form untuk menerima data pengguna menggunakan `<form>`, `<label>`, `<input>`, dan `<button>`.

```html
<form>
    <label for="nama">Nama:</label>
    <input type="text" id="nama" name="nama">

    <label for="email">Email:</label>
    <input type="email" id="email" name="email">

    <button type="submit">Kirim</button>
</form>
```

![Tahap 3](Screenshot%202026-09-30%20101112.png)

---

## 4. Radio Button dan Checkbox

Pada tahap keempat ditambahkan radio button dan checkbox pada form.

Radio button digunakan untuk memilih satu pilihan, sedangkan checkbox dapat digunakan untuk memilih satu atau beberapa pilihan.

```html
<p>Jenis Kelamin:</p>

<input type="radio" id="laki" name="gender" value="laki-laki">
<label for="laki">Laki-laki</label>

<input type="radio" id="perempuan" name="gender" value="perempuan">
<label for="perempuan">Perempuan</label>

<p>Hobi:</p>

<input type="checkbox" id="coding" name="hobi" value="coding">
<label for="coding">Coding</label>

<input type="checkbox" id="desain" name="hobi" value="desain">
<label for="desain">Desain</label>
```

![Tahap 4](Screenshot%202026-09-30%20101154.png)

---

## 5. Select dan Textarea

Pada tahap kelima digunakan `<select>` untuk membuat pilihan program studi dan `<textarea>` untuk memasukkan alamat.

```html
<label for="prodi">Program Studi</label>

<select id="prodi" name="prodi">
    <option value="">-- Pilih Prodi --</option>
    <option value="ti">Teknik Informatika</option>
    <option value="si">Sistem Informasi</option>
</select>

<br><br>

<label for="alamat">Alamat</label>
<br>

<textarea id="alamat" name="alamat" rows="5" cols="40"></textarea>
```

![Tahap 5](Screenshot%202026-09-30%20101222.png)

---

## 6. Validasi Form Dasar

Pada tahap keenam diterapkan validasi dasar menggunakan atribut `required`, `minlength`, `min`, dan `max`.

```html
<form>
    <label for="nama">Nama</label>
    <input type="text" id="nama" name="nama" required minlength="3">

    <label for="email">Email</label>
    <input type="email" id="email" name="email" required>

    <label for="umur">Umur</label>
    <input type="number" id="umur" name="umur" min="17" max="60" required>

    <button type="submit">Kirim</button>
</form>
```

![Tahap 6](Screenshot%202026-09-30%20101252.png)

---

## 7. Membuat Halaman Semantic HTML

Pada tahap ketujuh dibuat struktur halaman menggunakan semantic HTML seperti `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, dan `<footer>`.

```html
<header>
    <h1>Portal Mahasiswa</h1>
</header>

<nav>
    <a href="#">Beranda</a>
    <a href="#">Profil</a>
    <a href="#">Kontak</a>
</nav>

<main>
    <section>
        <h2>Informasi Akademik</h2>

        <article>
            <h3>Praktikum HTML Lanjutan</h3>
            <p>
                Mahasiswa mempelajari tabel, form,
                semantic HTML, multimedia, dan validasi.
            </p>
        </article>
    </section>

    <aside>
        Informasi tambahan mahasiswa.
    </aside>
</main>

<footer>
    <p>&copy; 2026 Teknik Informatika</p>
</footer>
```

![Tahap 7](Screenshot%202026-09-30%20101318.png)

---

## 8. Menambahkan Multimedia

Pada tahap kedelapan ditambahkan elemen multimedia berupa audio dan video menggunakan `<audio>` dan `<video>`.

File multimedia disimpan pada folder `media`.

```text
media/
├── audio.mp3
└── video.mp4
```

Kode audio:

```html
<audio controls>
    <source src="media/audio.mp3" type="audio/mpeg">
    Browser tidak mendukung audio.
</audio>
```

Kode video:

```html
<video controls width="480">
    <source src="media/video.mp4" type="video/mp4">
    Browser tidak mendukung video.
</video>
```

![Tahap 8](Screenshot%202026-09-30%20101435.png)

---

# B. Proyek Mini - Biodata Mahasiswa

Setelah menyelesaikan delapan tahapan praktikum, dibuat proyek mini berupa halaman `biodata.html`.

Halaman ini menggabungkan materi yang telah dipelajari, yaitu semantic HTML, tabel, form, validasi dasar, dan multimedia.

Data yang digunakan:

```text
Nama       : Stevanus David
NIM        : 312410106
Program    : Teknik Informatika
Status     : Bekerja & Mahasiswa
Email      : stevansdavidd@gmail.com
Alamat     : Cikarang Utara, Perum Grand Cikarang City
```

File yang dibuat:

```text
biodata.html
```

Screenshot halaman `biodata.html`:

![Biodata Mahasiswa](Screenshot%202026-09-30%20101855.png)

---

# C. Struktur Folder

```text
Lab2Web/
├── index.html
├── biodata.html
├── media/
│   ├── audio.mp3
│   └── video.mp4
├── Screenshot 2026-09-30 100745.png
├── Screenshot 2026-09-30 101043.png
├── Screenshot 2026-09-30 101112.png
├── Screenshot 2026-09-30 101154.png
├── Screenshot 2026-09-30 101222.png
├── Screenshot 2026-09-30 101252.png
├── Screenshot 2026-09-30 101318.png
├── Screenshot 2026-09-30 101435.png
├── Screenshot 2026-09-30 101855.png
└── README.md
```

---

# D. Kesimpulan

Praktikum 2 HTML Lanjutan membahas penggunaan tabel, form, berbagai jenis input, validasi dasar, semantic HTML, serta multimedia.

Delapan tahapan praktikum telah dikerjakan secara berurutan. Setelah seluruh tahapan selesai, materi tersebut diterapkan kembali dalam proyek mini berupa halaman `biodata.html`.

Melalui praktikum ini dapat dipahami bagaimana HTML digunakan untuk membuat struktur halaman web, menampilkan data dalam tabel, menerima input pengguna, melakukan validasi dasar, menggunakan struktur semantic, serta menampilkan audio dan video.
