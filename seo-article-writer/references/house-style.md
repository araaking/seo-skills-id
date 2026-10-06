# House Style: Format Artikel

Dokumen ini adalah format standar untuk seluruh artikel yang diproduksi menggunakan skill `article-draft-writer`. Berlaku untuk segala macam topik: gaya hidup, hobi, bisnis, teknologi, panduan praktis, edukasi umum, hingga topik sensitif (YMYL). Terapkan format ini kecuali pengguna meminta format khusus lainnya.

Lihat `contoh-artikel.md` untuk melihat implementasi nyata format ini pada berbagai kategori topik.

---

## 1. Document Order (Susunan Dokumen)

1. Tabel **Meta Information**
2. Pendahuluan (tanpa H1 di badan teks; Title meta berfungsi sebagai judul utama halaman)
3. Bagian H2 (dapat disertai sub-bab bernomor H3 bila diperlukan)
4. Bagian FAQ (jika ada pertanyaan lanjutan yang sering dicari pengguna)
5. Bagian Penutup / Rekomendasi Solutif
6. **Referensi**
7. **Catatan Editor** (hanya jika ada placeholder atau hal yang perlu diverifikasi editor manusia; tidak untuk dipublikasikan)

---

## 2. Meta Information

Awali output artikel dengan label bold dan tabel 2 kolom:

```markdown
**Meta Information**

| Element | Content |
|---|---|
| Title | Penelitian Korelasional: Pengertian, Jenis, Langkah & Contohnya |
| Description | Penelitian korelasional mengukur hubungan antarvariabel tanpa memanipulasinya. Pelajari jenis, langkah, dan contoh penerapannya di sini. |
| Slug | penelitian-korelasional |
```

- **Title:** sekitar 60–75 karakter. Tempatkan kata kunci utama di depan atau di posisi menonjol, diikuti subtopik utama.
- **Description:** sekitar 140–160 karakter. Mengandung kata kunci utama, menjelaskan manfaat artikel bagi pembaca secara mengalir (bukan sekadar daftar kata kunci).
- **Slug:** huruf kecil, dipisahkan tanda hubung (-), ringkas.

---

## 3. Pendahuluan

Panjang pendahuluan sekitar 2–3 paragraf ringkas (total 60–90 kata):
- Buka langsung dengan situasi nyata, keresahan, atau pertanyaan konkret yang dihadapi pembaca.
- Hindari basa-basi klise seperti "Di era modern saat ini", "Seiring perkembangan zaman", atau "Pernahkah Anda membayangkan...".
- Sebutkan topik utama dan jelaskan mengapa hal tersebut penting dipahami.
- Tutup pendahuluan dengan satu kalimat pengantar yang mengarahkan pembaca ke ulasan lengkap di bawahnya.
- **Tanpa gambar di bagian pendahuluan.**

---

## 4. Struktur Heading (H2 dan H3)

- **H2** untuk topik bahasan utama, **H3** untuk sub-item atau rincian turunan. Hindari H4 kecuali mutlak diperlukan.
- Tulis judul dalam *Title Case* bahasa Indonesia: kapitalisasi huruf pertama setiap kata utama; kata tugas/hubung tetap huruf kecil kecuali di awal kalimat (di, ke, dari, dan, atau, yang, untuk, pada, dengan, secara, agar, sebagai).
- Jika sebuah H2 berisi serangkaian item paralel (jenis, penyebab, langkah, tips, pertanyaan FAQ), beri nomor pada H3: `### 1. Desain Eksplanatori`.
- Istilah asing tetap dicetak miring (*italic*) di dalam judul: `## Cara Membaca *Scatter Plot*`.

---

## 5. Paragraf Bernapas & Aturan Spasi (Paragraph Rhythm)

Hindari membuat paragraf satu kalimat terisolasi (*choppy*), dan dilarang keras menumpuk banyak kalimat majemuk menjadi balok teks padat (*wall of text*).

