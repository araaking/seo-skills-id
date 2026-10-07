---
name: seo-article-writer
description: Tulis artikel SEO bahasa Indonesia yang lengkap dan siap terbit dari topik, keyword, brief, atau outline (termasuk hasil seo-content-outline), lengkap dengan tabel meta, H2/H3, FAQ, referensi, dan catatan editor, untuk niche umum, bisnis, gaya hidup, maupun YMYL (kesehatan, klinik, skincare, obat, keuangan, hukum). Output langsung rapi di tempat tujuannya, yaitu Markdown siap salin di chat (Claude, ChatGPT), Google Docs lewat connector atau Google Workspace API, atau file .docx, tanpa bullet ganda, tabel rusak, atau jarak berantakan. Gunakan skill ini setiap kali user meminta menulis, membuat, mengembangkan, atau menulis ulang artikel, artikel blog, konten SEO, naskah, atau draf, misalnya "tulisin artikelnya", "kembangkan outline ini jadi artikel", atau "buat artikelnya di Google Docs", walau tidak menyebut kata SEO. Bukan untuk membuat outline saja (pakai seo-content-outline) atau meta tag saja (pakai seo-meta-generator). English triggers - write SEO article, blog post, long-form article from outline, Indonesian article, article to Google Docs or docx.
---

# SEO Article Writer

Ubah topik, brief, atau outline menjadi artikel SEO bahasa Indonesia yang menjawab kebutuhan pembaca, akurat, bebas pola tulisan AI, dan **rapi di tempat tujuannya tanpa perlu dirapikan manual**.

## File Referensi

| File | Isi | Kapan dibaca |
|---|---|---|
| [references/output-channels.md](references/output-channels.md) | Cara menyajikan artikel di chat, Google Docs (connector atau API), .docx, dan teks polos, beserta template HTML dan pemeriksaan hasil | **Sebelum menulis**, untuk menentukan channel |
| [references/house-style.md](references/house-style.md) | Struktur, meta, pendahuluan, heading, paragraf, list, tabel, gambar, FAQ, Referensi, Catatan Editor, dan spesifikasi tampilan. **Sumber tunggal semua angka** | Selalu |
| [references/anti-slop.md](references/anti-slop.md) | Pola tulisan AI yang dilarang dan checklist-nya | Selalu, lalu jalankan checklist-nya sebelum menyerahkan |
| [references/google-genai-guidelines.md](references/google-genai-guidelines.md) | Pedoman resmi Google soal konten AI dan fitur AI Search, dipisah dari heuristik tim | Selalu |
| [references/ymyl-claim-gate.md](references/ymyl-claim-gate.md) | Gerbang klaim YMYL: status regulasi, sumber per klaim, rute pemberian, risiko, dan penanda outline | **Wajib** untuk Kategori 4 |
| [references/contoh-artikel.md](references/contoh-artikel.md) | Tiga contoh artikel (edukasi, YMYL, bisnis ringan) | Untuk kalibrasi nada dan ritme |

**Jika ada aturan yang bertentangan:**

- Angka dan bentuk artikel mengikuti `house-style.md`.
- Cara penyajian mengikuti `output-channels.md`.
- Klaim YMYL mengikuti `ymyl-claim-gate.md`, mengalahkan aturan gaya apa pun.
- Saat menulis ke Google Docs lewat connector, mekanisme teknis skill `google-workspace` (list asli, heading style, tabel, verifikasi) mengalahkan aturan format di skill ini.

---

## Alur Kerja

1. **Tentukan channel output** (output-channels.md bagian 1). Tanpa tool dokumen dan tanpa permintaan khusus, default-nya chat dengan Markdown siap salin.
2. **Pahami input dan kategori topik** (lihat di bawah). Untuk Kategori 4, baca ymyl-claim-gate.md.
3. **Kumpulkan dan cek sumber:**
   - Dengan outline: pakai sumber per poin dan hormati penandanya.
   - Tanpa outline: lakukan riset singkat sebelum menulis. Untuk YMYL, sumber P1–P2 wajib.
   - Tanpa akses web: tulis versi yang terkalibrasi dan tandai `[Verifikasi: …]`.
