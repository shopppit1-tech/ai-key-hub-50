# API GRATIS — 50 Direktori API AI

Static Progressive Web App (PWA) berbahasa Indonesia. Situs API GRATIS dapat diinstal dari browser yang mendukung PWA dan menyimpan shell halaman untuk akses offline setelah kunjungan pertama.

## Berkas PWA

- `index.html` — halaman utama, tombol instal, dan registrasi service worker.
- `manifest.webmanifest` — nama aplikasi, warna, mode standalone, dan ikon.
- `service-worker.js` — cache shell dan fallback navigasi offline.
- `icons/` — ikon aplikasi ukuran 180, 192, dan 512 piksel.

## GitHub Pages

Workflow `.github/workflows/pages.yml` menerbitkan branch `main`. Pada konfigurasi awal, buka **Settings → Pages → Build and deployment**, lalu pilih **GitHub Actions** sebagai source. Setelah Pages diaktifkan, push ke `main` akan menjalankan deploy otomatis.

PWA memerlukan HTTPS (GitHub Pages menyediakan HTTPS) dan browser yang mendukung instalasi aplikasi web. Pada iPhone/iPad, gunakan menu Bagikan di Safari lalu pilih **Tambahkan ke Layar Utama**.


## SEO dan Google Search

- `robots.txt` mengizinkan crawl halaman publik dan menunjuk ke sitemap.
- `sitemap.xml` berisi URL kanonis situs: `https://apigratis.my.id/`.
- Metadata title, description, canonical, Open Graph, Twitter Card, dan WebSite JSON-LD tersedia di HTML awal.
- Daftar 50 layanan dirender sebagai HTML statis; JavaScript hanya mengaktifkan pencarian dan filter.
- Properti domain diverifikasi di Google Search Console. Kirim `https://apigratis.my.id/sitemap.xml` melalui laporan **Sitemaps** setelah deploy.
