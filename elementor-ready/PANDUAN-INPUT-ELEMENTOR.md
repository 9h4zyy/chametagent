# Panduan Lengkap Input Project Chamet Agency ke WordPress Elementor

File-file di dalam folder `elementor-ready/` ini sudah **100% dipersiapkan khusus untuk WordPress & Elementor**. Tag `<!DOCTYPE html>`, `<head>`, `<link rel="stylesheet">`, dan script preview lokal sudah dibersihkan sehingga Anda dapat langsung melakukan **Copy & Paste** ke widget Elementor tanpa konflik tag maupun error console.

---

## 📁 Struktur Folder Siap Pakai

```text
elementor-ready/
├── PANDUAN-INPUT-ELEMENTOR.md          <-- Panduan ini
├── 00-GLOBAL-CSS/
│   └── global.css                     <-- CSS Global Sitewide
├── 01-THEME-BUILDER/
│   ├── header-template.html           <-- Template Header (Theme Builder)
│   └── footer-template.html           <-- Template Footer (Theme Builder)
├── 02-MAIN-PAGES/
│   ├── 01-page-home.html              <-- Halaman Home (Slug: /)
│   ├── 02-page-host.html              <-- Halaman Host (Slug: /host)
│   ├── 03-page-agent.html             <-- Halaman Agent (Slug: /agent)
│   └── 04-page-faq-hub.html           <-- Halaman FAQ Hub (Slug: /faq)
├── 03-FAQ-CATEGORY-PAGES/
│   ├── page-faq-general.html          <-- Slug: /faq-general
│   ├── page-faq-agency.html           <-- Slug: /faq-agency
│   ├── page-faq-app-account.html      <-- Slug: /faq-app-account
│   ├── page-faq-live-rules.html       <-- Slug: /faq-live-rules
│   └── page-faq-withdrawal.html       <-- Slug: /faq-withdrawal
└── 04-FAQ-QUESTION-ARTICLES/
    ├── faq-answer-01-what-is-chamet.html
    ├── ... (Total 48 file artikel pertanyaan FAQ)
    └── faq-answer-48-how-is-my-chamet-agency-commission-ratio-calculated.html
```

---

## 🚀 Langkah 1: Pasang Global CSS (Sitewide)

CSS ini mengatur seluruh tema visual, variabel warna neon violet/pink, tipografi font Google, glassmorphism, animasi interaktif, tombol, dan responsivitas mobile-first.

1. Masuk ke Dashboard WordPress -> Edit halaman apa saja dengan Elementor.
2. Klik tombol menu burger (garis tiga di pojok kiri atas panel Elementor) -> pilih **Site Settings** (Pengaturan Situs).
3. Pilih menu **Custom CSS** (CSS Kustom).
4. Buka file `elementor-ready/00-GLOBAL-CSS/global.css`, copy seluruh isinya, lalu paste ke kotak Custom CSS tersebut.
5. Klik **Update / Save Changes**.

*(Alternatif jika tidak memakai Elementor Pro: Masuk ke WP Admin -> **Appearance (Tampilan)** -> **Customize (Sesuaikan)** -> **Additional CSS (CSS Tambahan)**, paste di sana lalu klik Terbitkan).*

---

## 🧭 Langkah 2: Pasang Header & Footer di Elementor Theme Builder

Header dan footer dibuat terpisah sebagai template global agar konsisten di seluruh halaman situs.

### A. Template Header
1. Di Dashboard WP Admin, pilih **Templates** -> **Theme Builder** -> klik **Header** -> **Add New**.
2. Masukkan nama template (misal: `Chamet Global Header`).
3. Tambahkan 1 Container / Section Full Width (Content Width: Full Width, Columns Gap: No Gap, Padding: 0).
4. Tarik widget **HTML** (HTML Code) ke dalam container tersebut.
5. Buka file `elementor-ready/01-THEME-BUILDER/header-template.html`, copy seluruh isinya dan paste ke widget HTML.
6. Klik **Publish**, lalu atur Display Condition: **Entire Site** -> klik **Save & Close**.

### B. Template Footer
1. Di Dashboard WP Admin, pilih **Templates** -> **Theme Builder** -> klik **Footer** -> **Add New**.
2. Masukkan nama template (misal: `Chamet Global Footer`).
3. Tambahkan 1 Container / Section Full Width (Content Width: Full Width, Columns Gap: No Gap, Padding: 0).
4. Tarik widget **HTML** ke dalam container.
5. Buka file `elementor-ready/01-THEME-BUILDER/footer-template.html`, copy seluruh isinya dan paste ke widget HTML.
6. Klik **Publish**, lalu atur Display Condition: **Entire Site** -> klik **Save & Close**.

