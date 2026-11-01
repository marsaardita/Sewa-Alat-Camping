# Sewa Alat Camping

Aplikasi web untuk membantu proses penyewaan alat camping, mulai dari pengelolaan data barang dan pelanggan hingga pencatatan transaksi penyewaan.

## Fitur

- **Dashboard** — halaman ringkasan aplikasi.
- **Login dan registrasi** — autentikasi pengguna.
- **Data barang** — pengelolaan data perlengkapan camping.
- **Data pelanggan** — pengelolaan informasi pelanggan.
- **Transaksi penyewaan** — pencatatan transaksi penyewaan barang.
- **Struk transaksi** — menampilkan struk transaksi.

> Catatan: Daftar fitur ini disusun berdasarkan struktur halaman dan endpoint yang tersedia pada source code. Detail alur dan hak akses dapat disesuaikan lagi dengan implementasi aplikasi.

## Teknologi

### Frontend
- React
- Vite
- Tailwind CSS

### Backend
- PHP
- MySQLi

### Database
- MySQL

## Struktur Folder

```text
Sewa_Alat_Camping/
├── Backend/
│   ├── api/
│   ├── config/
│   ├── .env.example
│   ├── .htaccess
│   └── index.php
├── Frontend/
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── layout/
│   │   └── pages/
│   ├── .env.example
│   ├── package.json
│   └── vite.config.js
├── .gitignore
└── README.md
```

## Persiapan

Pastikan perangkat sudah memiliki:
- [XAMPP](https://www.apachefriends.org/) atau lingkungan lokal lain yang menyediakan Apache dan MySQL.
- [Node.js](https://nodejs.org/).
- Git (opsional, untuk mengambil source code).

## Cara Menjalankan

### 1. Clone repository

```bash
git clone https://github.com/marsaardita/Sewa-Alat-Camping.git
cd Sewa-Alat-Camping
```

Jika source code sudah tersedia secara lokal, lewati langkah ini.

### 2. Jalankan backend

1. Letakkan folder proyek di direktori `htdocs` XAMPP.
2. Jalankan Apache dan MySQL melalui XAMPP Control Panel.
3. Buat database MySQL dengan nama `sewa_alat_camping`.
4. Siapkan tabel database sesuai struktur yang digunakan aplikasi.
5. Salin `Backend/.env.example` menjadi `Backend/.env`.
6. Sesuaikan konfigurasi database di `Backend/.env`:

```env
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=
DB_NAME=sewa_alat_camping
DB_PORT=3306
```

Sesuaikan `DB_USER` dan `DB_PASSWORD` dengan konfigurasi MySQL lokal.

### 3. Jalankan frontend

Buka terminal pada folder `Frontend`, kemudian jalankan:

```bash
cd Frontend
npm install
```

Salin `Frontend/.env.example` menjadi `Frontend/.env`, lalu sesuaikan alamat API jika lokasi backend berbeda:

```env
VITE_URL_API=http://localhost/Sewa_Alat_Camping/Backend
```

Jalankan development server:

```bash
npm run dev
```

Buka alamat lokal yang ditampilkan oleh Vite di terminal.

## Konfigurasi Environment

File `.env` digunakan untuk konfigurasi lokal dan tidak disertakan dalam repository. Gunakan file `.env.example` sebagai template, lalu sesuaikan nilainya dengan lingkungan masing-masing.

Jangan mengunggah password, token, atau kredensial pribadi ke repository publik.

## Catatan

- Repository ini berisi source code aplikasi untuk keperluan pembelajaran dan portofolio.
- File dump/database SQL belum disertakan pada repository ini. Database perlu disiapkan sesuai struktur tabel yang digunakan aplikasi sebelum dijalankan.
- Aplikasi dijalankan di lingkungan lokal; repository ini tidak menyediakan deployment.

## Repository

[github.com/marsaardita/Sewa-Alat-Camping](https://github.com/marsaardita/Sewa-Alat-Camping)
