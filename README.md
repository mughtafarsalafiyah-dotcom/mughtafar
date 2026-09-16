# Website Angkatan Mughtafar — Salafiyah Pasuruan

Website resmi Angkatan Mughtafar, terhubung ke [Supabase](https://supabase.com) untuk database, autentikasi admin, dan penyimpanan foto.

## Struktur
- `index.html` — seluruh website (HTML, CSS, JS) dalam satu file, tanpa proses build.

## Setup Supabase
Kredensial Supabase (Project URL & anon/publishable key) sudah tertanam langsung di `index.html` (lihat bagian `SUPABASE CONFIG` di tag `<script>` paling bawah).

## Deploy ke Vercel
1. Push repo ini ke GitHub.
2. Di [vercel.com](https://vercel.com), klik **Add New → Project**, lalu import repo ini.
3. Vercel akan otomatis mendeteksi ini sebagai static site — tidak perlu build command khusus.
4. Setelah deploy pertama, setiap `git push` ke branch utama akan otomatis membuat deployment baru.

## Status migrasi ke Supabase
- ✅ Anggota — sudah pakai Supabase (database + storage foto)
- ⏳ Dokumentasi/Album, Quotes, Artikel, Pengurus, Pengaturan — masih pakai localStorage (migrasi menyusul)
