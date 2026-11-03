# Prompt: Clone Fitur Website dengan REA + OpenCode

Kumpulan prompt dari video tutorial cloning fitur website menggunakan **REA (Reverse Engineer Anything)**, **OpenCode**, **Next.js**, dan **Supabase**.

Video: [tempel link video di sini]

## Baca dulu sebelum mulai

**Hanya untuk website milik sendiri, atau yang sudah ada izin dari pemiliknya.** Jangan dipakai untuk meniru website, branding, atau tampilan orang lain tanpa izin.

Cara install OpenCode, setup REA, dan membuat project Next.js ada di video.

## Ganti placeholder sebelum dipakai

| Placeholder | Ganti dengan | Contoh |
|---|---|---|
| `[NAMA_FITUR]` | Nama fitur yang mau diselidiki | AI chat |
| `[URL_TARGET]` | URL halaman fitur di website target | https://contoh.com/chat |
| `<PROJECT_REF>` | Project ref Supabase milikmu | ada di dashboard Supabase |

## Urutan pemakaian

| Urutan | File | Mode OpenCode |
|---|---|---|
| 1 | [1-investigasi.md](1-investigasi.md) | Build |
| 2 | [2-rencana.md](2-rencana.md) | Plan |
| 3 | [3-build.md](3-build.md) | Build |

Tekan `Tab` di OpenCode untuk berpindah antara Plan dan Build.

## Catatan

- Pakai **project Supabase baru khusus clone**, jangan pernah database production.
- Isi `.env.local` (URL Supabase, anon key, API key AI) sendiri. Jangan tempel key ke chat agent.
- Hasil investigasi REA dari luar hanya mencakup yang terlihat di browser. Logika server, prompt sistem, dan skema database asli tidak ikut terbaca, jadi hasil clone akan berbeda di bagian itu.
- Perintah dan perilaku REA serta OpenCode bisa berubah di versi baru. Kalau ada yang tidak cocok, cek README REA dan dokumentasi OpenCode terbaru.

---

Dibuat oleh RVL. Github Radar tersedia di [rvllabs.id](https://rvllabs.id).
