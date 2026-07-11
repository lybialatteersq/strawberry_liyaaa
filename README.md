🍓 Strawberry Café — Website E-Commerce
"Soft dessert, sweet drink's."

Website e-commerce single-page untuk brand minuman dan dessert stroberi Strawberry Café, dibangun dengan HTML5, CSS3, dan Vanilla JavaScript murni — tanpa framework, tanpa backend, tanpa proses build. Langsung buka di browser, langsung jalan.

---

📋 Daftar Isi

Dokumentasi Bisnis
- Profil Brand
- Daftar Produk & Harga
- Metode Pembayaran
- Informasi Kontak
- Alur Pemesanan Pelanggan
- Rencana Pengembangan Bisnis

Dokumentasi Teknis
- Stack Teknologi
- Struktur File
- Arsitektur Halaman
- Logika JavaScript
- Sistem CSS & Tema Warna
- Cara Menjalankan
- Cara Deploy ke GitHub Pages
- Panduan Kustomisasi
- Status & Batasan

---

🏢 Dokumentasi Bisnis

1.1 Profil Brand

| Nama Brand | Strawberry Café |
|---|---|
| Tagline | "Soft dessert, sweet drink's." |
| Jenis Usaha | Minuman dan dessert berbahan dasar stroberi segar |
| Target Pasar | Remaja dan dewasa muda usia 15–30 tahun, pecinta makanan manis dan estetik |
| Keunggulan | Semua produk berbasis stroberi segar pilihan, dibuat homemade tanpa pengawet berlebihan |
| Jam Operasional | Setiap hari, 08.00 – 21.00 |

---

1.2 Daftar Produk & Harga

| No | Nama Produk | Deskripsi | Harga |
|---|---|---|---|
| 1 | Strawberry Dream Smoothies | Smoothie stroberi segar blended creamy, cocok buat mood booster | Rp 18.000 |
| 2 | Strawberry Matcha Milk | Matcha lembut bertemu stroberi manis, kombinasi estetik dan enak | Rp 22.000 |
| 3 | Strawberry Latte | Latte sutra dengan strawberry purée di bawah foam susu hangat | Rp 25.000 |
| 4 | Strawberry Cheesecake | Cheesecake lembut, graham cracker crust, topping stroberi segar | Rp 32.000 |
| 5 | Strawberry Choco Mint | Coklat gelap, mint segar, dan stroberi, trio rasa yang sempurna | Rp 28.000 |
| 6 | Strawberry Moci | Mochi kenyal isi filling stroberi dan krim, satu gigitan bliss | Rp 20.000 |

💡 Harga dapat diubah langsung di array products pada file script.js.

Biaya Pengiriman: Gratis ongkos kirim setiap Sabtu dan Minggu. Hari kerja dikenakan biaya sesuai jarak.

---

1.3 Metode Pembayaran

| Metode | Keterangan |
|---|---|
| 💙 E-Wallet DANA | Transfer instan ke nomor DANA terdaftar |
| 🧡 E-Wallet ShopeePay | Scan QR atau kirim ke akun ShopeePay |
| 🏦 Transfer Virtual Account BNI | Bayar via internet banking atau mobile banking BNI |

⚠️ Catatan: Pembayaran saat ini adalah simulasi front-end. Belum terhubung ke payment gateway sungguhan.

---

1.4 Informasi Kontak

| Kanal | Detail |
|---|---|
| 📞 Telepon / WhatsApp | 089607039881 |
| ✉️ Email | lybianamuftifa@gmail.com |
| 🕐 Jam Buka | Setiap hari, 08.00 – 21.00 |

---

1.5 Alur Pemesanan Pelanggan

```
┌─────────────────────────────────────────────────────────┐
│                   CUSTOMER JOURNEY                       │
├─────────────────────────────────────────────────────────┤
│                                                          │
│  1. Buka website → lihat Hero Section (Home)             │
│          ↓                                               │
│  2. Scroll / klik "Belanja Sekarang" → lihat 6 produk    │
│          ↓                                               │
│  3. Filter kategori / cari produk → klik tombol "+"      │
│          ↓                                               │
│  4. Buka Keranjang → cek item, ubah qty jika perlu       │
│          ↓                                               │
│  5. Isi form pengiriman → Nama, Email, HP, Alamat        │
│          ↓                                               │
│  6. Klik "Konfirmasi & Lanjut Bayar" → pilih metode      │
│          ↓                                               │
│  7. Klik "Bayar Sekarang" → muncul konfirmasi sukses     │
│          ↓                                               │
│  8. Keranjang otomatis kosong → siap order berikutnya    │
│                                                          │
└─────────────────────────────────────────────────────────┘
```

