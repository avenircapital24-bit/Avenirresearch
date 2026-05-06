# Avenir Research & Publication

Portal riset ekuitas PT Avenir Fortuna Corporindo — multi-page HTML.

## Struktur File

```
Avenir_Research/
├── index.html                    ← Beranda (home)
├── katalog.html                  ← Katalog semua riset
├── news.html                     ← Daftar Market News
├── news-pdb-q1-2026.html         ← Artikel news
├── news-windfall-tax-nikel.html  ← Artikel news
├── news-tpia-force-majeure.html  ← Artikel news
├── ptro.html                     ← Riset PT Petrosea Tbk
├── smar.html                     ← Riset PT SMART Tbk
├── mrvl.html                     ← Riset Marvell Technology
├── crm.html                      ← Riset Salesforce Inc
├── cmry.html                     ← Riset PT Cisarua Mountain Dairy
├── avia.html                     ← Riset PT Avian Brands
├── nisp.html                     ← Riset Bank OCBC NISP
├── bbri.html                     ← Riset Bank BRI
├── asgr.html                     ← Riset PT Astra Graphia
├── dewa.html                     ← Riset PT Dharma Satya Nusantara
├── ades.html                     ← Riset PT Akasha Wira International
├── wifi.html                     ← Riset PT Solusi Sinergi Digital
├── part.html                     ← Riset PT Mitra Pack
├── tentang.html                  ← Tentang Avenir
├── mitra.html                    ← Halaman Mitra
├── pengguna.html                 ← Akun Pengguna
└── vercel.json                   ← Konfigurasi deployment Vercel
```

## Cara Deploy ke Vercel

1. Extract ZIP → dapat folder `Avenir_Research/`
2. Upload folder ke GitHub (repo baru atau existing)
3. Connect repo di [vercel.com](https://vercel.com) → auto-deploy
4. Setelah dapat URL Vercel, set di Supabase:
   - Dashboard Supabase → **Authentication → URL Configuration**
   - **Site URL**: `https://[nama-project].vercel.app`
   - **Redirect URLs**: `https://[nama-project].vercel.app/*`

## Tambah Halaman Baru

- **News baru**: duplikat salah satu `news-*.html`, edit isinya, tambah link di `news.html`
- **Riset baru**: lihat file `TEMPLATE_riset.html` (tersedia terpisah), tambah card di `katalog.html`

## Catatan

- Setiap file HTML **self-contained** — CSS, JS, dan gambar sudah terembed
- Navigasi antar halaman menggunakan `window.location.href` (bukan SPA hash)
- Auth menggunakan Supabase (konfigurasi sudah terembed)

---
© 2026 PT Avenir Fortuna Corporindo · avenirfortuna.com