4. **Tulis naskah lengkap** mengikuti house-style.md dan anti-slop.md, dengan nada sesuai contoh-artikel.md.
5. **Sajikan ke channel** sesuai output-channels.md.
6. **Periksa** dengan checklist akhir di bawah. Untuk Google Docs dan .docx, baca ulang dokumen yang sudah jadi (output-channels.md bagian 8) lalu perbaiki temuannya.

---

## Kategori Topik

Sesuaikan riset, gaya bahasa, dan kedalaman dengan kategorinya. Jangan memaksakan sitasi akademis pada artikel ringan.

1. **Ringan dan gaya hidup** (hobi, wisata, kuliner, tips rumah, *outfit*, hiburan): santai, mengalir, dan praktis. Dasarnya logika umum dan tips teruji. **Tanpa** kutipan jurnal atau istilah klinis. Referensi boleh dihilangkan.
2. **Bisnis, karier, dan pemasaran:** profesional, lugas, dan taktis. Dasarnya praktik industri dan kerangka kerja nyata. Fokus pada langkah eksekusi, biaya, dan *return on investment*.
3. **Edukasi dan konseptual:** informatif dan terstruktur, dengan perumpamaan sederhana. Konsepnya akurat tanpa terasa seperti buku teks.
4. **YMYL** (kesehatan, obat, suplemen, tindakan klinik atau estetika, keuangan, hukum): tenang, jelas, empatik, dan **terkalibrasi**. Wajib lolos [ymyl-claim-gate.md](references/ymyl-claim-gate.md):
   - Status regulasi ditulis lebih dulu.
   - Satu klaim, satu sumber.
   - Rute pemberian harus cocok dengan buktinya.
   - Risiko serius disebut tanpa kalimat penenang.
   - Catatan Editor wajib ada.
   - Tanpa diagnosis individual, dosis tanpa resep, atau janji hasil.

---

## Menerjemahkan Outline atau Brief

- **Catatan penulis adalah instruksi, bukan teks artikel.** Ubah menjadi prosa jadi. Buang label "H2:/H3:" dan arahan penyajian dari naskah. Sitasi pendek `[situs](URL)` di outline diubah menjadi link inline pada nama sumbernya di dalam kalimat.
- **Struktur dan teks heading mengikuti outline.** Kembangkan setiap H2/H3/H4 sesuai arahan penyajiannya (paragraf, list, langkah bernomor, tabel, atau FAQ). Jika satu H3 hanya berisi 1–2 kalimat, gabungkan menjadi list di bawah H2.
- **Penanda outline wajib dihormati.** Aturan ini mengalahkan larangan "jangan menulis catatan mentah":
  - `[Verifikasi]`: cari sumbernya. Jika tidak ketemu, tulis versi terkalibrasi atau biarkan `[Verifikasi: …]`, lalu catat di Catatan Editor.
  - `[Review medis]`: tulis section-nya dengan kalibrasi ketat, lalu tambahkan "Bagian <H2> perlu ditinjau tenaga medis" di Catatan Editor.
  - `[Pengalaman]`: jangan dikarang. Tulis `[isi: pengalaman/kutipan praktisi tentang …]` dan catat di Catatan Editor.
- **Sumber:** Referensi hanya berisi sumber yang benar-benar dipakai. Sumber Prioritas 3 (blog klinik, penjual, *marketplace*) hanya dipakai sebagai klaim pihak tersebut, bukan dasar klaim keamanan atau efektivitas.
- **Dipindahkan:** jangan dibahas. Boleh disinggung satu kalimat plus Baca Juga.
- **Alternatif H1:** pilih satu sebagai dasar Title. Jika lebih dari 60 karakter, tambahkan baris `H1` di tabel meta.
- **Status pillar atau cluster** menentukan bentuk pendahuluan (house-style.md bagian 3).
- **Keyword:** sebarkan secara alami di Title, pendahuluan, subjudul yang relevan, dan badan teks, tanpa *keyword stuffing*.

---

## Aturan Inti yang Paling Sering Dilanggar

