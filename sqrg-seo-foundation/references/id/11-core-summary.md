# Ringkasan Inti SQRG (Referensi Cepat)

> Peta konsep paling penting dari SQRG 11 Sep 2025, dalam bahasa sendiri. Cukup untuk kebanyakan tugas. Untuk detail dan contoh, buka file bernomor yang dirujuk di tiap bagian.

## 1. Apa itu SQRG dan apa yang bukan

- Panduan untuk **rater manusia** yang menilai kualitas hasil pencarian Google. Rating mereka dipakai untuk **mengukur dan memperbaiki** sistem pencarian, bukan untuk menaikkan/menurunkan halaman tertentu. Satu rating tidak berdampak langsung pada ranking.
- Nilai SQRG untuk SEO: menunjukkan **standar kualitas yang ingin dicapai** sistem Google. Jangan menyebutnya "faktor ranking".
- Dua penilaian utama: **Page Quality (PQ)**, tidak bergantung query, dan **Needs Met (NM)**, bergantung query. → `01`, `10`

## 2. Page Quality dalam satu halaman

**Tiga langkah:** (1) tujuan sebenarnya merugikan atau menipu? → Lowest. (2) Berpotensi merugikan, tidak tepercaya, atau spam? → Lowest. (3) Jika tidak, nilai seberapa baik halaman mencapai tujuannya. → `02`

**Skala:** Lowest · Low · Medium · High · Highest (plus nilai antara). Ragu antara dua → pilih yang lebih rendah. → `07`

**Faktor:** tujuan halaman; tingkat YMYL; tipe situs; info tentang situs/kreator; kualitas MC; judul; peran iklan/SC; reputasi; Trust (E-E-A-T). Faktor-faktor ini saling memengaruhi. → `02`

**YMYL:** topik yang bisa berdampak signifikan pada kesehatan/keselamatan, keuangan, pemerintahan/kewargaan/masyarakat, atau kesejahteraan. Bersifat spektrum. Uji cepat: apakah orang yang hati-hati akan mencari ahli? Apakah cukup bertanya santai ke teman? → `01`

**MC / SC / Ads:** MC = yang langsung mencapai tujuan (termasuk judul dan isi di balik tab); SC = pendukung (navigasi, dll.); Ads = semua monetisasi, termasuk link afiliasi. **Ada atau tidaknya iklan, dengan sendirinya, bukan alasan rating naik atau turun.** → `01`

**Kualitas MC = effort + orisinalitas + bakat/skill + akurasi** (akurasi dan konsensus ahli wajib untuk informasi/YMYL). Konten otomatis massal tanpa kurasi ≠ effort. → `02`

**E-E-A-T:** Experience, Expertise, Authoritativeness mendukung **Trust**, yang paling penting. Halaman tidak tepercaya = E-E-A-T rendah, seberapa ahli pun. YMYL: saran dan info faktual sebaiknya dari ahli; berbagi pengalaman hidup boleh selama aman dan sesuai konsensus. → `02`, `07`

**Reputasi:** dari sumber independen, bukan klaim situs sendiri. Untuk YMYL, dari ahli di bidangnya. Data traffic bukan bukti reputasi. Tidak ada info reputasi ≠ tanda buruk untuk situs kecil. → `02`

## 3. Pemicu rating (satu saja cukup)

**Lowest** → `03`, `04`
- Tujuan merugikan/menipu; dibuat untuk untung pemilik dengan hampir nol upaya membantu.
- Merugikan diri/orang lain, kelompok tertentu, atau informasi menyesatkan yang berbahaya.
- Sama sekali tanpa info penanggung jawab untuk YMYL atau situs yang menangani uang/data.
- Reputasi sangat negatif; sangat tidak tepercaya.
- MC sengaja ditutupi iklan/pop-up/interstitial.
- Judul sangat menyesatkan atau sensasional.
- Diretas, dirusak, dipenuhi komentar spam; teks acak.
- **Spam:** expired domain abuse, site reputation abuse, scaled content abuse, dan MC yang seluruhnya/hampir seluruhnya disalin, diparafrase, di-embed, dibuat otomatis/AI, atau di-repost **tanpa effort, orisinalitas, dan nilai tambah** (tetap Lowest walau sumber dikredit).
- Profil penulis palsu (termasuk persona AI), klaim keahlian palsu, klaim "sudah diuji" yang palsu.

