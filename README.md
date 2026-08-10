[README.md](https://github.com/user-attachments/files/30887901/README.md)
<div align="center">

# MT Manager

**Satu aplikasi untuk mengatur semua terminal MetaTrader Anda.**

Scan otomatis semua MT4 & MT5 yang terpasang, kelola EA dan Indicator,
bersihkan file sampah, duplikat terminal, sampai unduh EA langsung dari link —
semuanya dari satu jendela.

[![Windows](https://img.shields.io/badge/Windows-7%20SP1%20%7C%2010%20%7C%2011-0078D6?style=flat-square&logo=windows&logoColor=white)](#-system-requirements)
[![Version](https://img.shields.io/badge/versi-1-EC3013?style=flat-square)](#)
[![Gratis](https://img.shields.io/badge/harga-gratis-5ecf3e?style=flat-square)](#)

<img src="Image/main-dark.png" alt="Tampilan utama MT Manager" width="900">

</div>

---

## Kenapa MT Manager?

Kalau Anda menjalankan lebih dari satu akun MetaTrader, pekerjaan kecil jadi
melelahkan. Mau pasang satu EA ke lima terminal? Buka folder data satu per satu.
Mau tahu kenapa disk penuh? Telusuri folder `Logs`, `Bases`, `Tester` sendiri.
Mau menambah terminal kedua dari broker yang sama? Install ulang dari awal.

MT Manager mengumpulkan semua itu ke satu tempat. Terminal Anda terdeteksi
otomatis, isinya ditampilkan rapi per kategori, dan setiap tindakan tinggal
satu klik.

---

## ✨ Fitur

### Semua terminal terdeteksi otomatis

Tekan **Scan MetaTrader** dan semua MT4/MT5 yang terpasang langsung muncul di
sidebar, dikelompokkan per jenis. Pilih salah satu untuk melihat detailnya:
nama, tipe, lokasi folder data, dan status autostart.

Isi terminal ditampilkan sebagai satu daftar rapi dengan label warna per
kategori — **Expert Advisor**, **Indicator**, **Script**, **Log**, **History**,
**Ticks**, dan **Cache** — lengkap dengan ukuran dan tanggal ubah.

<img src="Image/main-dark.png" alt="Daftar terminal dan file" width="820">

### Kelola EA & Indicator

Pasang EA atau Indicator ke terminal yang sedang dipilih tanpa perlu tahu di
folder mana file-nya harus ditaruh. Butuh menghapus? Centang beberapa file
sekaligus lalu hapus dalam satu langkah. Tersedia juga **Copy / Cut / Paste**
antar terminal — praktis untuk menyalin EA yang sama ke beberapa akun.

<img src="Image/menu-manage-ea.png" alt="Menu Manage EA / Indicator" width="820">

### Bersihkan file sampah

MetaTrader menumpuk log, data history, tick, dan cache tester yang bisa memakan
puluhan gigabyte. Menu **Utility** membersihkannya per jenis, jadi Anda bisa
memilih mana yang dibuang tanpa menyentuh EA atau setting. MetaEditor juga bisa
dibuka langsung dari sini.

<img src="Image/menu-utility.png" alt="Menu Utility" width="820">

### Install, duplikat, dan uninstall MetaTrader

<img src="Image/menu-add-remove-mt.png" alt="Menu Add / Remove MT" width="820">

**Install MetaTrader** menyediakan daftar broker siap pasang yang bisa dicari
dan difilter per MT4/MT5 — tinggal pilih, sisanya berjalan sendiri. Punya file
installer sendiri? Bisa juga dipakai lewat pilihan installer lokal.

<img src="Image/install-mt.png" alt="Jendela Install MetaTrader" width="620">

**Duplicate MetaTrader** membuat terminal kedua dari broker yang sama, lengkap
dengan progress copy dan langsung dijalankan setelah selesai. Berguna kalau
Anda punya beberapa akun di broker yang sama dan ingin tiap akun punya
terminalnya sendiri.

<img src="Image/duplicate-mt.png" alt="Jendela Duplicate MetaTrader" width="620">

### Unduh EA langsung dari link

Tempel URL (atau perintah `wget` lengkap) ke kotak **Wget Downloader**, dan
file akan diunduh dengan progress bar. File `.zip` otomatis diekstrak begitu
selesai, jadi EA langsung siap dipakai tanpa mampir ke File Explorer.

### Jalan otomatis saat komputer menyala

Setiap terminal punya sakelar **autostart** sendiri. Nyalakan, dan terminal itu
ikut jalan setiap Windows booting — cocok untuk VPS yang harus selalu online.
Saat MT Manager di-uninstall, semua entri autostart yang pernah dibuat ikut
dibersihkan otomatis.

### Tema gelap & terang

Satu klik untuk berganti tema, dan seluruh aplikasi ikut berubah seketika —
termasuk title bar-nya.

<img src="Image/main-light.png" alt="Tema terang" width="820">

### Notifikasi yang tidak mengganggu

Pemberitahuan muncul sebentar lalu hilang sendiri. Tidak ada lagi kotak dialog
yang harus ditutup manual setiap kali menyelesaikan sesuatu.

<img src="Image/toast.png" alt="Notifikasi ringan" width="820">

### Selalu versi terbaru

MT Manager memeriksa pembaruan sendiri, mengunduh, memasang, dan menjalankan
ulang dirinya — Anda cukup menekan satu tombol. Setiap versi baru datang dengan
catatan perubahan yang bisa dibaca kapan saja lewat **What's New**.

<img src="Image/whats-new.png" alt="What's New" width="620">

---

## 💻 System Requirements

| | Minimum |
|---|---|
| **Sistem operasi** | Windows 7 SP1 atau lebih baru — Windows 8, 8.1, 10, dan 11 didukung penuh (32-bit maupun 64-bit) |
| **.NET Framework** | Versi 4.8. Sudah bawaan di Windows 10 (update Mei 2019) ke atas; installer akan memberi tahu dan mengarahkan ke halaman unduhan resmi Microsoft bila belum ada |
| **MetaTrader** | MT4 dan/atau MT5 yang terpasang secara normal. Instalasi **portable** tidak terdeteksi |
| **Ruang disk** | Sekitar 10 MB untuk aplikasi |
| **RAM** | Tidak ada kebutuhan khusus — aplikasi ini ringan |
| **Hak Administrator** | **Tidak wajib.** MT Manager terpasang per-pengguna. Administrator hanya diperlukan bila Anda menduplikasi terminal yang berada di dalam `Program Files` |
| **Koneksi internet** | Diperlukan hanya untuk daftar broker, pengecekan pembaruan, dan Wget Downloader. Semua fitur lain berjalan offline |

---

## 📥 Instalasi

1. Unduh `MTManager-Setup-1.exe` dari halaman [Releases](../../releases).
2. Jalankan installer-nya, ikuti langkahnya sampai selesai.
3. Buka MT Manager, tekan **Scan MetaTrader**, dan terminal Anda langsung muncul.

Tidak perlu konfigurasi apa pun setelah instalasi.

---

## ❤️ Dukung Proyek Ini

MT Manager gratis dan bisa dipakai siapa saja. Kalau aplikasi ini membantu
pekerjaan Anda, dukungan sekecil apa pun sangat berarti untuk pengembangannya.

<img src="Image/donate.png" alt="Dialog donasi" width="480">

<div align="center">

[![Trakteer](https://img.shields.io/badge/Trakteer-EC3013?style=for-the-badge)](https://trakteer.id/dhimas_bagus4/tip)
[![Sociabuzz](https://img.shields.io/badge/Sociabuzz-EC3013?style=for-the-badge)](https://sociabuzz.com/dhimasbagus402/tribe)
[![Ko--fi](https://img.shields.io/badge/Ko--fi-EC3013?style=for-the-badge)](https://ko-fi.com/dhimasbagus)

</div>

---

## ❓ Pertanyaan Umum

**Apakah MT Manager mengubah setting atau akun trading saya?**
Tidak. MT Manager hanya mengelola file dan folder milik terminal — memasang,
menyalin, dan menghapus EA/Indicator, serta membersihkan log dan cache.
Akun, chart, dan setting trading Anda tidak disentuh.

**Kenapa terminal saya tidak muncul saat di-scan?**
MT Manager membaca terminal yang terpasang secara normal. MetaTrader yang
dijalankan dalam mode **portable** menyimpan datanya di folder aplikasi sendiri
sehingga tidak terdeteksi.

**Apakah data MetaTrader saya ikut terhapus kalau MT Manager di-uninstall?**
Tidak. Yang dibersihkan hanya milik MT Manager sendiri — pengaturan aplikasi
dan entri autostart yang pernah dibuatnya. Folder data MetaTrader tetap utuh.

**Apakah aplikasi ini berbayar?**
Tidak, gratis sepenuhnya.

---

<div align="center">
<sub>Developer? Catatan teknis, cara build, dan mekanisme update ada di
<a href="docs/DEVELOPMENT.md">docs/DEVELOPMENT.md</a>.</sub>
</div>