### Aturan Panjang Kalimat dan Paragraf
- **Kalimat ringkas dan bernapas (10–20 kata per kalimat):** Gunakan kalimat aktif yang to the point. Hindari menumpuk anak kalimat dengan banyak koma ("...yang mana..., dan..., sedangkan..., sehingga...").
- **Panjang paragraf ideal (2–3 kalimat ringkas, sekitar 30–50 kata):**
  - Setiap paragraf harus berisi **minimal 2 kalimat** (gagasan pokok + kalimat penjelas, mekanisme, atau dampaknya).
  - Paragraf maksimal 3–4 kalimat ringkas.
- **Aturan Pemecahan Paragraf (Split on Idea Shift):**
  - **Begitu fokus pembicaraan atau subtopik bergeser sedikit saja, SEGERA ENTER (PISAH PARAGRAF BARU)!**
  - Jangan memaksakan dua ide berbeda masuk ke satu paragraf hanya demi memenuhi syarat minimal kalimat.

#### Contoh Kasus Nyata Pemecahan Paragraf:

**Kasus A: Sesi Protokol vs Sensasi Tindakan**
*SALAH (terlalu padat, kalimat beranak-cucu, 2 ide berbeda disatukan):*
```text
Katalog protokol produsen menulis 6 sesi dengan jarak 7 hari untuk indikasi Slimming, dan halaman distributor menganjurkan rangkaian minimal 6 sesi dengan jeda 7 hari untuk hasil optimal. Sensasi yang umum dilaporkan pada mesoterapi adalah nyeri, kemerahan, dan bengkak ringan yang mereda dalam hitungan hari, sedangkan kapan hasil terlihat tidak ada angka pastinya karena dokter menilai dari sesi ke sesi.
```
*BENAR (dipecah menjadi 2 paragraf bernapas, masing-masing 2 kalimat ringkas):*
```text
Katalog produsen menganjurkan rangkaian minimal 6 sesi dengan jeda 7 hari untuk mendapatkan hasil optimal. Dokter biasanya akan mengevaluasi respons tubuh secara berkala dari sesi ke sesi.
Sensasi yang umum dilaporkan selama tindakan adalah nyeri ringan, kemerahan, atau sedikit bengkak di area suntikan. Reaksi ini tergolong wajar dan umumnya mereda sendiri dalam hitungan beberapa hari.
```

**Kasus B: Klaim Produsen vs Metabolisme Alami**
*SALAH (klaim pabrik dan ulasan fisiologi bertumpuk menjadi satu balok teks tebal):*
```text
Menurut klaim produsen, bahan aktif bekerja sinergis menginduksi lipolisis dan mengubah asam lemak bebas menjadi energi sehingga timbunan lemak menyusut. Secara fisiologi, carnitine memang berperan mengangkut asam lemak rantai panjang ke mitokondria untuk dioksidasi menjadi energi menurut NIH, tetapi kaitan mekanisme umum ini dengan hasil klinis produk spesifik belum dibuktikan studi independen.
```
*BENAR (dipecah menjadi 2 paragraf yang berimbang):*
```text
Klaim produsen menyebutkan bahwa kombinasi bahan aktif ini bekerja menginduksi pemecahan lemak. Lemak yang terurai kemudian diubah menjadi asam lemak bebas yang siap diproses oleh metabolisme tubuh.
Secara alami, carnitine memang berfungsi mengangkut asam lemak ke dalam sel untuk diolah menjadi energi. Namun, efektivitas formula injeksi ini tetap dipengaruhi oleh pola makan dan gaya hidup harian.
```

