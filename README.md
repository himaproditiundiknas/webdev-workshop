# Webdev Workshop - Profil Peserta

Halo teman-teman 👋

Selamat datang di repository **Webdev Workshop**.

Repository ini digunakan sebagai media latihan untuk belajar dasar-dasar **Git**, **GitHub**, **HTML**, dan **CSS**.

Di workshop ini, setiap peserta akan menambahkan **profil pribadi** ke halaman website menggunakan alur kerja GitHub, yaitu:

```text
Fork → Clone → Buat Branch → Edit File → Commit → Push → Pull Request
````

Tenang saja, semua langkah akan dijelaskan dari awal.

---

## Daftar Isi

1. [Tujuan Workshop](#tujuan-workshop)
2. [Apa yang Akan Kamu Buat](#apa-yang-akan-kamu-buat)
3. [Struktur Folder](#struktur-folder)
4. [Persiapan Sebelum Mulai](#persiapan-sebelum-mulai)
5. [Langkah 1 - Fork Repository](#langkah-1---fork-repository)
6. [Langkah 2 - Clone Repository](#langkah-2---clone-repository)
7. [Langkah 3 - Masuk ke Folder Project](#langkah-3---masuk-ke-folder-project)
8. [Langkah 4 - Buat Branch Baru](#langkah-4---buat-branch-baru)
9. [Langkah 5 - Upload Foto Profil](#langkah-5---upload-foto-profil)
10. [Langkah 6 - Buat Halaman Profil](#langkah-6---buat-halaman-profil)
11. [Langkah 7 - Tambahkan Card di Halaman Utama](#langkah-7---tambahkan-card-di-halaman-utama)
12. [Langkah 8 - Cek Perubahan](#langkah-8---cek-perubahan)
13. [Langkah 9 - Commit Perubahan](#langkah-9---commit-perubahan)
14. [Langkah 10 - Push ke GitHub](#langkah-10---push-ke-github)
15. [Langkah 11 - Buat Pull Request](#langkah-11---buat-pull-request)
16. [Ringkasan Perintah Git](#ringkasan-perintah-git)
17. [Aturan Kontribusi](#aturan-kontribusi)
18. [Masalah yang Sering Terjadi](#masalah-yang-sering-terjadi)
19. [Istilah Penting](#istilah-penting)

---

## Tujuan Workshop

Workshop ini bertujuan untuk membantu peserta memahami cara kerja Git dan GitHub melalui praktik langsung.

Setelah mengikuti workshop ini, peserta diharapkan mampu:

* Memahami fungsi Git dan GitHub
* Melakukan fork repository
* Melakukan clone repository
* Membuat branch baru
* Mengedit file HTML dan CSS
* Menambahkan file gambar ke project
* Melakukan commit
* Melakukan push ke GitHub
* Membuat Pull Request

---

## Apa yang Akan Kamu Buat

Setiap peserta akan menambahkan profil pribadi ke website ini.

Data yang akan ditambahkan:

* Foto profil
* Nama lengkap
* NIM
* Program studi
* Deskripsi singkat
* Minat atau ketertarikan

Nantinya semua profil peserta akan tampil di halaman utama dalam bentuk card yang rapi.

---

## Struktur Folder

Repository ini memiliki struktur folder seperti berikut:

```text
webdev-workshop/
├── index.html
├── README.md
├── assets/
│   └── style.css
├── photo/
│   └── foto-peserta.jpg
└── profile/
    └── nim.html
