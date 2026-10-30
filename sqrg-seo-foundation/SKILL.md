---
name: "sqrg-seo-foundation"
description: "Fondasi standar kualitas konten SEO berbasis Google Search Quality Rater Guidelines (SQRG) edisi 11 September 2025: Page Quality, E-E-A-T, YMYL, kriteria Lowest sampai Highest, kebijakan spam (scaled content abuse, site reputation abuse, expired domain abuse), konten AI, intent pencarian, dan skala Needs Met. Gunakan setiap kali user mengaudit atau menilai kualitas artikel, halaman, atau situs; bertanya soal E-E-A-T, YMYL, helpful content, atau apakah konten AI aman untuk SEO; menentukan intent keyword; membandingkan konten dengan pesaing; atau butuh standar kualitas saat membuat outline dan menulis artikel, termasuk saat skill SEO lain sedang dipakai. Pakai juga walau user tidak menyebut SQRG, misalnya 'artikel ini sudah bagus belum', 'kenapa halaman ini susah ranking', 'cek E-E-A-T', atau 'aman nggak pakai AI untuk artikel kesehatan'. English triggers: quality rater guidelines, page quality audit, E-E-A-T review, YMYL, needs met, search intent, spam policies."
---

# SQRG SEO Foundation

Skill ini adalah basis pengetahuan dan alat kerja untuk menilai serta merancang konten menurut standar yang dipakai rater Google dalam **Search Quality Rater Guidelines (SQRG) edisi 11 September 2025**. Isinya ditulis ulang dengan bahasa sendiri (bukan teks Google), dengan rujukan bagian dan halaman PDF asli. Sebagai pelengkap, `14-spam-policies.md` merangkum **kebijakan spam Google Search** (dokumen Search Central yang terpisah dari SQRG).

## Struktur dua bahasa

File referensi tersedia dalam dua versi yang setara, dengan **nama file, urutan bagian, dan rujukan halaman yang sama**:
- `references/en/`: bahasa Inggris. Paling mudah dicocokkan dengan PDF asli dan biasanya lebih hemat token.
- `references/id/`: bahasa Indonesia. Untuk dibaca tim dan saat butuh kutipan berbahasa Indonesia.

**Baca satu versi saja per tugas** supaya konteks tidak terisi dua kali. Default: `references/en/`. Pakai `references/id/` jika user meminta teks referensi berbahasa Indonesia atau ingin membaca file referensinya sendiri. Bahasa jawaban ke user tetap mengikuti bahasa user.

## Prinsip kerja