### Aturan Ketat: HANYA ENTER SEKALI (Single Line Break / `\n`)
- **Di seluruh dokumen artikel, HANYA gunakan enter sekali (`\n`).**
- Tepat di atas dan di bawah judul (H2/H3): enter **sekali**.
- Antar-paragraf isi maupun pendahuluan: enter **sekali** (tanpa baris kosong).
- Antara teks, instruksi gambar, dan caption: enter **sekali**.
- Antara tabel meta dan paragraf pendahuluan: enter **sekali**.
- **DILARANG KERAS menggunakan double enter / baris kosong (`\n\n`) di mana pun.**
- *Alasan teknis:* Di Google Docs dan Microsoft Word, setiap pergantian paragraf otomatis diberi spasi bawah (*spacing after* 10pt). Jika AI menyisipkan baris kosong (`\n\n`), Docs/Word akan merendernya sebagai paragraf kosong terpisah yang menghasilkan jarak spasi renggang raksasa.

---

## 6. Format Daftar (List) & Kompatibilitas Google Docs

Untuk daftar poin tak bernomor (*bulleted list*), **wajib menggunakan simbol bullet bulat unicode `• `**, BUKAN tanda strip/minus `- `.

*Alasan Teknis:*
Saat teks disalin (*copy-paste*) ke Google Docs atau Word, tanda minus `- ` sering kali tetap tertinggal sebagai teks mentah berupa tanda strip dan tidak otomatis menjadi bullet point visual. Dengan menuliskan simbol `• `, naskah langsung tampil rapi sebagai bullet points di aplikasi mana pun.

Format penulisan list:
- Awali list dengan satu kalimat pengantar pendek berakhiran tanda titik dua (`:`).
- Tiap butir list diawali dengan `• ` diikuti satu spasi.
- Poin list ditulis ringkas (sekitar 3–10 kata), diawali huruf kapital, dan tanpa titik di akhir jika bukan kalimat lengkap.

Contoh penulisan yang **BENAR**:
```text
Berikut beberapa kriteria umum yang perlu diperhatikan:
• Ditangani langsung oleh dokter atau praktisi bersertifikat
• Minimal 6 sesi perawatan dengan jeda 7 hari
• Sensasi nyeri ringan dan kemerahan sementara di area tindakan
• Perawatan pendukung di rumah selama 2 sampai 3 bulan
```

Contoh penulisan yang **SALAH** (menggunakan tanda minus):
```text
- Ditangani dokter atau praktisi terlatih
- Minimal 6 sesi dengan jeda 7 hari
- Sensasi nyeri ringan dan kemerahan
```

---

## 7. Tipografi dan Gaya Bahasa

- **Cetak miring (*italic*) istilah asing:** Miringkan kata asing non-baku setiap kali muncul, termasuk di dalam judul (*scatter plot*, *sampling*, *skincare*, *outfit*, *marketplace*).
- Jangan miringkan nama orang, nama merek/brand dagang, singkatan umum (SPSS, SEO, BPOM, SPF), atau kata serapan baku (variabel, korelasi, data, dokter).
- Gunakan sudut pandang "kamu" dan "-mu" secara ramah dan konsisten untuk artikel populer, atau gaya netral-profesional untuk artikel ilmiah/bisnis.
- **Anti-Meta-Writing:** Jangan pernah menulis kalimat proses penulisan seperti "Dalam artikel ini akan dijelaskan..." atau "Pada sub-bab ini kita akan melihat...". Tulis langsung substansinya.

---

## 8. Gambar dan Caption

- Cantumkan saran gambar pada bagian yang relevan (diagram alur, grafik perbandingan, contoh visual). Biasanya 3–5 gambar untuk artikel 1.000–1.500 kata.
- Format penulisan: tepat di bawah judul H2/H3, enter sekali:
```markdown
[Gambar: ilustrasi diagram alur langkah penelitian dari perumusan masalah hingga analisis data]
Alur Langkah Penelitian Korelasional | Sumber: SAGE Publications
```
- Baris pertama: `[Gambar: deskripsi visual instruksi untuk tim grafis]`.
- Baris kedua: `Deskripsi Singkat Gambar | Sumber: Nama Situs`.
- Jika gambar dibuat sendiri oleh tim internal, hilangkan bagian sumber: `Alur Langkah Penelitian Korelasional`.

