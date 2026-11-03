Gunakan REA untuk menyelidiki fitur [NAMA_FITUR] di [URL_TARGET].
Amati sebagai black box (browser, network, JS klien, CSS). Jangan minta source code.
Tulis file hanya di rea-results/. Isi dalam Bahasa Indonesia; nama field, properti CSS,
dan penanda UNKNOWN/INFERRED tetap Inggris. Lakukan maksimal [5] interaksi uji yang
singkat dan aman (tanpa data sensitif, tanpa aksi yang merusak atau berbayar).

Aturan efisiensi (penting):
- Buat MAKSIMAL 2 script bantu, simpan di rea-results/_probe/. Satu script untuk baca
  computed CSS, satu untuk menangkap network/streaming. Jangan bikin script baru
  per pertanyaan; ubah script yang ada.
- Ambil computed CSS hanya untuk komponen utama (input, tombol kirim, bubble pesan,
  card). Skip hover/focus/mobile kecuali sudah sempat dan murah.
- Kalau satu cara gagal, coba maksimal 2x lalu tandai UNKNOWN dan lanjut.
- Jangan simpan dump besar; ringkas output langsung, simpan hanya yang dipakai.
- Setelah CLONE_SPEC.md selesai, hapus file sementara di rea-results/_probe/ kecuali script-nya.

Tulis rea-results/CLONE_SPEC.md, ringkas dan berbentuk tabel/poin, berisi:

1. UI/UX: warna, tipografi, radius, bayangan, padding/margin/gap komponen utama (nilai asli dari computed CSS), plus state loading/kosong/disabled. Ambil screenshot halaman fitur ini: 1 di desktop (1280px) dan 1 di mobile (375px), simpan di rea-results/screenshots/ (desktop.png dan mobile.png). Jangan ambil screenshot lain. Kalau gagal, coba maksimal 2x lalu tandai UNKNOWN.

2. Perilaku: alur pengguna, state yang muncul, dan cara data dikirim/diterima (biasa, polling, streaming, websocket, dll.)

3. Data: endpoint + bentuk request/response, field entitas (tipe + contoh singkat), tempat data disimpan, dan draf tabel database berlabel INFERRED.

Aturan: bukti singkat tiap klaim, yang belum pasti tandai UNKNOWN, sensor
key/token/cookie, jangan salin kode/aset/branding, jangan query API/database di luar
yang diminta aplikasi itu sendiri, jangan tulis implementasinya.
Akhiri dengan daftar "Tidak bisa diamati dari luar".
