# Sistem Manajemen Fasilitas Kesehatan

Aplikasi manajemen fasilitas kesehatan berbasis web yang dirancang untuk memenuhi kebutuhan layanan kesehatan di fasilitas kesehatan tingkat pertama. Sistem ini menyediakan antarmuka yang intuitif untuk manajemen pasien, antrian, farmasi, dan integrasi dengan SATUSEHAT.

## Fitur Utama

### 1. Manajemen Pengguna
- Multi-role user (Frontline, Dokter, Perawat, Apoteker, Kasir, Keuangan)
- Autentikasi dan otorisasi berbasis peran
- Antarmuka yang responsif dengan dukungan mode gelap/terang

### 2. Manajemen Pasien
- Pendaftaran pasien baru
- Pencarian dan pengelolaan data pasien
- Integrasi dengan SATUSEHAT untuk sinkronisasi data pasien

### 3. Sistem Antrian
- Antrian real-time dengan WebSocket
- Prioritas antrian
- Status dan pembaruan antrian secara langsung

### 4. Manajemen Farmasi
- Inventaris obat
- Pemantauan stok
- Pencatatan transaksi farmasi

### 5. Pembayaran dan Keuangan
- Pencatatan pembayaran
- Laporan keuangan harian
- Pemantauan transaksi

### 6. Integrasi SATUSEHAT
- Konfigurasi kredensial SATUSEHAT
- Sinkronisasi data pasien
- Pertukaran data kesehatan sesuai standar FHIR

## Teknologi

- **Frontend**: React, TailwindCSS, shadcn/ui
- **Backend**: Express.js
- **Database**: PostgreSQL (via Drizzle ORM)
- **Real-time**: WebSocket
- **Autentikasi**: Passport.js
- **API Integration**: SATUSEHAT FHIR API

## Instalasi dan Penggunaan

1. Clone repositori
2. Install dependensi:
```bash
npm install
```

3. Konfigurasi environment variables:
```env
SESSION_SECRET=your_session_secret
DATABASE_URL=your_database_url
```

4. Jalankan aplikasi:
```bash
npm run dev
```

5. Buka aplikasi di browser:
```
http://localhost:5000
```

## Konfigurasi SATUSEHAT

1. Dapatkan kredensial SATUSEHAT:
   - Client ID
   - Client Secret
   - Organization ID

2. Masuk ke sistem sebagai admin
3. Buka menu Pengaturan
4. Masukkan kredensial SATUSEHAT
5. Simpan konfigurasi

## Lisensi

MIT License

habizinnia@gmail.com