1. **SQRG bukan daftar faktor ranking.** SQRG adalah panduan bagi rater manusia untuk mengevaluasi sistem pencarian; rating mereka tidak mengubah ranking halaman secara langsung. Sampaikan SQRG sebagai standar kualitas yang ingin dicapai sistem Google. Jangan menjanjikan kenaikan ranking.
2. **Bedakan tiga jenis klaim:** (a) isi SQRG, dengan rujukan bagian/halaman, misalnya "SQRG 4.6.5, hal. 42", atau isi kebijakan spam, dengan rujukan nama bagian, misalnya "Spam policies › Link spam"; (b) catatan praktik berlabel **[Application]**/**[Penerapan]**; (c) penilaianmu sendiri.
3. **Jangan mengarang aturan.** Jika situasi tidak dibahas SQRG, katakan begitu, lalu nilai berdasarkan prinsip umumnya (tujuan halaman, bahaya, effort, Trust).
4. **Urutan berpikir rater:** cek bahaya, penipuan, dan spam dulu; baru kualitas. Ragu antara dua rating → pilih yang lebih rendah. Rating adalah perkiraan, sertakan alasannya.
5. **Dua hal yang sering disalahpahami:** iklan saja tidak menurunkan rating, dan pemakaian AI saja tidak menentukan rating. Yang dinilai adalah effort, orisinalitas, nilai tambah, akurasi, dan kejujuran.
6. **Bahasa jawaban:** ikuti bahasa user (default Indonesia). Istilah teknis SQRG (Page Quality, Needs Met, MC, YMYL, E-E-A-T, Highly Meets, dll.) boleh tetap dalam bahasa Inggris.
7. **Redaksi persis:** file referensi berisi parafrase. Jika user butuh kata-kata persis Google, cek apakah ada PDF di `source/` (lihat `source/README.md`); jika ada, baca halaman terkait dengan `pdftotext -f N -l N` dan kutip seperlunya. Jika tidak ada, arahkan user ke halaman PDF yang relevan.
8. **Versi:** jika user menanyakan edisi terbaru dan web search tersedia, cari dulu. Status versi dan cara update ada di `13-changelog.md`. Saat memperbarui skill, ubah **kedua** versi bahasa pada file dan nomor bagian yang sama.

## Peta file referensi

Mulai dari `11-core-summary.md` untuk hampir semua tugas, lalu buka file bernomor sesuai kebutuhan. Peta lengkap dengan cakupan halaman ada di `00-index.md`.

| Kebutuhan | File (di `en/` atau `id/`) |
|---|---|
| Gambaran cepat seluruh konsep | `11-core-summary.md` |
| Audit halaman/artikel, review sebelum terbit | `12-audit-checklist.md` (+ file yang dirujuk di dalamnya) |
| Tujuan halaman, YMYL, MC/SC/Ads, identitas situs dan kreator | `01-pq-basics.md` |
| Kualitas MC, reputasi, E-E-A-T, pengalaman vs keahlian di YMYL | `02-pq-reputation-eeat.md` |
| Spam, konten AI/massal, salinan/parafrase, penipuan, konten berbahaya | `03-pq-lowest.md` |
| Contoh kasus Lowest | `04-pq-lowest-examples.md` |
| Konten biasa saja: filler, judul berlebihan, repackaging, Medium | `05-pq-low-medium.md` |
| Target kualitas tinggi dan benchmark | `06-pq-high-highest.md` |
| Forum/UGC, halaman 404/error, ensiklopedia, FAQ konseptual | `07-pq-special-pages.md` |
| Intent keyword, interpretasi query, locale | `08-user-intent.md` |
| Skala Needs Met dan contohnya | `09-needs-met-scale.md` |
| Produk, lokal, freshness, bahasa, PQ vs NM, flag | `10-needs-met-special-cases.md` |
| Versi, riwayat perubahan, cara update skill | `13-changelog.md` |
| Kebijakan spam Google (di luar SQRG): cloaking, doorway, redirect, teks tersembunyi, link spam, thin affiliation, site reputation + EEA, manual action | `14-spam-policies.md` |

## Alur kerja per jenis tugas

### A. Audit artikel, halaman, atau situs
1. Baca `11-core-summary.md` dan `12-audit-checklist.md`.
2. Kumpulkan bahan: isi halaman (fetch URL jika diberikan dan tool tersedia), keyword target, info penulis dan situs. Jika memungkinkan, lihat beberapa halaman lain di situs yang sama (pola spam dan template terlihat dari beberapa halaman) dan beberapa hasil teratas pesaing untuk kalibrasi.
3. Jalankan checklist secara berurutan. Buka file detail sesuai temuan: sinyal AI/massal/affiliate → `03` dan `04`; YMYL → `01` bagian 4 dan `02` bagian 5–6; ada keyword target → `08`, `09`, `10`; sinyal spam teknis atau link (redirect aneh, teks tersembunyi, halaman per kota, link berbayar, bagian pihak ketiga) → `14`.
4. Tulis laporan dengan template di akhir checklist. Sertakan bukti dari halaman dan rujukan bagian SQRG untuk setiap temuan.

### B. Membuat outline atau menulis artikel (termasuk saat skill SEO lain dipakai)
Gunakan skill ini sebagai **standar kualitas**, bukan pengganti skill penulisan. Sebelum atau saat menyusun brief/outline, tentukan:
- intent dominan dan interpretasi minor yang wajar (`08`);
- tingkat YMYL dan jenis E-E-A-T yang dibutuhkan: pengalaman, keahlian, atau sumber resmi (`01`, `02`);
- rencana nilai tambah: apa yang akan ada di artikel ini dan tidak ada di hasil teratas (`03` bagian 7, `06` bagian 2);
- struktur yang menaruh jawaban di atas dan menghindari filler, serta judul yang jujur (`05` bagian 3);
- kebutuhan kesegaran dan bahasa (`10` bagian 6 dan 11).
Sebelum menyerahkan hasil akhir, jalankan Tahap 1 dan 2 checklist secara ringkas.

### C. Riset keyword dan intent
Baca `08`, lalu `09` dan `10` untuk memperkirakan jenis hasil apa yang akan dianggap Highly Meets. Petakan setiap keyword ke jenis intent, interpretasi, kebutuhan format, kesegaran, dan lokalitas.

### D. Analisis pesaing atau "kenapa halaman ini sulit ranking"
Perkirakan PQ dan Needs Met untuk halaman user dan pesaing dengan kriteria yang sama, lalu tunjukkan selisihnya (nilai tambah, E-E-A-T, kecocokan intent, kesegaran). Sampaikan sebagai hipotesis kualitas, bukan penjelasan pasti tentang algoritma.

### E. Konten AI atau produksi massal
Baca `11-core-summary.md` bagian 4, `03` bagian 7.5–7.6, `04` kelompok F, dan `14` bagian 1 dan 5 (kebijakan spam kini juga mencakup manipulasi jawaban AI generatif). Fokus pada effort, kurasi, verifikasi fakta, nilai tambah per halaman, dan kejujuran identitas penulis.

### F. Topik YMYL (kesehatan, keuangan, hukum/pemerintahan, keselamatan)
Baca `01` bagian 4, `02` bagian 5–6, `03` bagian 3–5, dan FAQ di `07`. Tekankan akurasi, konsensus ahli, pedoman resmi terbaru, dan keahlian penulis atau reviewer.

### G. E-commerce, review produk, affiliate
Baca `01` bagian 6, `03` bagian 6.3, `05`, `06`, `10` bagian 9, dan `14` bagian 5.3, 6.2, dan 7 (thin affiliation, bagian pihak ketiga, atribut link). Cek bukti pengalaman langsung, info layanan pelanggan dan kebijakan, serta konflik kepentingan.

### H. Konten lokal atau multibahasa
Baca `08` bagian 3–4 dan 7.4, serta `10` bagian 10–11.

### I. Pertanyaan konseptual tentang SQRG
Jawab dari `11-core-summary.md`, lalu perdalam dengan file bernomor yang relevan. Jawab langsung dan ringkas, dengan rujukan bagian.

## Yang harus dihindari
- Menyarankan taktik yang disebut SQRG sebagai penipuan: persona penulis fiktif atau foto penulis buatan AI, klaim pengujian palsu, kredensial palsu, review "independen" yang ditulis produsen, iklan yang menyamar sebagai konten.
- Menyebut konten buruk hanya karena memakai AI atau karena ada iklan.
- Menganggap halaman tanpa info reputasi otomatis buruk (wajar untuk situs kecil dan orang biasa).
- Menyajikan catatan [Application]/[Penerapan] atau pendapat sendiri seolah-olah isi SQRG.
