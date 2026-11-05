# 🌐 Free Subdomain Provider — *.zettai.my.id

> Layanan Penyedia Subdomain Gratis `*.zettai.my.id` Terintegrasi Cloudflare DNS API v4, Otomatis SSL HTTPS, dan CDN Anti-DDoS.

Repo ini digunakan sebagai **Otentikasi & Registrasi Subdomain Terverifikasi** di [Zettai APIs](https://zettai.my.id/app/subdomain). Setiap pengguna yang ingin mendaftarkan subdomain gratis wajib melakukan **Fork** pada repository ini dan membuat file konfigurasi JSON.

---

## 🚀 Cara Mendaftarkan Subdomain Gratis

### 1. Fork & Star Repository Ini ⭐
1. Klik tombol **Fork** di pojok kanan atas repository ini: [Fork free-subdo](https://github.com/KazeDevID/free-subdo/fork).
2. Jangan lupa berikan **Star ⭐** untuk mendukung pengembang!

### 2. Buat File JSON Subdomain Kamu
Di repositori hasil Fork milikmu:
1. Buka folder `domains/`
2. Buat file baru dengan nama `domains/<nama-subdomain>.json` (contoh: `domains/mybot.json`).
3. Masukkan konfigurasi JSON seperti template:

```json
{
  "name": "mybot",
  "type": "CNAME",
  "target": "kazedev.github.io",
  "proxied": true,
  "title": "My Awesome Project",
  "description": "WhatsApp Bot & Landing Page",
  "creator": "username-github-kamu"
}
```

#### Pilihan Tipe Record:
- **CNAME**: Untuk GitHub Pages (`username.github.io`), Vercel (`cname.vercel-dns.com`), Render, Railway.
- **A**: Untuk server VPS (masukkan alamat IPv4, contoh: `103.145.22.10`).
- **REDIRECT**: Untuk URL redirection (contoh: `https://instagram.com/namakamu` atau link WhatsApp).
- **AAAA**: Untuk IPv6.
- **TXT**: Untuk verifikasi domain.

### 3. Verifikasi & Aktifkan di Web Portal
1. Buka portal [Zettai Subdomain](https://zettai.my.id/app/subdomain).
2. Masukkan nama subdomain dan **Username GitHub** kamu.
3. Klik **Verifikasi Fork & Aktifkan Subdomain**!
4. Sistem gateway akan otomatis memverifikasi repository fork kamu dan menerbitkan DNS Cloudflare secara instan.

---

## 👑 Keuntungan Sistem Ini
- **Permanen & Terbuka**: Konfigurasi domain kamu tercatat di GitHub secara transparan.
- **Dukungan Open-Source**: Membantu repositori owner mendapatkan achievement di GitHub (Forks, Stars, Contributors).
- **SSL Otomatis**: Dilengkapi Universal SSL dari Cloudflare tanpa biaya sepeserpun.

Created with ❤️ by [KazeDevID](https://github.com/KazeDevID).
