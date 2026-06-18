# 氷狐 Hyouko — Profile Card

Profile card pribadi Palih (Twitter & Wuthering Waves). Static site, no build step — vanilla HTML/CSS/JS.

🔗 Live: `https://Fall-Llihc.github.io/WutheringWaves-ProfileCard/` (aktif setelah GitHub Pages dinyalakan, lihat di bawah)

## Struktur

```
.
├── index.html          # markup utama (hero, info, BYF/DNI, joki, footer)
├── css/
│   └── style.css        # tone merah-putih-hitam, font Zen Old Mincho + Rajdhani + Inter
├── js/
│   └── main.js           # copy-to-clipboard untuk UID game
├── assets/
│   └── favicon.svg
├── .nojekyll             # supaya GitHub Pages tidak menjalankan Jekyll build
└── .gitignore
```

## Ganti avatar

Avatar saat ini berupa SVG inline (ikon topeng kitsune) di dalam `index.html` (bagian `.avatar`). Kalau mau pakai foto/art asli:

1. Taruh file gambar di `assets/avatar.png` (atau `.jpg`/`.webp`).
2. Di `index.html`, ganti blok `<svg class="avatar__mask">...</svg>` dengan `<img src="assets/avatar.png" alt="Avatar">`.
3. (Opsional) sesuaikan ukuran lewat class `.avatar` di `css/style.css`.

## Nyalakan GitHub Pages (sekali saja, manual)

1. Buka repo di GitHub → **Settings → Pages**.
2. Source: **Deploy from a branch**.
3. Branch: **main**, folder **/(root)** → **Save**.
4. Tunggu ~1 menit, situs akan live di URL di atas.

## Edit konten

Semua teks (bio, BYF, DNI, info joki) ada langsung di `index.html`, dicari gampang lewat komentar `<!-- ... -->` per section.