---

## 📄 Langkah 3: Membuat Halaman (Pages) Menggunakan Widget HTML

Untuk setiap halaman (Home, Host, Agent, FAQ, dst.), ikuti langkah standar berikut:

1. Masuk ke WP Admin -> **Pages (Laman)** -> **Add New (Tambah Baru)**.
2. Beri Judul Halaman (misal: `Home`, `Host`, `Agent`, atau `FAQ`).
3. Atur **Permalink / URL Slug** sesuai daftar di bawah.
4. Klik tombol **Edit with Elementor**.
5. Pada panel Elementor, klik icon **Settings (Roda Gigi)** di pojok kiri bawah:
   - Ubah **Page Layout** menjadi **Elementor Full Width**.
   *(Layout ini otomatis memuat Header dan Footer dari Theme Builder dan membebaskan area konten utama).*
6. Buat 1 Container / Section:
   - Content Width: **Full Width**
   - Padding / Margin: **0**
7. Drag & Drop 1 widget **HTML** ke dalam container tersebut.
8. Buka file kode yang sesuai dari folder `02-MAIN-PAGES` / `03-FAQ-CATEGORY-PAGES` / `04-FAQ-QUESTION-ARTICLES`.
9. Copy seluruh isi file dan paste ke kolom input widget HTML Elementor.
10. Klik **Publish / Update**. Selesai!

---

## 🔗 Daftar Slug / Permalink Wajib

Agar link antar-halaman (navbar, tombol CTA, kartu kategori FAQ, related questions) bekerja sempurna, pastikan URL slug setiap page diatur sebagai berikut:

### 1. Halaman Utama (`02-MAIN-PAGES`)
| File Sumber | Judul Halaman WP | Permalink / Slug Wajib | Keterangan |
| :--- | :--- | :--- | :--- |
| `01-page-home.html` | Home | `/` (Atur sebagai Front Page di Settings > Reading) | Beranda Utama |
| `02-page-host.html` | Host | `/host` | Portal Pendaftaran & Karir Host |
| `03-page-agent.html` | Agent | `/agent` | Portal Pendaftaran & Komisi Agensi |
| `04-page-faq-hub.html` | FAQ | `/faq` | Pusat Bantuan & Knowledge Hub |

### 2. Halaman Kategori FAQ (`03-FAQ-CATEGORY-PAGES`)
| File Sumber | Judul Halaman WP | Permalink / Slug Wajib |
| :--- | :--- | :--- |
| `page-faq-general.html` | General Questions | `/faq-general` |
| `page-faq-agency.html` | Agency Questions | `/faq-agency` |
| `page-faq-app-account.html` | App & Account | `/faq-app-account` |
| `page-faq-live-rules.html` | Live Streaming & Rules | `/faq-live-rules` |
| `page-faq-withdrawal.html` | Withdrawal & Commission | `/faq-withdrawal` |

### 3. Halaman Detail Pertanyaan FAQ (`04-FAQ-QUESTION-ARTICLES`)
- Terdapat 48 artikel FAQ interaktif.
- Slug halaman harus sama persis dengan nama file tanpa ekstensi `.html`.
- Contoh:
  * File `faq-answer-01-what-is-chamet.html` -> Slug: `/faq-answer-01-what-is-chamet`
  * File `faq-answer-28-how-can-i-withdraw-my-chamet-agency-commission.html` -> Slug: `/faq-answer-28-how-can-i-withdraw-my-chamet-agency-commission`

---

## ✨ Fitur & Keunggulan Khusus Paket Ini

1. **Asset Gambar Online**: Semua gambar hero, ilustrasi badge, dan logo menggunakan URL CDN online aktif (`https://chametagent.com/wp-content/uploads/2026/10/...`), sehingga Anda tidak perlu mengupload ulang gambar ke media library WordPress secara manual.
2. **Font Otomatis**: Font Google (*Plus Jakarta Sans* & *Outfit*) ter-load langsung dari `@import` di `global.css`.
3. **Internal JavaScript Aman**: Semua logika interaktif (Accordion FAQ, Mobile Hamburger Menu, Image Lightbox Modal, dan Emoticon SVG) menggunakan Vanilla JavaScript murni tanpa ketergantungan jQuery atau script eksternal berat.
4. **Zero Layout Shift (CLS)**: Setiap gambar memiliki dimensi `width` dan `height` presisi serta `alt` yang lengkap sesuai best practice SEO & Accessibility Elementor.