```

Keterangan:

| File / Folder      | Fungsi                                                      |
| ------------------ | ----------------------------------------------------------- |
| `index.html`       | Halaman utama yang menampilkan semua card profil peserta    |
| `README.md`        | File panduan penggunaan repository                          |
| `assets/style.css` | File CSS untuk mengatur tampilan website                    |
| `photo/`           | Folder untuk menyimpan foto profil peserta                  |
| `profile/`         | Folder untuk menyimpan halaman profil masing-masing peserta |

---

## Persiapan Sebelum Mulai

Sebelum mengikuti langkah-langkah di bawah, pastikan kamu sudah memiliki:

1. Akun GitHub
2. Git yang sudah terinstall di laptop
3. Code editor, misalnya Visual Studio Code
4. Koneksi internet

Untuk mengecek apakah Git sudah terinstall, buka terminal lalu jalankan:

```bash
git --version
```

Jika muncul versi Git, berarti Git sudah siap digunakan.

Contoh:

```bash
git version 2.44.0
```

---

# Langkah 1 - Fork Repository

Fork adalah proses menyalin repository utama ke akun GitHub kamu sendiri.

Dengan fork, kamu bisa mengedit repository versi kamu tanpa mengubah langsung repository utama.

Cara melakukan fork:

1. Buka repository ini di GitHub.
2. Klik tombol **Fork** di kanan atas halaman.
3. Klik **Create fork**.
4. Tunggu sampai proses selesai.

Setelah berhasil, kamu akan memiliki repository baru di akun GitHub kamu.

Contoh:

```text
https://github.com/username-kamu/webdev-workshop
```

Repository tersebut adalah hasil fork milik kamu.

---

# Langkah 2 - Clone Repository

Clone adalah proses mengambil repository dari GitHub ke laptop kamu.

Pastikan kamu melakukan clone dari repository hasil fork milik kamu, bukan langsung dari repository utama.

Cara clone:

1. Buka repository hasil fork di akun GitHub kamu.
2. Klik tombol **Code**.
3. Pilih tab **HTTPS**.
4. Copy link repository.

Kemudian buka terminal atau Git Bash, lalu jalankan:

```bash
git clone https://github.com/username-kamu/webdev-workshop.git
```

Ganti `username-kamu` dengan username GitHub kamu.

Contoh:

```bash
git clone https://github.com/santika/webdev-workshop.git
```

---

# Langkah 3 - Masuk ke Folder Project

Setelah clone selesai, masuk ke folder project:

```bash
cd webdev-workshop
```

Untuk melihat isi folder, kamu bisa menjalankan:

```bash
ls
```

Di Windows Command Prompt, bisa menggunakan:

```bash
dir
```

---

# Langkah 4 - Buat Branch Baru

Branch adalah jalur kerja terpisah.

Kita membuat branch baru agar perubahan yang kita buat tidak langsung masuk ke branch utama.

Gunakan format nama branch berikut:

```text
tambah-profile-nama-kamu
```

Contoh:

```bash
git checkout -b tambah-profile-santika
```

Contoh lain:

```bash
git checkout -b tambah-profile-budi
```

```bash
git checkout -b tambah-profile-citra
```

Untuk mengecek branch aktif, jalankan:

```bash
git branch
```

Branch yang sedang aktif biasanya ditandai dengan simbol `*`.

---

# Langkah 5 - Upload Foto Profil

Masukkan foto profil kamu ke folder:

```text
photo/
```

Gunakan nama file berdasarkan NIM agar rapi dan tidak sama dengan peserta lain.

Contoh:

```text
photo/123456789.jpg
```

Jika foto kamu berformat PNG:

```text
photo/123456789.png
```

Aturan foto:

* Gunakan foto yang sopan
* Gunakan format `.jpg`, `.jpeg`, atau `.png`
* Disarankan menggunakan foto berbentuk kotak
* Jangan upload KTP, kartu keluarga, alamat rumah, password, atau dokumen pribadi lainnya

---

# Langkah 6 - Buat Halaman Profil

Masuk ke folder:

```text
profile/
```

Lalu buat file HTML baru dengan nama berdasarkan NIM kamu.

Contoh:

```text
profile/123456789.html
```

Isi file tersebut dengan template berikut:

```html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <title>Profil Nama Kamu</title>

  <link rel="stylesheet" href="../assets/style.css" />
</head>
<body>
  <header>
    <h1>Profil Peserta</h1>
    <p>Halaman profil peserta Webdev Workshop</p>
  </header>

  <main class="profile-detail">
    <img src="../photo/123456789.jpg" alt="Foto Profil Nama Kamu" class="profile-photo" />

    <section class="profile-info">
      <h2>Nama Kamu</h2>

      <p><strong>NIM:</strong> 123456789</p>
      <p><strong>Program Studi:</strong> Teknologi Informasi</p>

      <h3>Tentang Saya</h3>
      <p>
        Tulis deskripsi singkat tentang diri kamu di sini.
        Contoh: Saya adalah mahasiswa yang sedang belajar web development.
      </p>

      <h3>Minat</h3>
      <ul>
        <li>Web Development</li>
        <li>UI/UX Design</li>
        <li>Frontend Development</li>
      </ul>

      <a href="../index.html" class="back-link">Kembali ke halaman utama</a>
    </section>
  </main>
