BIRTHDAY WEBSITE — GSAP

CARA MENJALANKAN
1. Extract file ZIP.
2. Buka folder birthday_website.
3. Jalankan index.html dengan browser. Untuk hasil terbaik, gunakan VS Code + ekstensi Live Server.

YANG BISA DIUBAH
- Buka index.html, cari bagian `const CONFIG` untuk mengganti nama penerima dan pengirim.
- Ganti tulisan tanggal ulang tahun pada bagian `.date` (saat ini 22 AUGUST).
- Foto kenangan: di bagian `#memories`, ganti elemen <div class="photo"> dengan:
  <div class="photo"><img src="assets/foto-1.jpg" alt="Kenangan kami"></div>
  Salin foto ke folder assets dan sesuaikan nama filenya.
- Video: letakkan video MP4 bernama `special-video.mp4` di folder assets.
- Musik latar belum dipasang agar audio video tidak bertabrakan. Musik bisa ditambahkan setelah file musik tersedia.

ANIMASI
- GSAP 3 + ScrollTrigger dimuat dari CDN, jadi koneksi internet diperlukan.
- Klik “Open Your Surprise”: teks intro menghilang, tirai kiri/kanan terbuka, lalu halaman ulang tahun tampil.
- Scroll memicu animasi reveal tiap section; kartu foto memiliki animasi masuk dan tombol navigasi titik mengikuti section aktif.

CATATAN
- Nama Thraveen dan Kamali serta tanggal 22 August diisi mengikuti referensi gambar. Silakan sesuaikan.
- Foto dan video masih berupa placeholder sampai kamu memasukkan file milikmu.

FITUR TAMBAHAN
- Section 3 (Our Precious Memories) kini memiliki tiga bunga pink yang tumbuh: batang naik, daun terbuka, kelopak mekar satu per satu, lalu bunga bergoyang lembut. Animasi dipicu saat section masuk viewport dan berjalan sekali.

PERBAIKAN ANIMASI BUNGA
- Animasi bunga section 3 diperbaiki: batang tumbuh, daun membuka, kelopak menyebar radial dari pusat dengan GSAP, pusat bunga muncul, lalu bunga bergoyang.
- Trigger memakai section #memories agar animasi tetap terpanggil saat section terlihat setelah intro dibuka.
