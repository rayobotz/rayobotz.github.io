# Brief Kolaborasi — Aplikasi Belajar N3 (Rayobotz)

Dokumen ini wajib dibaca sebelum mengusulkan atau mengubah apa pun di aplikasi ini.
Ditulis untuk AI lain (mis. ChatGPT) yang terhubung ke repo ini atas permintaan Ray.

## Visi

Aplikasi ini awalnya dibuat Ray untuk pasangannya yang menghadapi JLPT N3 pada Desember 2026.
Tujuannya: mengubah belajar bahasa Jepang yang terasa berat menjadi pengalaman yang ringan,
efektif, dan membuat penggunanya ingin kembali atas kemauannya sendiri.
Ciri khas yang TIDAK boleh hilang: aplikasi ini personal — isinya mengikuti buku
『JLPT N3 この一冊で合格する』(日本語の森) dan materi yang sudah dipelajari penggunanya
bersama sensei lesnya, lengkap dengan catatan pribadi dari Ray di beranda.
Jangka panjang Ray ingin aplikasi ini bisa dipakai masyarakat umum, dan proyek ini adalah
sarana Ray melatih kreativitas, pemecahan masalah, dan kepekaan terhadap pengguna.
Ekspansi publik adalah agenda setelah musim ujian (Desember 2026 / Januari 2027), bukan sekarang.

## Model kolaborasi (disepakati Ray, 28 Oktober 2026)

- AI lain (kamu) = **peninjau & pengusul**: review, ide, draf materi, cek silang sitasi & fakta.
- Muse (Obotz) = **editor & satu-satunya penerbit**: menilai usulan, mengintegrasikan,
  menguji, dan menerbitkan.
- **DILARANG mengedit langsung branch `main`**, terutama file `index.html` di repo
  `rayobotz.github.io`. File itu adalah hasil bangun (build) berisi audio yang disisipkan
  sebagai data URI; mengeditnya langsung akan ditimpa atau merusak jalur penerbitan.
  Sampaikan usulan sebagai teks/PR/branch terpisah untuk ditinjau Muse.
- Sumber kebenaran aplikasi adalah `index.html` di folder sumber (di luar repo ini);
  yang diterbitkan adalah file tunggal hasil regenerasi. Jangan mengusulkan perubahan
  arsitektur tanpa membahasnya dulu.

## Aturan desain (dari Ray, mengikat)

1. Sapaan dulu, panduan kemudian — layar pembuka tidak boleh berupa dinding teks.
   "Baru buka dah capek duluan banyak tulisan" adalah kegagalan desain di sini.
2. Yang wajib dilakukan pengguna: singkat dan di depan. Penjelasan panjang dilipat
   (elemen details / tautan kecil), bukan dihilangkan.
3. Satu misi = 8–10 menit. Sedikit tapi rutin mengalahkan banyak tapi sekali duduk.
4. Kehangatan datang dari sentuhan personal Ray (catatan kecil darinya), bukan dari
   maskot kekanak-kanakan, animasi berat, atau rasa bersalah ala streak.
5. Terjemahan & pembahasan Dokkai TERKUNCI sampai semua soalnya dijawab — ini disengaja
   demi kesiapan ujian. Jangan pernah mengusulkan membukanya lebih awal.
6. Bahasa antarmuka: Bahasa Indonesia yang alami dan hangat. Istilah Jepang memakai
   furigana ruby kecil di atas kanji dengan sakelar on/off (bawaan: menyala).

## Standar konten (mengikat, tanpa kecuali)

1. Contoh kalimat dan soal WAJIB orisinal, ditulis untuk aplikasi ini. DILARANG menyalin
   isi buku mana pun, termasuk buku 日本語の森.
2. Yang boleh diambil dari buku 日本語の森: daftar pola, urutan tema, dan nomor halaman —
   khusus Mode Penguat, karena itu materi yang sudah dipelajari pengguna.
3. Setiap klaim sumber/level harus bisa dibuktikan dengan tautan atau dokumen saat diminta.
   JLPT resmi tidak menerbitkan daftar grammar per level sejak 2010; label level adalah
   hasil audit silang (Minna no Nihongo, Sou Matome, Shin Kanzen Master, TRY!, JLPT Sensei,
   Bunpro) dan harus disebut sebagai rujukan cakupan, bukan "sumber resmi JLPT".
4. Furigana wajib diaudit: ruby seimbang untuk semua kanji di teks Jepang yang tampil.
5. Pilihan ganda: posisi jawaban benar WAJIB diacak saat tampil (sudah diperbaiki
   29 Oktober 2026, commit c8bc53d — jangan sampai regresi). Pengecoh harus masuk akal:
   keluarga pola yang sama atau kesalahan umum pembelajar.
6. Audio listening memakai rekaman penutur asli yang sudah ada; jangan mengganti dengan
   TTS tanpa persetujuan Ray.

## Cara mengusulkan perubahan

Sampaikan: (1) masalah/temuan dengan bukti, (2) usulan konkret, (3) risiko & alternatif,
(4) bagian mana dari aturan di atas yang relevan. Muse akan mengevaluasi secara independen —
termasuk menolak dengan alasan — lalu menerbitkan yang lolos dan memverifikasinya live.

## Pembaruan 29 Oktober 2026 — pivot materi inti

- Pelajaran buatan lama (Review N5, Fondasi N4, dan 15 pelajaran N3: grammar/kosakata/listening/reading/dokkai) DIHAPUS dari aplikasi.
- Yang dulu bernama "Mode Penguat" sekarang adalah MATERI INTI dan tampil sebagai bagian "Materi dari bukumu": 8 tema bunpō (Penjelasan + kuis), 3 deck flashcard kosakata hari 1–12, kuis campuran 70 pola, kuis konteks kosakata. Istilah "Mode Penguat" tidak lagi dipakai di aplikasi.
- "Misi Hari Ini — 3 Langkah" tetap ada sebagai roadmap harian; langkah-langkahnya kini menunjuk unit materi buku (tema bunpō berikutnya, deck kosakata berikutnya, antrean kuis yang skornya belum sempurna).
- Dokkai & Listening: belum ada materi dari buku; tombolnya menampilkan catatan "lagi disiapkan" (Ray belum memutuskan sumber/formatnya). Jangan mengusulkan konten dokkai/listening seolah sudah diputuskan.
- Ekspansi berikutnya mengikuti buku yang sama: pola bunpō 71–88 dst. + kosakata hari 13–15, bertahap.

## Pembaruan 29 Okt 2026 — Ekspansi 1 TERBIT
Ekspansi 1 sudah live (commit f079311): bunpō pola 71–89 sebagai Tema 9 （目的・方法・動作， 7 pola), Tema 10 （ルール・アドバイス, 6 pola), Tema 11 （並列， 6 pola) — masing-masing lengkap Penjelasan + kuis + Latihan Bikin Kalimat — plus 30 kata kosakata lanjutan urut daftar Bab 1 ("batch hari 13–15"; buku tidak punya pembagian hari dan tidak menyediakan arti — arti ditulis untuk aplikasi ini). Semua unit ekspansi TERKUNCI sampai 13 unit inti selesai (gerbang sesuai keputusan Ray), tampil sebagai teaser berkunci. Kuis campuran hanya memakai kolam inti selama ekspansi terkunci. Urutan berikutnya: Kotoba produksi, lalu Dokkai set 1, lalu Chōkai (menunggu keputusan format audio dari Ray).