**Low** → `05`
- MC kurang effort/orisinalitas/skill; ketidakakuratan ringan.
- Banyak MC hasil kemas ulang dengan sedikit nilai tambah.
- Filler banyak atau menonjol sehingga MC sulit ditemukan.
- Judul sedikit menyesatkan atau dilebih-lebihkan.
- Iklan/SC sangat mengganggu.
- Info situs/kreator kurang memuaskan untuk tujuannya (terutama toko dan YMYL).
- Reputasi agak negatif; klaim keahlian dibesar-besarkan.
- E-E-A-T tidak memadai untuk topiknya. Reputasi situs yang bagus **tidak** menutupi ini.

**Medium** → `05`: tujuan tercapai; "tidak ada yang salah, tidak ada yang istimewa", atau campuran tanda High dan tanda Low ringan. Halaman "rata-rata" ada di sini.

**High** → `06`: syarat dasar terpenuhi, plus minimal satu: MC dengan effort/orisinalitas/skill tinggi; reputasi positif; E-E-A-T tinggi.

**Highest** → `06`: hal yang sama di level "sangat": konten terbaik di topiknya, reputasi sangat positif, atau sumber otoritatif yang unik.

## 4. Konten AI menurut SQRG (rangkuman lintas bagian)

- AI generatif didefinisikan sebagai **alat** yang bisa membantu atau disalahgunakan. **Pemakaian AI saja tidak menentukan rating.** → `01`, `03`
- Yang dinilai: effort, orisinalitas, nilai tambah, akurasi, dan kejujuran. AI tanpa kurasi untuk produksi massal = scaled content abuse. Seluruh MC hasil AI tanpa nilai tambah = Lowest. → `03`
- Tanda yang dikenali rater: sisa kalimat khas chatbot, kalimat terpotong, kesalahan fakta yang janggal, jawaban yang masuk akal per kalimat tapi tidak nyambung, situs yang membahas topik apa saja di luar fokusnya, format tanya-jawab massal dari pertanyaan "People Also Ask". → `04`
- Persona penulis buatan AI = info menipu → Lowest. → `03`

## 5. Needs Met dalam satu halaman

**Skala:** FullyM (khusus query dengan satu target spesifik: situs tertentu atau fakta Know Simple, dan **hampir semua** pengguna puas) · HM (sangat membantu; **rating tertinggi yang mungkin untuk kebanyakan query**) · MM (membantu, rata-rata sampai bagus) · SM (kurang membantu, atau membantu untuk interpretasi yang tidak mungkin) · FailsM (gagal, melenceng, salah, basi, atau tidak berguna). → `09`

**Prinsip kunci:** → `09`, `10`
- Pahami query dulu: interpretasi (dominan, common, minor wajar, minor tak mungkin, no chance) dan intent (Know/Know Simple, Do, Website, Visit-in-Person). → `08`
- **Melewatkan aspek kunci query** (tahun, lokasi, "non", perbandingan) → FailsM, bukan SM.
- Hasil tidak berguna = FailsM walau PQ-nya tinggi. Halaman PQ sangat rendah (penipuan, teks acak) = FailsM, kecuali query navigasi ke situs itu sendiri.
- Judul yang sangat menyesatkan di SERP → SM atau lebih rendah.
- Query yang butuh konten segar (berita, acara berulang, harga, produk): konten basi → rendah sampai FailsM.
- Query dalam bahasa locale → pengguna ingin hasil dalam bahasa locale, termasuk saat mengetik nama diri atau kata Inggris dalam huruf Latin. Pengecualian: situs resmi global yang dicari, info teknis yang memang berbahasa Inggris.
- Hasil yang beragam (format, perspektif, kedalaman, jenis situs) bisa sama-sama HM.
- Untuk query lokal, "dekat" tergantung jenis tempatnya.

## 6. Lima pertanyaan inti sebelum menerbitkan konten

1. Apa tujuan halaman ini, dan apakah benar-benar untuk membantu pembaca? → `01`
2. Seberapa YMYL topiknya, dan apakah tingkat akurasi serta keahliannya sudah sepadan? → `01`, `02`
3. Apa nilai tambah halaman ini dibanding hasil teratas yang sudah ada? → `03`, `05`
4. Apakah pengalaman, keahlian, dan identitas penulis/penerbit terlihat dan bisa diverifikasi? → `02`
5. Untuk keyword targetnya, apakah halaman ini menjawab intent dominan secara langsung, lengkap, mutakhir, dan dalam bahasa yang tepat? → `08`, `09`, `10`

Untuk audit lengkap, pakai `12-audit-checklist.md`.