1. **Tanpa meta-writing.** Jangan menulis "Artikel ini membedah/membahas…", "Simak ulasan lengkapnya…", atau "Pada bagian ini…". Pendahuluan ditutup dengan pertanyaan atau keputusan utama pembaca.
2. **List adalah list asli.** Di Markdown pakai `- `. Di Docs/Word pakai format list dokumen. **Jangan mengetik `•`**, karena di Google Docs hasilnya menjadi bullet ganda `● •`. Pengecualiannya hanya channel teks polos.
3. **Tabel meta dan tabel isi adalah tabel asli**, bukan baris "Title - …".
4. **Tidak ada paragraf kosong** di dokumen jadi, karena jarak berasal dari pengaturan paragraf. Di sumber Markdown, blok **dipisah satu baris kosong**, karena satu Enter saja membuat paragraf menyatu.
5. **Paragraf pertama di bawah H2 langsung menjawab heading**, dan untuk YMYL jawabannya terkalibrasi. Gambar diletakkan setelah paragraf itu, tidak tepat di bawah heading.
6. **Tidak mengarang** angka, studi, kutipan, pengalaman, atau URL. Gunakan `[isi: …]` atau `[Verifikasi: …]` dan catat di Catatan Editor.
7. **Tanpa kontras biner** dalam bentuk apa pun ("tidak hanya… tetapi juga", "bukan sekadar", "banyak yang mengira… padahal"). "Berikut…" maksimal sekali per artikel.
8. **Meta: Title 45–60 karakter, Description 130–155 karakter.** Hitung dengan kode bila bisa.
9. **Nama sumber di dalam teks adalah link.** Jurnal, media, lembaga, regulator, atau dokter yang dikutip ditautkan ke halaman yang benar-benar dibuka. Kalimat atribusinya wajar ("Tinjauan sistematis di [Jurnal] (2025) menemukan…"), tanpa "satu tinjauan…" atau "alias", dan temuannya sama dengan isi sumber. URL tidak diketahui: `[isi: URL sumber X]`, bukan tebakan (house-style.md bagian 10).
10. **Panjang tanpa pengisi.** Default minimal 1.000 kata substansi. Untuk YMYL, jangan menambah butir tanpa sumber demi target kata.

---

## Bentuk Output

- **Chat:** artikelnya saja, dimulai dari `**Meta Information**` dan diakhiri Referensi atau Catatan Editor. Pakai Markdown standar, tanpa code block, dan tanpa kalimat pengantar atau penutup obrolan.
- **Google Docs** (connector atau API): dokumen dibuat dan diperiksa ulang. Balasan di chat cukup 1–2 kalimat beserta tautannya.
- **.docx:** file dibuat dengan style asli dan diperiksa ulang. Balasan di chat singkat saja.

---

## Checklist Akhir

**Konten**

- [ ] Intent pembaca terjawab, dan pendahuluan sesuai jenis keyword (definisi dijawab langsung, cluster dibuka hook).
- [ ] Setiap H2 dibuka dengan jawaban langsung.
- [ ] Checklist [anti-slop.md](references/anti-slop.md) bagian 7 lolos.
- [ ] Checklist [google-genai-guidelines.md](references/google-genai-guidelines.md) bagian 7 lolos.
- [ ] Untuk YMYL, [ymyl-claim-gate.md](references/ymyl-claim-gate.md) lolos dan Catatan Editor ada.
- [ ] Panjang Title dan Description sudah dihitung dan sesuai batas.
- [ ] Semua sumber di Referensi benar-benar dibuka dan dipakai.
- [ ] Setiap sumber yang disebut di badan artikel ditautkan, dan temuannya sudah dicocokkan dengan abstrak atau halaman aslinya.

**Format**

- [ ] Sesuai channel yang dipilih (output-channels.md).
- [ ] Untuk chat: blok dipisah baris kosong, list memakai `- `, tabel diapit baris kosong, tanpa code block.
- [ ] Untuk Google Docs atau .docx: pemeriksaan output-channels.md bagian 8 lolos (tabel asli, tanpa penanda list yang diketik, tanpa paragraf kosong, heading asli).