---

1.6 Rencana Pengembangan Bisnis

- [ ] Integrasi payment gateway resmi (Midtrans / Xendit)
- [ ] Notifikasi otomatis WhatsApp/email ke pemilik saat order masuk
- [ ] Sistem login & riwayat pesanan pelanggan
- [ ] Dashboard admin: kelola menu, harga, stok
- [ ] Ongkos kirim dinamis berdasarkan lokasi
- [ ] Program loyalitas / poin reward pelanggan
- [ ] Fitur ulasan & rating produk
- [ ] Integrasi marketplace (Tokopedia, Shopee)

---

🛠 Dokumentasi Teknis

2.1 Stack Teknologi

| Komponen | Teknologi | Keterangan |
|---|---|---|
| Struktur | HTML5 | Semantik, aksesibel |
| Styling | CSS3 murni | Custom properties, Grid, Flexbox |
| Interaktivitas | Vanilla JavaScript | Tanpa library/framework |
| Font | Google Fonts | Playfair Display + DM Sans |
| Foto Produk | URL Unsplash | Foto langsung dari link eksternal |
| Dependensi | Google Fonts CDN | Satu-satunya dependensi eksternal |
| Build tool | ❌ Tidak ada | Tidak perlu npm, webpack, dll |
| Backend | ❌ Tidak ada | Murni front-end statis |

---

2.2 Struktur File

```
strawberry-cafe/
│
├── index.html        ← Struktur halaman utama
├── style.css         ← Seluruh styling dan responsive design
├── script.js         ← Seluruh logika interaktif
└── README.md         ← Dokumentasi ini
```

---

2.3 Arsitektur Halaman

```
index.html
│
├── <nav>                  Navigasi fixed (logo + menu link + search bar)
│
├── <section #home>        Hero: judul, deskripsi brand, tombol CTA
├── <section #promo>       Kartu promo: New Member, Happy Hour, Weekend
├── <section #menu>        Grid 6 kartu produk dengan foto, harga, tombol +
├── <section #about>       Cerita brand + chips keunggulan
│
├── <footer>               Kontak yang bisa diklik + copyright
│
├── #cart-bubble           Tombol keranjang pojok kanan bawah
│
└── #cartModal             Modal keranjang belanja
    ├── Cart Items          Daftar produk + qty control
    ├── Cart Total          Total harga otomatis
    ├── #delivery-section   Form data pengiriman
    ├── #payment-section    Pilih metode pembayaran
    └── #success-section    Konfirmasi pembayaran berhasil
```

---

2.4 Logika JavaScript

Data Produk

Semua data produk disimpan dalam satu array products di script.js:

```javascript
const products = [
  {
    id: 1,
    name: "Strawberry Dream Smoothies",
    cat: "drink",
    price: 18000,
    img: "https://images.unsplash.com/...",
    desc: "Smoothie stroberi segar blended creamy."
  },
  // ...
];
```

Array ini adalah single source of truth — kartu menu, isi keranjang, dan total harga semuanya dirender dari array ini.

State Keranjang

```javascript
let cart = {};
// Contoh isi: { 1: 2, 3: 1 }
// artinya: produk id=1 qty 2, produk id=3 qty 1
```

| Fungsi | Tugasnya |
|---|---|
| addToCart(id) | Tambah produk ke keranjang, update bubble count |
| changeQty(id, delta) | Tambah/kurangi qty; hapus otomatis jika qty ≤ 0 |
| renderCart() | Re-render isi modal setiap kali state berubah |
| updateBubble() | Update angka di tombol keranjang pojok bawah |
| rupiah(n) | Format angka ke format Rupiah |

Alur Checkout

```
openCart()          → buka modal keranjang
renderCart()        → tampilkan item + form pengiriman
confirmDelivery()   → validasi form, tampilkan section pembayaran
selectPay()         → pilih metode, tampilkan instruksi pembayaran
bayarSekarang()     → validasi metode, tampilkan sukses
resetAll()          → reset cart, form, dan tutup modal
```

Validasi

- Form pengiriman: Nama, Email, HP, dan Alamat wajib diisi
- Format email divalidasi dengan regular expression
- Pembayaran: wajib pilih salah satu metode sebelum bisa bayar

---

2.5 Sistem CSS & Tema Warna

Semua warna menggunakan CSS Custom Properties di :root agar mudah diganti:

```css
:root {
  --rose:     #F7A8B8;   /* Pink rose — warna utama */
  --blush:    #FDDDE6;   /* Pink blush — latar section */
  --cream:    #FFF5F7;   /* Krem pink — latar halaman */
  --lavender: #E8D5F5;   /* Lavender — aksen promo */
  --text:     #4A2C35;   /* Coklat tua — teks utama */
  --muted:    #9B6F7A;   /* Mauve — teks sekunder */
  --white:    #FFFFFF;   /* Putih — latar kartu */
  --border:   #F2C5D0;   /* Pink border — garis pembatas */
}
```

