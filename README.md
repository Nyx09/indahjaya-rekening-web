# Daftar Rekening — Indah Jaya (Toko Bangunan)

Halaman resmi daftar rekening pembayaran Indah Jaya, live di:
**https://indahjaya-rekening.netlify.app**

## Fitur
- Daftar 3 rekening (BCA ×2, BRI ×1) dengan logo bank
- Tombol **Salin** di tiap kartu — nomor ter-copy ke clipboard tanpa salah ketik
- Catatan keamanan transfer (waspada modus — nama penerima harus sesuai)
- Tailwind CSS v4 (browser CDN) + ikon Lucide
- Dependensi nol — statis murni, deploy ke mana saja

## Rekening
| Bank | No. Rekening | a.n. |
|------|--------------|------|
| BCA | 3710100666 | Lie Farihian |
| BRI | 020701011140500 | Lie Farihian |
| BCA | 3710528445 | Shervia Devi Winoto |

## Deploy
Netlify CLI:
```
netlify deploy --prod --dir .
```
atau hubungkan repo ini langsung di Netlify (publish dir: `.`).

## Edit rekening
Edit array `accounts` di `index.html`, lalu deploy ulang.
