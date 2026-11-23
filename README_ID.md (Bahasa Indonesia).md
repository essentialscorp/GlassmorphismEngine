<div align="center">

  <!-- PLACEHOLDER BANNER / LOGO PROYEK -->
  <img src="assets/banner.png" alt="LiquidGlass LSPosed Banner" width="100%" />

  # LiquidGlass untuk WhatsApp & Instagram (Modul LSPosed)

  **Ubah tampilan WhatsApp & Instagram di perangkat Samsung Anda menjadi estetika LiquidGlass yang elegan dan modern secara dinamis—tanpa memodifikasi file APK asli.**

  [![Android](https://img.shields.io/badge/Android-16%2B-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://www.android.com/)
  [![Device](https://img.shields.io/badge/Samsung-Rooted-1428A0?style=for-the-badge&logo=samsung&logoColor=white)](https://www.samsung.com/)
  [![LSPosed API](https://img.shields.io/badge/LSPosed%20API-101%20--%20103-blue?style=for-the-badge)](https://github.com/LSPosed/LSPosed)
  [![WhatsApp](https://img.shields.io/badge/WhatsApp-Dukungan%20Beta-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://www.whatsapp.com/)
  [![Instagram](https://img.shields.io/badge/Instagram-Segera%20Hadir-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/)
  [![License](https://img.shields.io/badge/License-GPLv3-orange?style=for-the-badge)](LICENSE)

  <p align="center">
    <a href="README.md">🇺🇸 English</a> •
    <a href="README_ID.md">🇮🇩 Bahasa Indonesia</a> •
    <a href="README_ES.md">🇪🇸 Español</a>
  </p>

</div>

---

## 📖 Penjelasan Proyek

**LiquidGlass** adalah modul Xposed/LSPosed tingkat lanjut yang dirancang khusus untuk perangkat Samsung yang sudah di-*root* pada versi Android terbaru. Dengan melakukan *hooking* langsung ke jalur rendering antarmuka (UI) aplikasi secara *runtime*, modul ini menerapkan efek **blur transparan real-time, glassmorphism, dan refraksi cairan** (LiquidGlass) pada **WhatsApp** (saat ini tahap Beta) dan **Instagram** (segera hadir).

Karena bekerja sepenuhnya melalui metode *Xposed hooking*, **tidak diperlukan modifikasi APK (patching), repackaging, maupun clone aplikasi**. Aplikasi Anda tetap 100% original, aman dari risiko *banned* mod, dan tetap bisa mendapatkan pembaruan resmi langsung dari Google Play Store.

---

## 🎬 Pratinjau (Preview)

> *Ganti path gambar di bawah ini dengan file `.gif` atau `.mp4` Anda sendiri di dalam folder `assets/` pada repositori ini.*

<div align="center">
  <table>
    <tr>
      <td align="center"><b>WhatsApp (Beta)</b></td>
      <td align="center"><b>Instagram (Segera Hadir)</b></td>
    </tr>
    <tr>
      <td><img src="assets/preview_whatsapp.gif" alt="Pratinjau WhatsApp LiquidGlass" width="320"/></td>
      <td><img src="assets/preview_instagram.gif" alt="Pratinjau Instagram LiquidGlass" width="320"/></td>
    </tr>
  </table>
</div>

---

## ✨ Fitur Utama & Roadmap

- **Tanpa Modifikasi APK:** Melakukan *hook* langsung pada *View* UI saat aplikasi berjalan; mempertahankan tanda tangan digital (signature) asli aplikasi.
- **Blur Dinamis Real-Time:** Latar belakang transparan dengan akselerasi perangkat keras (*hardware-accelerated*) serta pengaturan radius blur, opasitas warna, dan lengkungan sudut.
- **Integrasi WhatsApp (🧪 Beta):** Menerapkan latar obrolan transparan, bilah navigasi/atas *frosted glass*, dan *modal* kaca pada versi WhatsApp Global terbaru.
- **Integrasi Instagram (⏳ Segera Hadir):** Dukungan tampilan kaca transparan untuk beranda Instagram, DM, dan bilah navigasi sedang dalam tahap pengembangan aktif.
- **Ringan & Hemat Baterai:** Menggunakan API `RenderEffect` bawaan Android dan API blur khusus Samsung untuk menjamin kelancaran animasi tanpa *frame drop*.

---

## 📱 Perangkat yang Didukung & Spesifikasi Sistem

Untuk memastikan performa dan stabilitas maksimal, pastikan perangkat Anda memenuhi persyaratan berikut:

| Komponen | Persyaratan / Kompatibilitas |
| :--- | :--- |
| **Merek Perangkat** | Perangkat Samsung Galaxy Rooted (Seri S, Z, Note, dan Seri A) |
| **Versi OS** | **Android 16+** (OneUI 8.0 / 8.1 atau lebih baru) |
| **Solusi Root** | Magisk (v27+), KernelSU, atau APatch |
| **Framework** | **LSPosed** (Zygisk / NeoZygisk) yang mendukung **API 101 – 103** |
| **Aplikasi Target** | **WhatsApp (Global Terbaru - Beta)** & **Instagram (Segera Hadir)** |

> **⚠️ Catatan:** Perangkat non-Samsung atau Custom ROM berbasis AOSP **tidak didukung secara resmi**, karena modul ini memanfaatkan API rendering blur bawaan Samsung.

---

## 🚀 Cara Penggunaan & Instalasi

1. **Prasyarat:** Pastikan perangkat Samsung Anda sudah di-*root* dan memiliki **LSPosed (API 101–103)** yang aktif.
2. **Unduh:** Unduh file `LiquidGlass-vX.X.apk` versi terbaru dari halaman [Releases](../../releases).
3. **Instal:** Instal file APK yang telah diunduh seperti menginstal aplikasi biasa.
4. **Aktifkan Modul:**
   - Buka aplikasi **LSPosed Manager**.
   - Masuk ke tab **Modul (Modules)** dan aktifkan **LiquidGlass**.
   - Pada daftar cakupan (*Scope*), centang **WhatsApp** *(serta **Instagram** setelah dukungan dirilis)*.
5. **Terapkan Perubahan:**
   - Lakukan **Paksa Berhenti (Force Stop)** pada aplikasi WhatsApp melalui pengaturan perangkat, lalu buka kembali untuk melihat efek LiquidGlass.
6. **Kustomisasi (Opsional):** Buka aplikasi pendamping **LiquidGlass** dari laci aplikasi untuk mengatur intensitas blur, warna kaca, dan efek garis tepi.

---

## 🛠️ Pemecahan Masalah (Troubleshooting)

<details>
<summary><b>1. Efek LiquidGlass tidak muncul di WhatsApp.</b></summary>
<br>
- Pastikan **WhatsApp** sudah dicentang di dalam menu **Scope Modul LSPosed**.
- Pastikan Anda telah melakukan **Force Stop (Paksa Berhenti)** pada WhatsApp setelah mengaktifkan modul.
- Periksa apakah framework LSPosed Anda berjalan pada **API 101 hingga 103**. Versi LSPosed lama tidak dapat melakukan *hook* pada sistem UI Android 16+.
</details>

<details>
<summary><b>2. WhatsApp tiba-tiba Force Close (Crash) atau tampilan berantakan setelah update dari Play Store (Catatan Beta).</b></summary>
<br>
- Karena dukungan WhatsApp saat ini masih berstatus **Beta** dan WhatsApp sering mengubah struktur kelas internalnya pada pembaruan baru, update versi Global terbaru terkadang dapat memutus *hook*. Jika terjadi *crash*, hilangkan centang WhatsApp sementara di Scope LSPosed dan periksa pembaruan modul di halaman [Releases](../../releases).
</details>

<details>
<summary><b>3. Terjadi lag atau patah-patah (frame drop) saat menggulir obrolan.</b></summary>
<br>
- Buka aplikasi pengaturan **LiquidGlass** dan turunkan nilai **Radius Blur** atau matikan fitur **Refraksi Real-time** (khususnya untuk GPU seri Galaxy A kelas menengah).
- Pastikan opsi *Nonaktifkan overlay HW (Disable HW Overlays)* dalam keadaan **mati** di Opsi Pengembang Android.
</details>

<details>
<summary><b>4. Muncul peringatan "LSPosed API Mismatch" atau modul gagal dimuat.</b></summary>
<br>
- Modul ini dikompilasi khusus untuk **LSPosed API 101–103** pada Android 16+. Silakan perbarui versi Zygisk dan LSPosed Anda ke rilis terbaru yang kompatibel.
</details>

---

## 🤝 Kontribusi & Laporan Bug

Kontribusi, saran fitur, dan laporan masalah sangat kami hargai!
- Menemukan *bug* pada WhatsApp Beta? Silakan buat [Issue](../../issues) baru dan lampirkan **Log LSPosed** beserta detail **Tipe Perangkat, Versi OneUI, dan Versi WhatsApp**.

---

## 📜 Penafian & Lisensi

- **Penafian (Disclaimer):** Modul ini disediakan *"sebagaimana adanya"*. Melakukan *root* pada perangkat Samsung akan membatalkan garansi Samsung Knox. Pengembang tidak bertanggung jawab atas *bootloop*, ketidakstabilan sistem, atau masalah pada aplikasi pihak ketiga.
- **Lisensi:** Didistribusikan di bawah lisensi **GNU General Public License v3.0 (GPLv3)**. Lihat file `LICENSE` untuk informasi selengkapnya.