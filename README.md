# Serambi Fokus

Ruang fokus bersuasana alam: pemandangan (alam, laut dan akuarium, kota), cuaca (hujan, panas, salju, badai angin, debu dan pasir), timer fokus, waktu sholat dan adzan, widget Al-Qur'an karaoke, kalender Hijriah, hadis, arah kiblat, pemutar MP3, catatan, task terjadwal, running text, dan screensaver.

Satu file HTML, tanpa build, tanpa npm, tanpa server. Semua data pengguna tersimpan di browser pengguna sendiri.

## Mencoba secara lokal

Buka `index.html` di browser. Widget yang memanggil internet (Al-Qur'an, hadis) lebih andal bila situs dibuka lewat `https://` (hosting), bukan dari file lokal.

## Memasang di GitHub Pages

1. Buat repositori **public** baru, unggah semua file di folder ini (termasuk `.nojekyll`).
2. Buka **Settings > Pages**. Pada "Source" pilih **Deploy from a branch**, pilih branch `main` dan folder `/ (root)`, lalu simpan.
3. Tunggu beberapa menit. Alamat situs muncul di halaman Pages.

## Memasang di Cloudflare Pages

**Workers & Pages > Create application > Pages > Drag and drop your files**, lalu unggah folder ini. Putuskan sejak awal antara unggah langsung atau sambung ke Git, karena proyek unggah langsung tidak bisa dialihkan ke Git nanti.

## Data dan privasi

Pengaturan, catatan, foto latar, logo sponsor, daftar MP3, file adzan, dan ukuran ikan disimpan di browser pengguna (localStorage dan IndexedDB). Tidak ada akun dan tidak ada server milik aplikasi. Pengguna dapat memindahkan data lewat **Workspace > Pengaturan > Cadangan data** (unduh dan pulihkan), dan melindunginya lewat tombol **Lindungi data**. Lihat `privacy.html`.

## Layanan pihak ketiga (periksa syaratnya sebelum penggunaan komersial)

| Layanan | Dipakai untuk | Status syarat |
|---|---|---|
| api.alquran.cloud dan islamic.network (CDN audio) | Teks Arab, terjemahan Indonesia, audio per ayat | Syarat dibaca 8 Nov 2026: teks boleh dipakai bebas untuk non-komersial; untuk komersial tidak perlu izin tetapi pencantuman sumber diminta; audio qari berlisensi non-komersial, boleh dikemas ke produk komersial tetapi hak cipta ada pada qari yang dapat meminta penghapusan |
| mp3quran.net | Daftar qari dan audio per surah | Syarat penggunaan belum diverifikasi. Hubungi pengelola sebelum penggunaan komersial |
| api.myquran.com | Hadis acak | Syarat penggunaan belum diverifikasi. Hubungi pengelola sebelum penggunaan komersial |

Tampilkan sumber data di aplikasi (sudah ada di widget) dan jangan menyalin atau menjual ulang konten atau file audio mereka sebagai paket data.

Foto latar yang diunggah pengguna menjadi tanggung jawab pengguna. Periksa lisensi tiap foto (misalnya dari Pexels) sebelum memakainya pada produk komersial.

## Menyesuaikan

Semua kode ada di `index.html`. Titik awal yang berguna: daftar pemandangan (`const SC=[...]`), nilai bawaan pengaturan (`const CFD={...}`), lokasi sholat bawaan (`const PL={...}`), dan teks credit di bagian bawah halaman.

## Lisensi

**PolyForm Noncommercial License 1.0.0** (lihat `LICENSE`). Gratis untuk penggunaan **nonkomersial**: pribadi, hobi, belajar, penelitian, ibadah, serta organisasi nirlaba, lembaga pendidikan, dan lembaga pemerintah. Kamu boleh mengubah dan membagikannya untuk tujuan nonkomersial selama menyertakan file `LICENSE` dan baris `Required Notice`.

**Penggunaan komersial memerlukan lisensi tertulis terpisah**, misalnya menjual, memakainya dalam produk atau layanan berbayar, atau menjalankannya untuk kepentingan perusahaan. Kontak: farmatrance@gmail.com

Lisensi ini berlaku untuk kode aplikasi saja. Layanan, data, dan audio pihak ketiga memiliki syarat sendiri (lihat bagian di atas), dan lisensi ini tidak mengubahnya. Lisensi ini termasuk *source-available*, bukan *open source* menurut definisi OSI.

## Jasa kustom

Pemegang hak cipta dapat menawarkan versi kustom (merek, tema, running text sponsor) dan lisensi komersial sebagai layanan berbayar.
