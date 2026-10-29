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

---

## Pembaruan 29 Oktober 2026 (sore) — Dokkai set 1 TERBIT & prinsip pengingat Minna

**Dokkai set 1 sudah live** (commit b7deb51, terverifikasi 6/6): 4 teks orisinal — pengumuman perpustakaan （短文）, email perubahan rencana （短文）, pamflet kelas memasak (pencarian info bersyarat), esai pengalaman （中文）; total 9 soal. Model tipe soal & tingkat kesulitan mengacu pada 『新完全マスター読解 N3』 dan 『JLPT N3 完全模試』 (keduanya milik Ray, dibedah strukturnya); tema kosakata mengikuti bukunya. Setiap teks dilengkapi strategi membaca + satu tips praktis berbahasa Indonesia sederhana di intro, 4 kartu kata kunci dari teks, dan terjemahan+pembahasan yang terkunci sampai semua soal dijawab. Kategori Dokkai kini aktif (sebelumnya hanya catatan "lagi disiapkan"); misi inti & gerbang Ekspansi tidak berubah.

**Prinsip konten baru — "pengingat Minna":** bila konsep N3 membingungkan, penjelasan boleh menyisipkan satu baris pengingat ke konsep serupa di buku level dasar (Minna no Nihongo I/II), dengan syarat: (1) sifatnya hanya jembatan ingatan, BUKAN materi yang harus dipelajari; (2) ditulis jujur bahwa penyajiannya berbeda di level dasar; (3) rujukan jilid/bab wajib diverifikasi dari PDF Minna milik Ray sebelum ditulis — tidak boleh mengarang nomor bab.

**Aturan sitasi (tegas dari Ray, 29 Okt 2026 sore):** daftar "Sumber & kejujuran materi" hanya boleh memuat rujukan yang BENAR-BENAR dipakai materi yang ada di aplikasi saat ini. Seri warisan dari pelajaran lama yang sudah dihapus (Sou Matome, TRY!, Shin Kanzen Master generik) sudah dibuang dari daftar; model Dokkai kini dicantumkan spesifik (『新完全マスター読解 N3』 + 『JLPT N3 完全模試』, perannya: tipe soal, panjang teks, tingkat kesulitan). Bila kelak ada materi baru memakai rujukan baru, sitasi ditambah SAAT materi itu terbit — bukan sebelumnya. Minna no Nihongo juga belum dicantumkan karena pengingat Minna belum diterapkan di konten mana pun.

## Chōkai set 1–2 (29 Okt 2026 — TERBIT)
- Ray menyetujui (29 Okt 2026) audio TTS dua penutur untuk materi Chōkai BARU (pengecualian sadar dari aturan "jangan ganti audio penutur asli dengan TTS" — ini konten baru tanpa rekaman asli, dan di dalam aplikasi diberi label jujur "Suara: TTS (sintetis)"). Urutan tipe soal: 即時応答 → ポイント理解 → 課題理解 → 概要理解 → 発話表現 (terakhir, butuh ilustrasi).
- Set 1–2: 即時応答 2×5 soal; transkrip terkunci sampai menjawab. Audio tertanam di berkas aplikasi dan diubah jadi blob URL saat diputar (kendala teknis penerbitan; jangan diusulkan diubah tanpa cek ke Muse).
- Sitasi ditambah saat materi ini terbit: 『JLPT N3 完全模試』(J Research) sebagai model tipe soal Chōkai — sesuai aturan sitasi (ditulis ketika materinya benar-benar terbit).
