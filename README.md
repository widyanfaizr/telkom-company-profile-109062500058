#
Telkom University Company Profile - Praktikum

Project simulasi HTML, CSS, PHP native, MySQL/MariaDB, dan Git.

# Telkom University Company Profile — Praktikum Git & PHP Native

![Git](https://img.shields.io/badge/Git-Version%20Control-F05032?logo=git&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-Native-777BB4?logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-Database-4479A1?logo=mysql&logoColor=white)
![Release](https://img.shields.io/badge/Release-v1.0.0-blue)

Repository ini berisi proyek simulasi web **Company Profile Telkom University** yang dibangun menggunakan HTML, CSS, PHP Native, dan MySQL/MariaDB[cite: 56, 57]. Proyek ini dirancang sebagai sarana praktikum alur kerja *Version Control System* menggunakan **Git** dan **GitHub**[cite: 56, 57].

> **Catatan:** Seluruh konten institusi pada proyek ini bersifat simulasi untuk keperluan pembelajaran dan praktikum[cite: 57, 78].

---

## Fitur Utama
- **Beranda Dinamis**: Menampilkan ringkasan program studi dan highlight berita[cite: 71, 81].
- **Program Studi**: Menampilkan daftar program studi secara dinamis dari database[cite: 71, 80].
- **Berita & Detail Berita**: Fitur baca berita lengkap menggunakan URL parameter dan *Prepared Statement*[cite: 71, 84, 85].
- **Form Kontak**: Mengirim pesan dengan metode `POST` dan *Prepared Statement*[cite: 71, 86, 87].
- **Simulasi Admin**: Form tambah berita lokal[cite: 71, 88].

---

## Tech Stack & Prasyarat
- **Bahasa & Library**: PHP Native (MySQLi), HTML5, CSS3[cite: 56, 57, 80].
- **Database**: MySQL / MariaDB[cite: 56, 57].
- **Web Server**: Apache via XAMPP[cite: 57, 64].
- **Version Control**: Git & GitHub[cite: 56, 57].
- **Code Editor**: Visual Studio Code[cite: 57, 63].

---

## Struktur Folder Proyek
```text
telkom-company-profile/
├── assets/
│   └── css/
│       └── style.css          # Stylesheet utama aplikasi
├── config/
│   └── database.php           # Koneksi ke database MySQL
├── database/
│   └── telkom_profile.sql     # Schema dan seed data awal
├── includes/
│   ├── header.php             # Navigasi & elemen header bersama
│   └── footer.php             # Elemen footer bersama
├── admin/
│   ├── add_news.php           # Form input berita (lokal)
│   └── save_news.php          # Proses simpan berita
├── index.php                  # Halaman utama (Beranda)
├── profile.php                # Halaman profil institusi
├── programs.php               # Halaman daftar program studi
├── news.php                   # Halaman daftar berita
├── news_detail.php            # Halaman detail berita
├── contact.php                # Form pesan kontak
└── contact_process.php        # Proses simpan pesan kontak
```[cite: 72]

---

##  Panduan Instalasi Cepat

### 1. Persiapan Server Lokal
1. Pastikan **XAMPP** sudah terinstal dan buka **XAMPP Control Panel**[cite: 64].
2. Buka terminal/command line, lalu salin (*clone*) repository ini ke folder `htdocs` XAMPP Anda:
   ```bash
   cd C:\xampp\htdocs
   git clone [https://github.com/USERNAME/telkom-company-profile.git](https://github.com/USERNAME/telkom-company-profile.git)
   ```[cite: 70, 72]
3. Jalankan service **Apache** dan **MySQL** pada XAMPP Control Panel[cite: 64, 73].

### 2. Import Database
1. Buka browser dan akses **[http://localhost/phpmyadmin/](http://localhost/phpmyadmin/)**[cite: 64, 73].
2. Buat database baru bernama `telkom_profile`[cite: 73].
3. Pilih tab **SQL** atau **Import**, lalu jalankan file script `database/telkom_profile.sql` yang ada di dalam proyek[cite: 73, 102].

### 3. Jalankan Proyek
Buka browser dan akses URL berikut:
```text
http://localhost/telkom-company-profile
```[cite: 102]

---

##  Konvensi Git Commit
Proyek ini menerapkan standar pesan *commit* terstruktur berbasis *Conventional Commits*:
- `feat:` untuk penambahan fitur baru (contoh: `feat: hubungkan database dan tampilkan program studi`)[cite: 62, 83]
- `fix:` untuk perbaikan bug (contoh: `fix: validasi id berita sebelum query`)[cite: 62]
- `docs:` untuk pembaruan dokumentasi (contoh: `docs: inisialisasi README`)[cite: 62, 73]
- `style:` untuk perubahan tampilan atau CSS (contoh: `style: rapikan tampilan navbar responsif`)[cite: 62]
- `chore:` untuk pemeliharaan konfigurasi dan setup (contoh: `chore: tambahkan gitignore`)[cite: 62, 69]

---

##  Penulis & Pengembang
* **Nama**: Widyan Faiz Rabbani
* **Institusi**: Telkom University Purwokerto

---
*Dibuat untuk memenuhi tugas dan panduan praktikum modul Git, GitHub, PHP Native, & MySQL.*[cite: 56, 57]