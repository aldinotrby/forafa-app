# forafa-app
Forafa merupakan platform forum percakapan pihak kedua untuk keperluan jual beli sebagai reseller atau tangan kedua yang menjual produk digital ke pengguna atau pihak ketiga, untuk keperluan memberikan kode masuk/login kedalam suatu produk digital tanpa melalui reseller atau pihak kedua.

Tentu. Aku buatkan README.md yang cocok untuk repository GitHub, dengan penjelasan konsep, alur pengguna, fitur, teknologi, dan struktur sistem. Aku juga akan menjaga istilah reseller, maker, dan user supaya konsep tangan kedua yang kamu maksud tetap jelas.

# Forafa App
Forafa App adalah platform forum percakapan sementara yang dibuat untuk membantu reseller produk digital menghubungkan pengguna dengan maker atau penyedia produk digital secara langsung, khususnya ketika pengguna membutuhkan kode verifikasi, kode login, atau kode akses.
Forafa berperan sebagai **pihak ketiga berbasis forum** yang mempertemukan User dan Maker tanpa memperlihatkan identitas satu sama lain.
## Konsep
Dalam transaksi produk digital, terdapat tiga pihak:
- **Maker**: Pihak yang menyediakan atau membuat produk digital.
- **Reseller**: Pihak kedua yang membeli produk dari Maker dan menjualnya kembali kepada User.
- **User**: Pembeli atau pengguna akhir produk digital.
Contoh:
> Reseller membeli akses ChatGPT dari Maker, kemudian menjual akses tersebut kepada User.
Ketika User ingin login, terkadang sistem membutuhkan kode verifikasi.
Tanpa Forafa:
```text
User
  ↓
Meminta kode kepada Reseller
  ↓
Reseller meminta kode kepada Maker
  ↓
Maker memberikan kode kepada Reseller
  ↓
Reseller memberikan kode kepada User

Proses tersebut dapat menjadi tidak efisien apabila ketiga pihak tidak sedang online secara bersamaan.

Dengan Forafa:

User
  ↓
Forum Forafa
  ↓
Maker
  ↓
Memberikan kode

Reseller tidak perlu menjadi perantara dalam setiap permintaan kode.

⸻

Tujuan

Forafa dibuat untuk mengurangi ketergantungan komunikasi antara Reseller dan User ketika User membutuhkan kode login atau kode akses dari Maker.

Tujuan utama Forafa:

* Mempermudah User meminta kode secara langsung kepada Maker.
* Mengurangi beban Reseller dalam meneruskan permintaan kode.
* Mengatasi masalah perbedaan waktu online antara User, Reseller, dan Maker.
* Menyediakan ruang komunikasi sementara.
* Menjaga identitas User dan Maker tetap tersembunyi.
* Membuat forum yang dapat digunakan tanpa proses pendaftaran bagi User dan Maker.

⸻

Cara Kerja

1. Reseller Membuat Akun

Reseller melakukan pendaftaran dan login ke Forafa.

Setelah berhasil masuk, Reseller dapat membuat forum baru.

2. Reseller Membuat Forum

Reseller membuat sebuah forum percakapan untuk produk atau transaksi tertentu.

Setiap forum akan menghasilkan sebuah link khusus.

Contoh:

https://forafa.example/forum/8xK92Lm

Link tersebut kemudian diberikan kepada:

* User
* Maker

3. User dan Maker Masuk ke Forum

User dan Maker cukup membuka link forum.

Mereka tidak perlu membuat akun.

Identitas mereka tidak ditampilkan kepada satu sama lain.

Contohnya:

User:
"Minta kode min"
Maker:
"123456"
User:
"Terima kasih"

Reseller tetap dapat melihat percakapan tersebut tanpa harus ikut aktif berkomunikasi.

4. Forum Berakhir

Setiap forum aktif selama 24 jam sejak dibuat.

Setelah 24 jam, forum tidak dapat digunakan kembali.

Reseller juga dapat menghapus forum kapan saja sebelum masa aktif berakhir.

⸻

Privasi Identitas

Salah satu konsep utama Forafa adalah menyembunyikan identitas antara User dan Maker.

User

User:

* Tidak memiliki profil.
* Tidak perlu membuat akun.
* Tidak mengetahui identitas Maker.
* Tidak mengetahui identitas Reseller.
* Hanya dapat mengakses forum melalui link.

Maker

Maker:

* Tidak memiliki profil.
* Tidak perlu membuat akun.
* Tidak mengetahui identitas User.
* Tidak mengetahui identitas Reseller.
* Hanya dapat mengakses forum melalui link.

Reseller

Reseller merupakan satu-satunya pihak yang mengetahui konteks hubungan antara User dan Maker.

Reseller:

* Memiliki akun.
* Dapat membuat forum.
* Mendapatkan link forum.
* Dapat membagikan link kepada User dan Maker.
* Dapat melihat percakapan.
* Dapat ikut mengirim pesan.
* Dapat menghapus forum.

⸻

Alur Sistem

                    FORAFA APP
                        │
                        │
                  Reseller Login
                        │
                        ▼
                 Membuat Forum
                        │
                        ▼
                  Link Forum
                        │
             ┌──────────┴──────────┐
             │                     │
             ▼                     ▼
           User                   Maker
       Tanpa akun              Tanpa akun
             │                     │
             └──────────┬──────────┘
                        │
                        ▼
                 Forum Percakapan
                        │
                        ▼
              User meminta kode
                        │
                        ▼
                Maker memberikan kode
                        │
                        ▼
                    Selesai

⸻

Contoh Penggunaan

Misalnya Reseller menjual akses sebuah produk digital kepada User.

User mendapatkan link forum dari Reseller.

User:
Min, minta kode login.
Maker:
Siap, kodenya 839201.
User:
Sudah, terima kasih.

Reseller tidak perlu meneruskan pesan:

User → Reseller → Maker

karena komunikasi dapat berlangsung langsung melalui forum:

User → Forum → Maker

Dengan demikian, Reseller tidak harus online bersamaan dengan User dan Maker.

⸻

Masa Aktif Forum

Setiap forum memiliki masa aktif selama:

24 Jam

Setelah masa aktif berakhir:

Forum
  ↓
Expired
  ↓
Tidak dapat digunakan

Reseller juga memiliki kontrol untuk menghapus forum secara manual sebelum 24 jam berakhir.

Reseller
    │
    ▼
Hapus Forum
    │
    ▼
Forum Tidak Dapat Diakses

⸻

Fitur Utama

Reseller

* Registrasi akun
* Login
* Logout
* Membuat forum
* Mendapatkan link forum
* Melihat forum yang dibuat
* Melihat percakapan
* Ikut mengirim pesan
* Menghapus forum
* Melihat status forum
* Forum otomatis kedaluwarsa setelah 24 jam

User

* Mengakses forum melalui link
* Tidak perlu registrasi
* Tidak perlu login
* Mengirim pesan
* Menerima pesan dari Maker
* Identitas tidak ditampilkan

Maker

* Mengakses forum melalui link
* Tidak perlu registrasi
* Tidak perlu login
* Mengirim pesan
* Menerima pesan dari User
* Identitas tidak ditampilkan

⸻

Teknologi

Forafa App dibangun menggunakan teknologi sederhana agar mudah dikembangkan dan dijalankan.

Backend

* PHP Native

Database

* MySQL

Frontend

* HTML5
* CSS3
* JavaScript

⸻

Arsitektur Sederhana

┌───────────────────────────┐
│           User            │
│      Tanpa Registrasi     │
└─────────────┬─────────────┘
              │
              │
              ▼
┌───────────────────────────┐
│        Forafa App         │
│                           │
│      Forum Percakapan     │
└─────────────┬─────────────┘
              │
              │
              ▼
┌───────────────────────────┐
│           Maker           │
│      Tanpa Registrasi     │
└───────────────────────────┘
              ▲
              │
              │
       ┌──────┴──────┐
       │  Reseller   │
       │  Controller │
       └─────────────┘

⸻

Konsep Identitas

Forafa tidak menggunakan sistem profil untuk User dan Maker.

Identitas dapat direpresentasikan menggunakan label sederhana dalam forum.

Contoh:

User:
Minta kode min.
Maker:
Kodenya 123456.

Tidak ada informasi seperti:

Nama:
Username:
Foto profil:
Email:
Nomor telepon:

yang ditampilkan kepada pihak lain.

Reseller tetap dapat mengakses forum karena Reseller merupakan pemilik forum.

⸻

Struktur Data

Secara sederhana, sistem dapat menggunakan beberapa tabel utama:

users
├── id
├── name
├── email
├── password
└── created_at
forums
├── id
├── reseller_id
├── forum_token
├── created_at
├── expires_at
└── status
messages
├── id
├── forum_id
├── sender_type
├── message
└── created_at

sender_type dapat digunakan untuk membedakan pengirim pesan:

user
maker
reseller

Sedangkan forum_token digunakan sebagai identitas unik forum pada URL.

Contoh:

/forum/8xK92Lm

⸻

Keamanan

Karena forum dapat diakses menggunakan link, sistem perlu memperhatikan keamanan akses.

Beberapa mekanisme yang dapat diterapkan:

* Menggunakan token forum yang sulit ditebak.
* Tidak menggunakan ID forum secara langsung pada URL.
* Menggunakan prepared statement untuk query database.
* Melakukan validasi input.
* Melakukan escaping output untuk mencegah XSS.
* Menggunakan password hashing untuk akun Reseller.
* Memberikan batas panjang pesan.
* Menghapus atau menonaktifkan forum yang sudah expired.
* Menggunakan session yang aman untuk akun Reseller.

Contoh token:

/forum/8xK92LmP4qT7

lebih aman dibandingkan:

/forum/1
/forum/2
/forum/3

karena ID berurutan lebih mudah ditebak.

⸻

Struktur Folder

Contoh struktur project:

forafa-app/
│
├── assets/
│   ├── css/
│   │   └── style.css
│   │
│   ├── js/
│   │   └── app.js
│   │
│   └── images/
│
├── config/
│   └── database.php
│
├── auth/
│   ├── login.php
│   ├── register.php
│   └── logout.php
│
├── reseller/
│   ├── dashboard.php
│   ├── create-forum.php
│   ├── forums.php
│   └── delete-forum.php
│
├── forum/
│   ├── index.php
│   ├── send-message.php
│   └── messages.php
│
├── includes/
│   ├── header.php
│   ├── footer.php
│   └── auth.php
│
├── index.php
├── .htaccess
└── README.md

Struktur tersebut dapat berubah sesuai kebutuhan pengembangan aplikasi.

⸻

Instalasi

1. Clone Repository

git clone https://github.com/username/forafa-app.git

Masuk ke folder project:

cd forafa-app

2. Jalankan Web Server

Forafa menggunakan PHP Native dan MySQL.

Project dapat dijalankan menggunakan:

* Laragon
* XAMPP
* Apache + PHP + MySQL

Jika menggunakan Laragon, letakkan project di:

C:\laragon\www\forafa-app

Kemudian jalankan:

Apache
MySQL

3. Buat Database

Buat database MySQL:

CREATE DATABASE forafa_db;

Kemudian import struktur database yang tersedia pada folder:

database/

4. Konfigurasi Database

Sesuaikan konfigurasi database pada:

config/database.php

Contoh:

$host = "localhost";
$dbname = "forafa_db";
$username = "root";
$password = "";

5. Jalankan Aplikasi

Buka:

http://localhost/forafa-app

⸻

Roadmap

Pengembangan Forafa dapat dilakukan secara bertahap.

MVP

* [x]	Konsep forum sementara
* [ ]	Registrasi Reseller
* [ ]	Login Reseller
* [ ]	Dashboard Reseller
* [ ]	Membuat forum
* [ ]	Generate link forum
* [ ]	User masuk melalui link
* [ ]	Maker masuk melalui link
* [ ]	Chat User ↔ Maker
* [ ]	Reseller dapat melihat chat
* [ ]	Forum aktif 24 jam
* [ ]	Reseller dapat menghapus forum

Pengembangan Berikutnya

* [ ]	Auto-expired forum
* [ ]	Countdown masa aktif forum
* [ ]	Notifikasi pesan baru
* [ ]	Auto-refresh pesan
* [ ]	AJAX untuk chat real-time
* [ ]	Rate limiting
* [ ]	Anti-spam
* [ ]	Moderasi pesan
* [ ]	Sistem laporan forum
* [ ]	Riwayat forum Reseller
* [ ]	Statistik penggunaan forum

⸻

Prinsip Utama Forafa

Forafa dibangun dengan konsep sederhana:

Reseller membuat forum
        ↓
Reseller membagikan link
        ↓
User masuk
        +
Maker masuk
        ↓
User meminta kode
        ↓
Maker memberikan kode
        ↓
Selesai

Reseller tidak perlu menjadi penghubung aktif dalam setiap permintaan kode.

Forafa hanya menyediakan ruang komunikasi sementara untuk mempercepat proses tersebut.

⸻

Status Project

Status: Development

Forafa App masih dalam tahap pengembangan dan dapat mengalami perubahan pada fitur, struktur database, maupun arsitektur aplikasi.

⸻

License

License project dapat ditentukan sesuai kebutuhan pengembang.

Menurutku konsep utamanya sudah cukup kuat untuk dijadikan README karena **masalah → solusi → alur → aktor → teknologi** terlihat jelas. Yang paling penting, README ini tidak menggambarkan Forafa sebagai marketplace, tetapi sebagai **temporary communication bridge** antara User dan Maker yang dikendalikan oleh Reseller.
