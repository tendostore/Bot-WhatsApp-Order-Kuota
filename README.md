<div align="center">
  
  # 🤖 Bot WhatsApp Order Kuota (PPOB)
  
  **Script Bot WhatsApp Otomatis dengan Integrasi API Digiflazz & Terminal Control Panel**
  
  [![Node.js](https://img.shields.io/badge/Node.js-20.x-green?style=for-the-badge&logo=nodedotjs)](https://nodejs.org/)
  [![Baileys](https://img.shields.io/badge/Library-Baileys-orange?style=for-the-badge&logo=whatsapp)](https://github.com/WhiskeySockets/Baileys)
  [![Digiflazz](https://img.shields.io/badge/API-Digiflazz-blue?style=for-the-badge)](https://digiflazz.com/)
  [![PM2](https://img.shields.io/badge/Process-PM2-8B0000?style=for-the-badge&logo=pm2)](https://pm2.keymetrics.io/)

  <p align="center">
    Mudah diinstal • Sangat Ringan • Otomatisasi Penuh • Aman
  </p>
</div>

---

## 🚀 Cara Cepat Instalasi (1-Click Install)

Siapkan VPS Linux (Ubuntu/Debian) Anda. Cukup **Copy** baris kode di bawah ini, **Paste** ke terminal VPS Anda, lalu tekan **Enter**. 

Sistem akan mengunduh dan menginstal semuanya secara otomatis tanpa perlu campur tangan manual:

```bash
apt update && wget -qO install.sh https://raw.githubusercontent.com/tendostore/Bot-WhatsApp-Order-Kuota/main/install.sh && chmod +x install.sh && ./install.sh
```

## 📖 Deskripsi Proyek

**Bot WhatsApp Order Kuota** adalah solusi cerdas bisnis PPOB (Pulsa, Paket Data, Token Listrik, Voucher Game, E-Wallet, dll) yang beroperasi secara penuh di atas platform WhatsApp. Script ini dirancang untuk mengubah nomor WhatsApp Anda menjadi "Mesin Kasir Otomatis" yang siap melayani pelanggan 24 jam nonstop tanpa perlu dijaga.

Terhubung langsung secara *real-time* dengan server **Digiflazz** (salah satu *biller* PPOB terbesar di Indonesia), bot ini akan memproses setiap pesanan yang masuk secara instan, mengecek status transaksi, hingga memberikan struk atau laporan kepada pelanggan.

### 🌟 Mengapa Memilih Bot Ini?
Kebanyakan bot WhatsApp PPOB mengharuskan penggunanya mengerti bahasa pemrograman (*coding*) untuk sekadar mengubah harga atau menambah produk. **Bot ini berbeda!** Kami menghadirkan **Terminal UI Control Panel** (Panel Manajemen Berbasis Teks). Admin hanya perlu mengetik perintah `bot` di VPS, dan sebuah panel interaktif yang ramah pengguna akan muncul. Anda bisa mengelola member, mengatur harga, hingga melakukan *backup* semudah memilih menu di ATM!

---

## ⚡ Fitur Lengkap & Keunggulan

Bot ini dibekali dengan berbagai fitur mutakhir yang membedakannya dari script bot PPOB standar:

### 🔌 Integrasi Transaksi Cerdas (Digiflazz)
* **Real-time Order Processing:** Saat pelanggan mengirim format order, bot langsung meneruskannya ke API Digiflazz dalam hitungan milidetik.
* **Auto-Polling Status (Pengecekan Otomatis):** Bot secara cerdas akan memantau transaksi yang berstatus *Pending*.
* **Auto-Send SN (Serial Number):** Jika pesanan sukses, bot otomatis mengirimkan notifikasi beserta SN ke pelanggan.
* **Auto-Refund System:** Sistem anti-rugi! Jika transaksi gagal (misal: nomor salah atau gangguan *provider*), saldo pelanggan akan dikembalikan secara utuh dan otomatis.

### 💻 Terminal Control Panel (Admin CLI)
* **Zero-Coding Management:** Tambah produk, edit harga, hapus produk, hingga ganti API Key Digiflazz langsung dari panel menu terminal VPS.
* **Manajemen Saldo Member:** Tambah (Top-Up) atau kurangi saldo pelanggan cukup dengan memasukkan ID WhatsApp mereka.
* **Proses Instalasi Mandiri:** Script secara otomatis menginstal `Node.js`, mengurus *dependencies*, dan menyetting *daemon* aplikasi latar belakang.

### 👥 Sistem Database & Membership Lokal
* **Database Super Ringan (JSON):** Tidak membutuhkan instalasi *database* berat seperti MySQL atau MongoDB. Cocok untuk VPS dengan spesifikasi rendah (RAM 1GB).
* **Auto-Registration:** Pelanggan yang baru pertama kali *chat* akan otomatis terdaftar di *database* dengan ID unik.
* **Fitur Katalog & Saldo:** Pelanggan dapat mengecek sisa saldo dan melihat katalog harga secara *real-time*.

### 🛡️ Keamanan, Stabilitas & Maintenance
* **Login via Pairing Code:** Ucapkan selamat tinggal pada *QR Code* yang sering gagal! Bot menggunakan sistem kode tautan 8 digit dari Baileys terbaru. Lebih aman, stabil, dan jarang *logout* sendiri.
* **PM2 Background Daemon:** Bot dijaga oleh PM2. Jika server di-*restart* atau terjadi *error*, bot akan otomatis menyala kembali (Auto-Restart 24/7).
* **Auto-Backup ke Telegram:** Konfigurasi dan *database* Anda sangat berharga. Bot akan membungkus file data menjadi `.zip` yang bersih dan mengirimkannya ke chat Telegram Anda setiap 12 Jam secara otomatis (tersedia juga opsi *backup* manual).
* **Direct Link Restore:** Pindah VPS? Cukup *paste* link file `.zip` *backup* Anda, dan sistem akan memulihkan seluruh data bot Anda dalam hitungan detik!
* **Pesan Broadcast:** Fitur ampuh untuk mengirimkan pengumuman atau promo langsung ke ribuan *database* nomor pelanggan Anda.

---

## ⚙️ Panduan Setup Awal

Setelah menu instalasi terbuka di terminal, ikuti urutan berikut agar bot berjalan sempurna:

1. Pilih **Menu 1** `(Install & Buat File Bot Otomatis)`. Biarkan sistem menginstal *library* secara *silent*.
2. Pilih **Menu 10** `(Ganti API Digiflazz)`. Masukkan Username dan Production API Key Digiflazz Anda.
3. Pilih **Menu 2** `(Mulai Bot)`. Masukkan nomor WA bot Anda. Buka WhatsApp di HP, pilih "Perangkat Tertaut", lalu masukkan Kode Pairing yang muncul di layar terminal.
4. Tekan `CTRL + C` untuk menghentikan bot sementara.
5. Pilih **Menu 3** `(Jalankan Bot di Latar Belakang)`. Selesai! Bot kini aktif 24 jam nonstop.

> 💡 **TIPS SANGAT PENTING:** <br>Untuk membuka panel kontrol admin di lain waktu, Anda tidak perlu repot mengetik perintah yang panjang atau mencari direktori instalasi. Cukup ketik **`bot`** di terminal VPS Anda lalu tekan `Enter`!

---

## 📱 Daftar Perintah WhatsApp (Untuk Pelanggan)

| Perintah | Fungsi | Contoh Penggunaan |
| :--- | :--- | :--- |
| `bot` | Menampilkan menu bantuan dan informasi ID Member. | `bot` |
| `.saldo` | Mengecek sisa saldo lokal member. | `.saldo` |
| `.harga` | Melihat katalog produk dan harga yang tersedia. | `.harga` |
| `.order` | Membeli produk (Format: `.order [kode] [tujuan]`) | `.order E15GB 081234567890` |

---

## 🎛️ Cuplikan Menu Panel Admin (Ketik: `bot`)

```text
===============================================
      🤖 PANEL PENGELOLA TENDO STORE 🤖      
===============================================
--- MANAJEMEN BOT ---
1. Install & Buat File Bot Otomatis
2. Mulai Bot (Terminal)
3. Jalankan Bot di Latar Belakang (PM2)
4. Hentikan Bot (PM2)
5. Lihat Log / Error Bot

--- MANAJEMEN TOKO & SISTEM ---
6. 👥 Manajemen Member (Saldo)
7. 🛒 Manajemen Produk (Harga)
8. ⚙️ Bot Telegram Setup (Auto-Backup)
9. 💾 Backup & Restore Data
10. 🔌 Ganti API Digiflazz
11. 🔄 Ganti Akun Bot WA (Reset Sesi)
12. 📢 Kirim Pesan Broadcast
0. Keluar
===============================================
