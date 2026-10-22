# CODING AGENT RULES

Projek ini akan dipakai untuk Wordpress Elementor HTML Element dan Site Custom CSS. Oleh karena itu, projek ini WAJIB mengikuti konfigurasi ini:

- Setiap page adalah HTML.
- Setiap HTML page punya Javascripnya sendiri dan WAJIB INTERNAL JAVASCRIPT.
- Untuk design WAJIB pakai CSS EXTERNAL, TIDAK BOLEH CSS INTERNAL dan INLINE.
- Saat membuat Header (Nav) dan Footer, WAJIB DIBUAT HTML TERPISAH. Jangan satukan dengan HTML PAGE.
- Custom Font wajib dari Google Font.
- Menikuti Aturan Detail dibawah ini.

## Aturan Penulisan Konten

- Jangan pernah mengubah copywriting yang diberikan user.
- Jangan menambahkan atau mengurangi apapun yang diberikan user.
- Copywriting harus 100% karena itu sudah disesuaikan untuk SEO.

## Aturan Projek

- Pastikan struktur projeknya rapih, assets tempatkan di tempatnya.
- Semua page HTML dan CSS ada di root, jangan masukkan kedalam sub-folder.

## Aturan HTML

- Setiap Page = 1 Full HTML Standalone
- Wajib mengikuti bestpractice SEMANTIC HTML agar SEOnya bagus.
- Wajib mengisi semua ALT IMAGE dengan isi sesuai dengan konteksnya.
- Tidak boleh mengimport Custom Font di HTML karena Custom Font Wajib di CSS.
- Tiap Link Internal untuk pindah antar page wajib "/<slug-page>" dengan mengikuti prinsip href Wordpress Elementor Page dan slugnya harus sesuai dengan nama page .html yang dibuat.
- Untuk External Link tidak ada aturan khusus kecuali harus open in blank page.
- Header dan Footer dipisah, dengan membuat header.html dan footer.html.

## Aturan CSS

- CSS masuk ke Global CSS Elementor yang berlaku sitewide.
- CSS hanya ada 1 dan UNTUK SEMUA PAGE termasuk Header dan Footer.
- Pastikan mengikuti bestpractice CSS dengan mengdefine hal berulang dengan ":root {--<property-css>}"
- Saat menggunakan Custom Font wajib mengimport dari CSS menggunakan CSS "@import".
- Pastikan Mobile First Responsive Breakpoin.

## Aturan JS

- Semua TAG script JS harus inline di dalam body TAG HTML.
- Menerapkan Internal JS.
- Tidak ada file .js terpisah.
- Dilarang menaruh script di dalam head.

# Aturan Accessibility dan Performa

- Semua img wajib ada alt dan ada isinya sesuai konteksnya.
- loading="lazy" untuk semua gambar kecuali LCP image (hero above the fold).
- Semua img wajib ada attribute width dan height untuk mencegah layout shift (CLS).
- Gunakan rel="preload" untuk aset kritis.

## List Link/Informasi External

Berikut adalah Link yang berguna dan akan di pakai mengisi link dari copywriting. Kalau linknya Kosong berarti memang tidak ada dan kalau ada isinya pastikan dipakai!


# FOOTER
- icon wajib menggunakan svg untuk media sosial dibawah ini

TikTok
@halalivechat
https://www.tiktok.com/@chamet.agencyyy
Instagram
@halalivechat
https://www.instagram.com/chametagencyy/
Telegram: https://t.me/chametsupport