Tipografi:
- Playfair Display (serif) → heading & judul: kesan elegan dan feminin
- DM Sans (sans-serif) → body text: bersih dan mudah dibaca

Layout:
- CSS Grid untuk menu produk (auto-fill minmax 240px)
- Flexbox untuk navigasi, kartu, dan modal
- Breakpoint utama: 768px (tablet/mobile)

Animasi:
- Modal keranjang: animation slideUp 0.3s ease
- Hover kartu produk: transform translateY(-4px) + box-shadow
- Semua transisi murni CSS, tanpa library animasi

---

🚀 Cara Menjalankan

Di Komputer Lokal

Cara 1 — Langsung buka (paling simpel):

Double-click file index.html → terbuka di browser

Cara 2 — Pakai Live Server di VS Code (direkomendasikan):

1. Install extension Live Server di VS Code
2. Klik kanan index.html → Open with Live Server
3. Website auto-refresh setiap kali kamu edit & save ✅

Tidak perlu npm install, node, atau setup apapun.

---

🌐 Cara Deploy ke GitHub Pages

```
1. Buat akun GitHub → github.com

2. Klik "New repository"
   - Nama repo: strawberry-cafe
   - Visibility: Public
   - Klik "Create repository"

3. Upload file:
   - Klik "uploading an existing file"
   - Drag & drop: index.html, style.css, script.js, README.md
   - Klik "Commit changes"

4. Aktifkan GitHub Pages:
   - Settings → Pages (menu kiri)
   - Source: Deploy from a branch
   - Branch: main → / (root)
   - Klik Save

5. Tunggu 1-2 menit, lalu website live di:
   https://usernamekamu.github.io/strawberry-cafe
```

---

✏️ Panduan Kustomisasi

Ubah Nama / Harga Produk

Edit array products di dalam script.js:

```javascript
{ id:1, name:"Nama Produk Baru", cat:"drink", price:20000,
  img:"https://...", desc:"Deskripsi produk." }
```

Tambah Produk Baru

Tambah objek baru di array products di script.js, sesuaikan kategori dengan "drink" atau "dessert".

Ubah Warna Tema

Edit nilai hex di :root pada style.css:

```css
--rose: #F7A8B8; /* ganti warna utama di sini */
```

Ubah Foto Background Hero

Cari di style.css:

```css
#home {
  background: url('link-foto-baru') center/cover no-repeat;
}
```

Ubah Foto Produk

Ganti URL foto di array products pada script.js dengan URL foto baru.

Ubah Kontak

Cari di index.html bagian footer dan ganti nomor serta email.

---

⚠️ Status & Batasan

| Fitur | Status | Keterangan |
|---|---|---|
| Tampilan & navigasi | ✅ Selesai | Responsif, mobile-friendly |
| Filter & search produk | ✅ Selesai | Real-time by kategori & nama |
| Slider range harga | ✅ Selesai | Filter harga maksimum |
| Keranjang belanja | ✅ Selesai | Tambah, kurangi, hapus item |
| Form pengiriman | ✅ Selesai | Validasi semua field + format email |
| Pilih metode pembayaran | ✅ Selesai | 3 pilihan tersedia |
| Konfirmasi transaksi | ✅ Selesai | Pesan sukses dengan nama pembeli |
| Penyimpanan pesanan | ❌ Belum ada | Pesanan hilang saat refresh |
| Payment gateway resmi | ❌ Belum ada | Masih simulasi |
| Notifikasi ke pemilik | ❌ Belum ada | Perlu backend/WA API |
| Login pelanggan | ❌ Belum ada | Perlu autentikasi |
| Manajemen stok | ❌ Belum ada | Perlu admin panel + database |

Rekomendasi Langkah Selanjutnya (Go-Live)

- Payment Gateway → Daftar di Midtrans atau Xendit, integrasikan Snap.js
- Database pesanan → Gunakan Google Sheets + Google Apps Script (gratis) atau Firebase
- Notifikasi WhatsApp → Gunakan WA Business API atau Fonnte
- Hosting lebih profesional → Vercel atau Netlify (lebih cepat dari GitHub Pages, tetap gratis)

---

📄 Kredit

Website dibuat khusus untuk brand Strawberry Café
Font: Playfair Display & DM Sans via Google Fonts
Foto produk: Unsplash (keperluan akademik)

© 2025 Strawberry Café. Soft dessert, sweet drink's. 🍓
