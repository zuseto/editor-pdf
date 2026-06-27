# Editor PDF

Tool **editor PDF berbasis web** dalam **satu file HTML** — tanpa server, tanpa build, tanpa instalasi. Semua proses berjalan **lokal di browser** sehingga file PDF tidak pernah diunggah ke mana pun (privat & aman). Dirancang untuk mudah ditempel di **Blogspot** atau halaman web mana pun.

> Bagian dari kumpulan tool PDF bertema **emerald** (selaras dengan _Organize PDF_).

**🔗 Demo langsung:** https://zuseto.github.io/editor-pdf/

## ✨ Fitur

- **Tambah Teks** — klik di halaman untuk menaruh teks, klik dua kali untuk menyunting. Atur warna & ukuran font.
- **Blok Warna / Sorotan** dengan pilihan **bentuk** lewat dropdown:
  - ■ Blok isi (sorotan/stabilo)
  - ▢ Kotak garis (mengotaki)
  - ● Elips isi
  - ○ Lingkaran garis (melingkari)
- **Preset Stabilo** (kuning / hijau / pink / biru) untuk sorotan instan.
- **Garis** lurus & **Coret** bebas (freehand) dengan pengatur ketebalan.
- **Sisip Gambar** (PNG, JPG, WebP, GIF — otomatis dikonversi ke PNG agar pasti ter-embed).
- **Geser, ubah ukuran, hapus** tiap elemen.
- **Undo / Redo** (termasuk `Ctrl+Z` / `Ctrl+Y`) hingga 40 langkah.
- **Hapus editan** per halaman atau semua halaman sekaligus.
- **Multi-halaman** dengan navigasi & **zoom**.
- **Simpan & Unduh** menjadi PDF baru (`editor.pdf`) — semua editan dibakar ke dalam dokumen.

## 🚀 Cara Pakai

1. Buka `editorpdf.html` langsung di browser (klik dua kali), **atau** tempel kodenya ke halaman web.
2. Seret & jatuhkan file PDF ke kotak unggah, atau klik untuk memilih.
3. Edit menggunakan toolbar di atas halaman.
4. Klik **Simpan & Unduh PDF**.

## 📝 Cara Menempel di Blogspot

1. Buka editor pos Blogspot, pindah ke mode **HTML view**.
2. Salin seluruh isi `editorpdf.html` dan tempel ke badan pos.
3. Publikasikan. Seluruh tool dibungkus dalam `#pdf-editor-app-container` agar tidak bentrok dengan tema blog.

> Catatan: ada slot iklan **Google AdSense** di dalam file. Ganti `data-ad-client` & `data-ad-slot` dengan milikmu, atau hapus blok `<ins class="adsbygoogle">` bila tidak dipakai.

## 🧱 Teknologi

- [PDF.js](https://github.com/mozilla/pdf.js) — render pratinjau halaman (via CDN).
- [pdf-lib](https://pdf-lib.js.org/) — menulis teks, bentuk, garis, & gambar ke PDF (via CDN).
- [Font Awesome](https://fontawesome.com/) & [Inter](https://fonts.google.com/specimen/Inter) untuk ikon & tipografi.

Tidak ada langkah build — cukup buka file HTML-nya.

## 🔒 Privasi

Seluruh pemrosesan terjadi di perangkat pengguna (di dalam browser). **Tidak ada file yang dikirim ke server.**

## ⚠️ Catatan Teknis

- Halaman dirender pada rotasi 0° agar koordinat layar ↔ titik PDF konsisten. PDF dengan `/Rotate` bawaan akan tampil tegak.
- Teks memakai font standar **Helvetica** (WinAnsi). Karakter di luar Latin-1 (mis. emoji) diganti `?` saat disimpan.

## 📄 Lisensi

[MIT](LICENSE) © zuseto