</body>
</html>
```

Ubah bagian berikut sesuai data kamu:

```text
Nama Kamu
123456789
Teknologi Informasi
Deskripsi tentang saya
Minat
Nama file foto
```

Perhatikan bagian foto:

```html
<img src="../photo/123456789.jpg" alt="Foto Profil Nama Kamu" class="profile-photo" />
```

Jika foto kamu menggunakan format `.png`, maka ubah menjadi:

```html
<img src="../photo/123456789.png" alt="Foto Profil Nama Kamu" class="profile-photo" />
```

---

# Langkah 7 - Tambahkan Card di Halaman Utama

Setelah membuat halaman profil, buka file:

```text
index.html
```

Cari bagian komentar berikut:

```html
<!-- Peserta menambahkan card baru di bawah ini -->
```

Lalu tambahkan card profil kamu di bawah komentar tersebut.

Contoh:

```html
<div class="card">
  <a href="profile/123456789.html">
    <img src="photo/123456789.jpg" alt="Foto Profil Nama Kamu" />
    <span class="caption">
      <strong>Nama Kamu</strong>
      <small>NIM: 123456789</small>
    </span>
  </a>
</div>
```

Pastikan:

* `href` mengarah ke file profil kamu
* `src` mengarah ke foto kamu
* Nama dan NIM sudah benar

Contoh jika menggunakan data Santika:

```html
<div class="card">
  <a href="profile/123456789.html">
    <img src="photo/123456789.jpg" alt="Foto Profil Santika" />
    <span class="caption">
      <strong>Santika</strong>
      <small>NIM: 123456789</small>
    </span>
  </a>
</div>
```

---

# Langkah 8 - Cek Perubahan

Sebelum menyimpan perubahan, cek file apa saja yang berubah.

Jalankan:

```bash
git status
```

Biasanya akan terlihat file seperti:

```text
index.html
photo/123456789.jpg
profile/123456789.html
```

Jika file-file tersebut muncul, berarti perubahan sudah terdeteksi oleh Git.

---

# Langkah 9 - Commit Perubahan

Tambahkan semua perubahan:

```bash
git add .
```

Lalu buat commit:

```bash
git commit -m "Menambahkan profil Nama Kamu"
```

Contoh:

```bash
git commit -m "Menambahkan profil Santika"
```

Commit adalah proses menyimpan riwayat perubahan di Git.

Gunakan pesan commit yang jelas.

Contoh yang baik:

```text
Menambahkan profil Santika
Menambahkan foto dan halaman profil Budi
Menambahkan card profil Citra
```

Contoh yang kurang baik:

```text
update
fix
coba
tes
```

---

# Langkah 10 - Push ke GitHub

Push adalah proses mengirim perubahan dari laptop ke GitHub.

Jalankan:

```bash
git push origin nama-branch-kamu
```

Contoh:

```bash
git push origin tambah-profile-santika
```

Setelah push berhasil, perubahan kamu akan masuk ke repository hasil fork milik kamu di GitHub.

---

# Langkah 11 - Buat Pull Request

Pull Request adalah permintaan untuk menggabungkan perubahan dari repository kamu ke repository utama.

Cara membuat Pull Request:

1. Buka repository hasil fork kamu di GitHub.
2. Klik tombol **Compare & pull request**.
3. Pastikan arah Pull Request benar.

Biasanya arahnya seperti ini:

```text
base repository: himaproditiundiknas/webdev-workshop
base branch: main

