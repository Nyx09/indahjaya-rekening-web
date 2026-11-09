# Daftar Rekening — Indah Jaya (Toko Bangunan)

Halaman resmi daftar rekening pembayaran Indah Jaya, live di:
**https://indahjaya-rekening.netlify.app**

## Fitur
- Daftar 3 rekening (BCA ×2, BRI ×1) dengan logo bank
- Tombol **Salin** di tiap kartu — nomor ter-copy ke clipboard tanpa salah ketik (ada feedback "Tersalin"/"Gagal")
- Ikon inline SVG, CSS Tailwind v4 hasil build — dependensi runtime nol

## Rekening
| Bank | No. Rekening | a.n. |
|------|--------------|------|
| BCA | 3710100666 | Lie Farihian |
| BRI | 020701011140500 | Lie Farihian |
| BCA | 3710528445 | Shervia Devi Winoto |

## Deploy
```
netlify deploy --prod --dir .
```
Target site tersimpan di `.netlify/state.json` (di-commit), jadi deploy dari komputer mana pun tetap ke situs yang benar.

## Edit rekening
Kartu rekening ditulis **statis** di `index.html` (cari komentar `Kartu rekening`). Edit angka/nama di sana, lalu deploy ulang.

## Edit style / class Tailwind baru
CSS-nya `tailwind.css` hasil build — kalau menambah class baru, rebuild dulu sebelum deploy:
```
npm install
npm run build:css
```

## PDF & QR
Sumber PDF cetak (2 varian: A4 penuh & A4 Konten A5 dengan QR menuju web ini) beserta asetnya ada di `E:\nexwrap_new\_backup\rekening-pdf`. Tidak disimpan di repo ini agar tidak ter-publish ke website (repo ini hanya web-nya). Untuk regenerate PDF: buka HTML-nya di Edge → Print → Save as PDF.
