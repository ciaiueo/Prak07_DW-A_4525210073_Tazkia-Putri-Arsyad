
# PRAKTIKUM DESAIN WEB - PERTEMUAN 7
## HTML Form Dasar (Input & Pengiriman Data)

---

## 1. Deskripsi Project

Project ini merupakan hasil pengerjaan Praktikum Desain Web Pertemuan 6 yang membahas tentang HTML Form Dasar, Input, dan Pengiriman Data.

Tujuan dari praktikum ini adalah memahami cara membuat formulir pada halaman website menggunakan HTML, mengenal berbagai jenis input, menggunakan label, id, dan name, serta memahami fungsi tombol dalam sebuah form.

Pada project ini dibuat dua halaman formulir, yaitu:
1. Form Pendaftaran Kursus.
2. Form Penerimaan Mahasiswa Baru.

Website dirancang menggunakan kombinasi warna pastel pink, kuning, hijau, dan biru agar tampilannya terlihat menarik, lucu, sederhana, dan mudah digunakan.

---

## 2. Tujuan Praktikum

Tujuan pengerjaan praktikum ini adalah:

- Memahami penggunaan elemen `<form>` dalam HTML.
- Memahami atribut action dan method.
- Mengenal berbagai tipe input HTML.
- Memahami fungsi atribut label, id, dan name.
- Memahami perbedaan button submit, reset, dan button.
- Membuat form yang rapi dan mudah digunakan.
- Menerapkan CSS untuk mempercantik tampilan website.
- Membuat tampilan website yang responsif pada desktop dan mobile.

---

## 3. Struktur Folder Project

Berikut merupakan struktur folder yang digunakan:

```text
Prak07/
│
├── index.html
│
├── mahasiswa.html
│
├── css/
│   └── style.css
│
└── README.md
```

### Keterangan File:

**1. index.html**

Merupakan halaman utama yang berisi Form Pendaftaran Kursus. Halaman ini digunakan untuk memasukkan data calon peserta kursus.

**2. mahasiswa.html**

Merupakan halaman yang berisi Form Penerimaan Mahasiswa Baru. Form ini dibuat berdasarkan studi kasus pada modul praktikum.

**3. css/style.css**

Merupakan file CSS eksternal yang digunakan untuk mengatur desain dan tampilan kedua halaman website.

**4. README.md**

Merupakan file dokumentasi yang menjelaskan isi project, tujuan, struktur folder, fitur, dan cara menjalankan website.

---

## 4. Teknologi yang Digunakan

Dalam pengerjaan project ini digunakan beberapa teknologi:

- **HTML5:** Digunakan untuk membuat struktur halaman website dan elemen formulir.
- **CSS3:** Digunakan untuk mengatur warna, ukuran, jarak, tata letak, dan tampilan website.
- **JavaScript:** Digunakan pada tombol button untuk menampilkan pesan pemberitahuan sederhana.
- **Visual Studio Code:** Digunakan sebagai aplikasi untuk menulis dan mengedit kode program.
- **Google Chrome:** Digunakan untuk menjalankan dan menguji hasil website.

---

## 5. Penjelasan Halaman Website

### A. Form Pendaftaran Kursus (index.html)

Halaman ini merupakan tugas individu yang bertujuan membuat formulir pendaftaran kursus dengan minimal lima tipe input dan tiga jenis button.

Input yang digunakan:

| No. | Jenis Input | Fungsi |
|---|---|---|
| 1 | text | Memasukkan nama lengkap |
| 2 | email | Memasukkan alamat email |
| 3 | password | Memasukkan kata sandi |
| 4 | number | Memasukkan umur |
| 5 | date | Memilih tanggal lahir |
| 6 | tel | Memasukkan nomor telepon |

Tiga jenis button yang digunakan:

1. **Submit:** Digunakan untuk mengirim data formulir.
2. **Reset:** Digunakan untuk mengembalikan seluruh input ke nilai awal.
3. **Button:** Digunakan untuk menampilkan pesan pemberitahuan melalui JavaScript.

Setiap input dilengkapi dengan label, id, dan name agar hubungan antara keterangan dan kolom input dapat berfungsi dengan baik.

### B. Form Penerimaan Mahasiswa Baru (mahasiswa.html)

Halaman ini dibuat berdasarkan studi kasus pada modul praktikum mengenai kebutuhan panitia penerimaan mahasiswa.

Data yang diminta dalam formulir meliputi:

| No. | Field | Tipe Input |
|---|---|---|
| 1 | Nama Lengkap | text |
| 2 | Alamat Email | email |
| 3 | Password | password |
| 4 | Nilai | number |
| 5 | Tanggal Lahir | date |

Setiap field memiliki atribut:

- **Label:** Memberikan keterangan pada setiap kolom.
- **ID:** Memberikan identitas pada elemen input.
- **Name:** Menentukan nama data yang dikirim.
- **Type:** Menentukan jenis data yang dapat dimasukkan.

Pada input nilai juga digunakan atribut min="0" dan max="100" untuk membatasi rentang nilai.

---

## 6. Penjelasan Elemen HTML Form

### A. Form

Elemen `<form>` digunakan untuk membungkus seluruh elemen input yang akan diisi oleh pengguna.

Contoh:

```html
<form action="#" method="post">
```

Atribut yang digunakan:

- **action:** Menentukan tujuan pengiriman data.
- **method:** Menentukan metode pengiriman data.

### B. Method GET dan POST

- **GET:** Mengirimkan data melalui URL dan cocok digunakan untuk pencarian atau data non-sensitif.
- **POST:** Mengirimkan data melalui body request dan lazim digunakan untuk formulir pendaftaran.

Pemilihan method tidak otomatis menjamin keamanan data. Keamanan tetap membutuhkan HTTPS dan validasi server.

### C. Label dan Input

Elemen `<label>` digunakan sebagai keterangan untuk input.

Contoh:

```html
<label for="nama">Nama Lengkap</label>
<input type="text" id="nama" name="nama">
```

Atribut for pada label harus memiliki nilai yang sama dengan id pada input agar keduanya saling terhubung.

### D. Jenis Button

- `type="submit"` untuk mengirim formulir.
- `type="reset"` untuk mengembalikan input ke kondisi awal.
- `type="button"` untuk tombol biasa yang dapat diberikan tindakan menggunakan JavaScript.

---

## 7. Desain dan Tampilan Website

Website menggunakan tema pastel aesthetic dengan kombinasi empat warna utama:

| Warna | Kode Warna | Penggunaan |
|---|---|---|
| Pink Soft | #F8DDE8 | Judul dan tombol daftar |
| Yellow Soft | #FFF0C9 | Tombol reset |
| Green Soft | #DDF1E3 | Tombol periksa data |
| Blue Soft | #DDEBFA | Aksen dan warna latar |

Desain dibuat menggunakan CSS eksternal pada folder css.

Beberapa pengaturan CSS yang diterapkan:

- Background menggunakan kombinasi warna pastel.
- Form menggunakan card berwarna putih.
- Border dibuat membulat menggunakan border-radius.
- Input diberikan jarak dan warna border yang lembut.
- Tombol memiliki warna berbeda sesuai fungsinya.
- Hover digunakan untuk memberikan efek ketika tombol diarahkan kursor.
- Media query digunakan agar tampilan menyesuaikan ukuran layar.

---

## 8. Responsive Design

Website dilengkapi dengan media query CSS untuk menyesuaikan tampilannya pada perangkat mobile.

Contoh kode:

```css
@media (max-width: 480px) {
    .container {
        padding: 22px;
    }

    .buttons {
        flex-direction: column;
    }
}
```

Dengan pengaturan tersebut, tampilan form dapat menyesuaikan ukuran layar yang lebih kecil sehingga tetap nyaman digunakan.

---

## 9. Pengujian Website

Pengujian dilakukan menggunakan Google Chrome untuk memastikan setiap elemen formulir dapat ditampilkan dan digunakan dengan baik.

Beberapa pengujian yang dilakukan:

1. Memastikan kedua halaman dapat dibuka.
2. Memastikan seluruh input dapat digunakan.
3. Memastikan password ditampilkan dalam bentuk karakter tersembunyi.
4. Memastikan input email menggunakan validasi format email dari browser.
5. Memastikan input number dapat menerima angka.
6. Memastikan input date dapat memilih tanggal.
7. Menguji tombol submit, reset, dan button.
8. Memastikan label terhubung dengan input melalui atribut for dan id.
9. Memastikan desain dapat menyesuaikan tampilan desktop dan mobile.

---

## 10. Cara Menjalankan Project

Berikut langkah-langkah menjalankan website:

1. Pastikan seluruh file project sudah berada dalam satu folder.
2. Buka folder project menggunakan Visual Studio Code.
3. Pastikan file HTML sudah terhubung dengan CSS melalui kode:

```html
<link rel="stylesheet" href="css/style.css">
```

4. Simpan seluruh file menggunakan Ctrl + S.
5. Buka file index.html menggunakan Google Chrome.
6. Website Form Pendaftaran Kursus akan ditampilkan.
7. Klik link yang tersedia untuk membuka halaman Form Penerimaan Mahasiswa Baru.

---

## 11. Catatan Pengembangan

Project ini masih berupa prototipe formulir HTML dan belum terhubung dengan backend maupun database.

Atribut action="#" digunakan sebagai placeholder tujuan pengiriman data. Oleh karena itu, data yang dimasukkan belum disimpan secara permanen.

Untuk pengembangan selanjutnya, website dapat diintegrasikan dengan PHP, database MySQL, serta validasi data pada sisi server.

---

## 12. Kesimpulan

Melalui praktikum Desain Web Pertemuan 6, saya telah mempelajari dan menerapkan penggunaan HTML Form untuk membuat formulir pendaftaran kursus dan formulir penerimaan mahasiswa baru.

Saya memahami penggunaan berbagai tipe input, atribut label, id, name, action, dan method, serta perbedaan fungsi tombol submit, reset, dan button.

Selain itu, saya juga menerapkan CSS untuk membuat tampilan website lebih menarik dengan kombinasi warna pastel pink, kuning, hijau, dan biru. Penggunaan media query membantu membuat tampilan website menyesuaikan ukuran layar desktop dan mobile.

Dengan pengerjaan project ini, saya memperoleh pemahaman mengenai dasar pembuatan formulir pada website yang nantinya dapat dikembangkan dan diintegrasikan dengan backend.

---

**Praktikum Desain Web - Pertemuan 6**  
**Materi: HTML Form Dasar (Input & Pengiriman Data)**