---

## 9. Internal Links & Baca Juga

- **Inline links:** Tautkan istilah penting pertama kali ke artikel terkait jika ada URL yang valid.
- **Baca Juga:** Sisipkan 1–2 kali di akhir section H2 sebelum H2 berikutnya:
```markdown
**Baca Juga:** [Judul Asli Artikel Terkait](https://contoh.com/artikel)
```
- Gunakan placeholder `**Baca Juga:** [isi: artikel tentang topik X]` jika URL belum tersedia, dan catat di **Catatan Editor**.

---

## 10. FAQ (Frequently Asked Questions)

- H2: `FAQ Seputar <Topik>`
- Pertanyaan sebagai numbered H3 (`### 1. Apakah Tindakan Ini Menimbulkan Efek Samping?`).
- Jawaban berupa satu paragraf padu (2–3 kalimat ringkas, sekitar 30–50 kata), langsung menjawab inti pertanyaan di kalimat pertama.

---

## 11. Bagian Penutup (Next Steps)

- H2 penutup bukan sekadar rangkuman ulang ("Kesimpulan"), melainkan memberikan langkah nyata bagi pembaca:
  - Topik kesehatan/medis: `Kapan Harus ke Dokter?`
  - Topik bisnis/tools: `Langkah Awal Memulai di Bisnismu`
  - Topik konsep/metodologi: `Kapan Metode Ini Paling Tepat Digunakan?`

---

## 12. Referensi

Tutup naskah dengan label bold `**Referensi:**` dan daftar sumber dengan simbol bullet `• `:

```markdown
**Referensi:**

• [Judul Asli Halaman](https://contoh.com/halaman) | Nama Situs
• Nama Penulis, Inisial. (Tahun). *Judul Buku/Jurnal*. Nama Penerbit.
```

- Masukkan hanya rujukan yang benar-benar digunakan. Jangan membuat referensi palsu atau dekoratif.

---

## 13. Penyesuaian Nada & Gaya Penulisan (Topic Calibration)

Jangan samakan semua artikel! Sesuaikan dengan 4 tingkatan topik:

1. **Topik Ringan & Gaya Hidup (Lifestyle, Hobi, Wisata, Tips Rumah, Outfit):**
   - Nada santai, ramah, mengalir, praktis.
   - **TIDAK PERLU** riset akademis/jurnal berat, kutipan NIH, atau istilah klinis kaku.
2. **Topik Bisnis, Karier & Pemasaran:**
   - Nada profesional, lugas, berbasis praktik industri nyata dan framework teruji.
3. **Topik Edukasi & Konseptual Umum:**
   - Nada informatif, terstruktur, memakai perumpamaan sederhana.
4. **Topik Sensitif / YMYL (Kesehatan Medis, Keuangan Berat, Legal):**
   - Nada otoritatif, berhati-hati, verifikasi sumber resmi (Kemenkes, BPOM, OJK), tanpa diagnosa atau klaim muluk.

---

## 14. Word Document (.docx) Settings

| Elemen | Pengaturan |
|---|---|
| Font Badan Teks | Arial, 11 pt |
| Line Spacing | 1.15 (Multiple) |
| Paragraph Spacing | 10 pt after (tanpa baris kosong tambahan) |
| Alignment | Justified (Rata Kiri-Kanan) |
| H2 | Heading 2 style, Arial 16 pt, Bold |
| H3 | Heading 3 style, Arial 14 pt, Bold |
| Gambar | Centered (Rata Tengah) |
| Caption | Centered, 11 pt reguler, tepat di bawah gambar |
| Bullet List | Simbol bullet `• `, hanging indent 0.25" |
| Referensi | Simbol bullet `• `, font 10–11 pt |
| Meta Table | 2 kolom di bagian paling atas |