head repository: username-kamu/webdev-workshop
compare branch: tambah-profile-nama-kamu
```

4. Isi judul Pull Request.

Contoh judul:

```text
Menambahkan profil Santika
```

5. Klik **Create pull request**.

Setelah itu, mentor atau panitia akan mengecek Pull Request kamu.

Jika sudah sesuai, Pull Request akan digabungkan ke repository utama.

---

# Ringkasan Perintah Git

Berikut ringkasan perintah yang digunakan dari awal sampai akhir:

```bash
git clone https://github.com/username-kamu/webdev-workshop.git
cd webdev-workshop
git checkout -b tambah-profile-nama-kamu
git status
git add .
git commit -m "Menambahkan profil Nama Kamu"
git push origin tambah-profile-nama-kamu
```

Contoh lengkap:

```bash
git clone https://github.com/santika/webdev-workshop.git
cd webdev-workshop
git checkout -b tambah-profile-santika
git status
git add .
git commit -m "Menambahkan profil Santika"
git push origin tambah-profile-santika
```

---

# Aturan Kontribusi

Agar repository tetap rapi, ikuti aturan berikut:

1. Jangan menghapus file peserta lain.
2. Jangan mengubah data peserta lain.
3. Jangan mengubah foto peserta lain.
4. Jangan mengubah file CSS tanpa arahan mentor.
5. Simpan foto hanya di folder `photo/`.
6. Simpan halaman profil hanya di folder `profile/`.
7. Gunakan nama file berdasarkan NIM.
8. Pastikan data kamu sudah benar sebelum membuat Pull Request.

---

# Format Nama File

Gunakan format berikut:

```text
photo/nim.jpg
profile/nim.html
```

Contoh:

```text
photo/123456789.jpg
profile/123456789.html
```

Jika menggunakan PNG:

```text
photo/123456789.png
profile/123456789.html
```

---

# Masalah yang Sering Terjadi

## 1. Foto Tidak Muncul

Periksa nama file dan lokasi foto.

Jika foto berada di folder `photo`, maka di `index.html` gunakan:

```html
<img src="photo/123456789.jpg" alt="Foto Profil Nama Kamu" />
```

Jika foto dipanggil dari file di dalam folder `profile`, gunakan:

```html
<img src="../photo/123456789.jpg" alt="Foto Profil Nama Kamu" />
```

Perhatikan perbedaan:

```text
photo/123456789.jpg
../photo/123456789.jpg
```

---

## 2. Halaman Profil Tidak Terbuka

Periksa link di `index.html`.

Contoh yang benar:

```html
<a href="profile/123456789.html">
```

Pastikan nama file di folder `profile` sama persis.

---

## 3. Error Saat git clone

Pastikan link repository benar.

Contoh:

```bash
git clone https://github.com/username-kamu/webdev-workshop.git
```

Jangan lupa mengganti `username-kamu` dengan username GitHub kamu.

---

## 4. Error Saat git push

Pastikan kamu push ke branch yang benar.

Cek branch dengan:

```bash
git branch
```

Lalu push sesuai nama branch:

```bash
git push origin tambah-profile-nama-kamu
```

---

## 5. Lupa Membuat Branch

Jika kamu sudah terlanjur mengedit file tanpa membuat branch, tidak apa-apa.

Buat branch baru dengan:

```bash
git checkout -b tambah-profile-nama-kamu
```

Lalu lanjutkan proses commit dan push seperti biasa.

---

# Istilah Penting

| Istilah      | Penjelasan                                                   |
| ------------ | ------------------------------------------------------------ |
| Git          | Aplikasi untuk mencatat perubahan pada file project          |
| GitHub       | Website untuk menyimpan project Git secara online            |
| Repository   | Folder project yang disimpan dan dikelola dengan Git         |
| Fork         | Menyalin repository orang lain ke akun GitHub sendiri        |
| Clone        | Mengambil repository dari GitHub ke laptop                   |
| Branch       | Jalur kerja terpisah untuk mengedit project                  |
| Commit       | Menyimpan perubahan ke riwayat Git                           |
| Push         | Mengirim perubahan dari laptop ke GitHub                     |
| Pull Request | Permintaan untuk menggabungkan perubahan ke repository utama |
| Merge        | Menggabungkan Pull Request ke branch utama                   |

---

# Catatan Keamanan Data

Repository ini dapat dilihat oleh publik jika repository bersifat public.

Jangan upload data pribadi yang sensitif seperti:

* KTP
* Kartu keluarga
* Alamat rumah
* Nomor HP pribadi
* Password
* Dokumen rahasia

Cukup gunakan:

* Foto profil
* Nama
* NIM
* Program studi
* Deskripsi singkat

---

# Penutup

Jangan takut salah.

Workshop ini dibuat agar kamu bisa belajar Git dan GitHub secara langsung melalui praktik sederhana.

Jika mengalami error, tanyakan kepada mentor atau panitia workshop.

Selamat belajar dan selamat berkontribusi 🚀

````

Bagian paling penting untuk peserta pemula adalah urutan ini:

```text
Fork dulu → Clone repo hasil fork → Buat branch → Edit → Commit → Push → Pull Request
````
