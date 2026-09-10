# Inspirasi & Ekspirasi - Game Pembelajaran Pernapasan 🫁

Game interaktif edukasi mengenai mekanisme pernapasan manusia (Inspirasi dan Ekspirasi) untuk mata pelajaran Biologi/IPA (Bab 2 - Hal 42), dikembangkan dengan standar visual futuristik dan responsif untuk berbagai perangkat (Desktop, Laptop, Tablet, dan Ponsel).

---

## 🌟 Fitur Utama

1. **Dual-Layer Responsive Architecture**:
   - Panggung interaktif dengan rasio aspek standar 16:9 (`.game-stage`) yang berpusat di tengah layar.
   - Penskalaan otomatis berbasis **Container Queries (`cqw` dan `cqh`)** sehingga teks, kartu, slider, dan karakter selalu terbingkai proporsional tanpa risiko teks meluap (*overflow*).
   - Latar belakang ambient *full-bleed* yang mengisi layar secara penuh tanpa garis potong hitam.
2. **Simulasi Pernapasan Interaktif (Lottie Animation)**:
   - Slider dinamis untuk mengontrol proses tarik napas (*Inspirasi*) dan hembus napas (*Ekspirasi*).
   - Visualisasi pergerakan paru-paru, diafragma, serta aliran gas O2 dan CO2 secara langsung.
3. **Tantangan Menahan Napas**:
   - Fitur latihan fase bernapas (Tarik napas, Tahan napas, dan Hembus napas) dengan penanda durasi detik interaktif.
4. **Kuis Evaluasi Pemahaman**:
   - 4 soal pilihan ganda interaktif dengan umpan balik visual dan audio instan serta perhitungan skor akhir.
5. **Dukungan Audio Lengkap**:
   - Musik latar (*ambient music*), efek suara klik/geser, peluit, suara apresiasi skor, dan narasi panduan (*voice-over*).

---

## 📁 Struktur Direktori

```text
├── index.html          # File HTML utama aplikasi & logic game
├── package.json        # Metadata proyek & script lokal
├── vercel.json         # Konfigurasi deployment & cache Vercel
├── .gitignore          # File pengecualian Git
├── README.md           # Dokumentasi proyek
└── assets/
    ├── audio/          # Musik latar, sound effects, dan rekaman narasi VO
    ├── images/         # Asset SVG kartu, tombol, background, dan storyboard
    ├── js/             # Library lottie.min.js & data animasi JSON
    └── motion/         # File kerja animasi Lottie JSON & dokumen logika motion
```

---

## 🚀 Menjalankan Secara Lokal

Anda dapat menjalankan proyek ini langsung di browser atau menggunakan server lokal ringan:

### Opsi 1: Menggunakan Node / npm
```bash
# Menjalankan local server di port 3000
npm start
```
Buka browser dan akses: `http://localhost:3000`

### Opsi 2: Langsung Buka File HTML
Buka file `index.html` dengan peramban modern (Google Chrome, Microsoft Edge, Mozilla Firefox, atau Safari).

---

## ☁️ Panduan Deploy ke Vercel

Proyek ini telah dikonfigurasi penuh dengan `vercel.json` dan siap di-deploy ke Vercel secara langsung:

### Metode 1: Hubungkan ke GitHub (Direkomendasikan)
1. Buat repositori baru di akun GitHub Anda (misal: `inspirasi-ekspirasi-game`).
2. Jalankan perintah git untuk menambahkan remote dan push:
   ```bash
   git remote add origin https://github.com/USERNAME/inspirasi-ekspirasi-game.git
   git branch -M main
   git push -u origin main
   ```
3. Masuk ke [dashboard Vercel](https://vercel.com/new).
4. Pilih **Import Git Repository** dan pilih repositori yang baru saja di-push.
5. Biarkan pengaturan default (Framework Preset: *Other*), lalu klik **Deploy**.

### Metode 2: Deploy Cepat Menggunakan Vercel CLI
Jika Anda telah menginstal Vercel CLI di komputer:
```bash
npx vercel
```
Ikuti petunjuk di terminal untuk mempublikasikan proyek dalam hitungan detik.

---

## 📜 Lisensi
Dikembangkan untuk keperluan media pembelajaran interaktif.
