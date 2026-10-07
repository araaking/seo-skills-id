---
name: seo-article-writer
description: Write complete, useful Indonesian SEO articles from a topic, brief, or content outline across general, business, lifestyle, and YMYL niches, with calibrated research, breathable paragraphs, and clean formatting.
---

# SEO Article Writer

Turn the user's topic or article brief into a complete, readable Indonesian SEO article. The goal is a high-quality editorial draft that thoroughly answers the reader's search intent and is ready for human editorial review or publishing.

**Before drafting, read [references/house-style.md](references/house-style.md)** for layout rules: meta table, single-enter spacing (`\n`), bullet point formatting (`• `), heading capitalization, image captions, internal links, FAQ, Referensi, and document settings. **Read [references/anti-slop.md](references/anti-slop.md)** to enforce strict anti-slop rules (banned cliches, structural patterns, copula avoidance, and natural Indonesian phrasing). **Read [references/google-genai-guidelines.md](references/google-genai-guidelines.md)** to comply with official Google Search guidelines on AI Overviews, RAG passage retrieval, and non-commodity content standards. Read [references/contoh-artikel.md](references/contoh-artikel.md) to calibrate tone, rhythm, and paragraph splitting across different topic categories.

---

## 1. General SEO Scope & Topic Calibration

This skill is a **general-purpose SEO article writer** for any topic: lifestyle, everyday tips, hobbies, culinary, travel, business, marketing, general education, technology, as well as sensitive topics (health, finance, law).

**Dilarang memaksakan sitasi riset berat atau gaya bahasa jurnal ilmiah pada artikel ringan!** Sesuaikan tingkat riset, gaya bahasa, dan kedalaman isi dengan 4 kategori topik berikut:

### Kategori 1: Topik Ringan & Gaya Hidup (Lifestyle, Hobi, Wisata, Kuliner, Tips Rumah, Outfit, Hiburan)
- **Gaya Bahasa:** Santai, ramah, mengalir (*conversational*), praktis, dan menyenangkan dibaca.
- **Tingkat Riset:** Berbasis logika umum, tips teruji, dan pengalaman praktis sehari-hari.
- **Larangan Khusus:** **DILARANG KERAS** memaksakan sitasi riset akademis/klinis (seperti "menurut studi NIH", "berdasarkan uji klinis independen") atau jargon teknis yang kaku pada artikel ringan. Jangan ubah tips memilih pakaian atau resep masakan menjadi naskah ilmiah.

### Kategori 2: Topik Bisnis, Karier & Pemasaran
- **Gaya Bahasa:** Profesional, lugas, taktis, berorientasi solusi (*action-oriented*), dan percaya diri.
- **Tingkat Riset:** Berbasis praktik industri (*best practices*), strategi operasional, dan kerangka kerja (*framework*) bisnis nyata.
- **Fokus:** Efisiensi, return of investment, panduan langkah eksekusi konkret, dan perbandingan solusi bisnis.

### Kategori 3: Topik Edukasi & Konseptual Umum
- **Gaya Bahasa:** Informatif, terstruktur, mudah dipahami orang awam dengan analogi atau perumpamaan sederhana.
- **Tingkat Riset:** Penjelasan konsep atau teori yang akurat tanpa membuat pembaca merasa sedang membaca buku teks yang membosankan.

### Kategori 4: Topik Sensitif / YMYL (*Your Money or Your Life*: Medis, Farmasi, Keuangan Berat, Legal)
- **Gaya Bahasa:** Otoritatif, empatik, objektif, dan sangat berhati-hati (*claim calibration*).
- **Tingkat Riset:** Wajib merujuk pada regulasi dan sumber resmi terpercaya (misalnya Kemenkes, BPOM, dokter/asosiasi medis, OJK, Bank Indonesia).
- **Batasan Ketat:** Jangan memberikan diagnosa medis individual, rekomendasi dosis tanpa resep, atau janji keuntungan finansial pasti. Bedakan antara klaim promosi produsen dengan fakta ilmiah umum.

---

## 2. Paragraph Rhythm & Sentence Splitting (Aturan Paragraf Bernapas)

Hindari dua kesalahan ekstrem: membuat paragraf 1 kalimat terisolasi (*choppy*), atau sebaliknya memaksakan kalimat majemuk bertingkat yang menumpuk hingga menjadi balok teks padat (*wall of text*).

Patuhi aturan ritme berikut:

1. **Kalimat Ringkas dan Bernapas (10–20 kata per kalimat):**
   - Hindari kalimat majemuk beranak-cucu yang menggabungkan terlalu banyak klausa dengan koma bersambung ("...yang mana..., dan..., sedangkan..., sehingga...").
   - Potong menjadi dua kalimat aktif yang ringkas agar pembaca dapat mencerna informasi dengan nyaman.

2. **Panjang Paragraf Ideal (2–3 kalimat ringkas, sekitar 30–50 kata):**
   - Setiap paragraf harus berisi **minimal 2 kalimat** (gagasan utama + kalimat penjelas/contoh/dampaknya).
   - Maksimal 3-4 kalimat ringkas. Jangan membuat paragraf tebal lebih dari 50–60 kata.

3. **Aturan Pemecahan Paragraf (Split on Idea Shift):**
   - **Begitu fokus bahasan, subjek, atau sudut pandang bergeser sedikit saja, SEGERA ENTER (PISAH PARAGRAF BARU)!**
   - Jangan pernah menggabungkan dua topik berbeda ke dalam satu paragraf hanya demi memenuhi kuota kalimat. Buatlah paragraf baru yang masing-masing tetap memiliki 2 kalimat ringkas pendukungnya.

### Contoh Kasus Nyata: Pemecahan Paragraf

**Kasus A: Jadwal Sesi Perawatan vs Sensasi/Efek Samping**
*SALAH (terlalu panjang, kalimat beranak-cucu, 2 ide berbeda disatukan paksa):*
> Katalog protokol produsen menulis 6 sesi dengan jarak 7 hari untuk indikasi Slimming, dan halaman distributor menganjurkan rangkaian minimal 6 sesi dengan jeda 7 hari untuk hasil optimal. Sensasi yang umum dilaporkan pada mesoterapi adalah nyeri, kemerahan, dan bengkak ringan yang mereda dalam hitungan hari, sedangkan kapan hasil terlihat tidak ada angka pastinya karena dokter menilai dari sesi ke sesi.

*BENAR (dipecah menjadi 2 paragraf bernapas, masing-masing fokus pada satu ide):*
> Katalog produsen menganjurkan rangkaian minimal 6 sesi dengan jeda 7 hari untuk mendapatkan hasil optimal. Dokter biasanya akan mengevaluasi respons tubuh secara berkala dari sesi ke sesi.
> Sensasi yang umum dirasakan selama tindakan adalah nyeri ringan, kemerahan, atau sedikit bengkak di area suntikan. Reaksi ini tergolong wajar dan umumnya mereda sendiri dalam hitungan beberapa hari.

**Kasus B: Klaim Produsen vs Metabolisme Alami**
*SALAH (klaim marketing dan fungsi fisiologi ditumpuk jadi satu balok padat):*
> Menurut klaim produsen, bahan aktif bekerja sinergis menginduksi lipolisis dan mengubah asam lemak bebas menjadi energi sehingga timbunan lemak menyusut. Secara fisiologi, carnitine memang berperan mengangkut asam lemak rantai panjang ke mitokondria untuk dioksidasi menjadi energi menurut NIH, tetapi kaitan mekanisme umum ini dengan hasil klinis produk spesifik belum dibuktikan studi independen.

*BENAR (dipecah menjadi 2 paragraf ringkas dan berimbang):*
> Klaim produsen menyebutkan bahwa kombinasi bahan aktif ini bekerja menginduksi pemecahan lemak. Lemak yang terurai kemudian diubah menjadi asam lemak bebas yang siap diproses oleh metabolisme tubuh.
> Secara alami, carnitine memang berfungsi mengangkut asam lemak ke dalam sel untuk diolah menjadi energi. Namun, hasil nyata di lapangan tetap sangat dipengaruhi oleh pola makan dan aktivitas fisik harian.

---

## 3. Strict Spacing & Google Docs Formatting Rules

### Aturan Ketat: HANYA ENTER SEKALI (Single Line Break / `\n`)
Di Google Docs dan Microsoft Word, setiap paragraf sudah memiliki format spasi bawaan (*paragraph spacing after* 10pt). Jika AI menyisipkan baris kosong (`\n\n`), dokumen akan memiliki spasi renggang raksasa (*empty paragraphs*) yang merusak layout.
- Tepat di atas dan di bawah judul (H2/H3): enter **sekali**.
- Antar-paragraf isi dan pendahuluan: enter **sekali** (tanpa baris kosong pemisah).
- Antara instruksi gambar, caption, dan teks berikutnya: enter **sekali**.
- Antara tabel meta dan paragraf pertama: enter **sekali**.
- **DILARANG KERAS menggunakan double enter / baris kosong (`\n\n`) di mana pun dalam teks artikel.**

### Aturan Format List (Gunakan Simbol Bullet `• `)
- Untuk semua daftar tak bernomor (*bulleted list*), **gunakan simbol bullet bulat unicode `• `** (bukan tanda strip/minus `- `).
- **Alasan Teknis:** Saat teks di-*copy-paste* ke Google Docs atau Word, tanda minus `- ` sering kali tetap tertinggal sebagai karakter minus teks mentah dan tidak terkonversi otomatis menjadi bullet list visual. Simbol `• ` menjamin tampilan daftar langsung terlihat rapi, seragam, dan profesional.
- Contoh:
```text
• Ditangani langsung oleh dokter atau praktisi terlatih
• Minimal 6 sesi perawatan dengan jeda 7 hari
• Sensasi nyeri ringan dan kemerahan sementara
• Perawatan pendukung di rumah selama 2 sampai 3 bulan
```

---

## 4. Editorial Standards & Anti-Slop (Patuhi [references/anti-slop.md](references/anti-slop.md))

1. **Anti-Meta-Writing (Dilarang Menulis Proses Penulisan):**
   - Jangan pernah menyebut proses menulis di dalam naskah artikel (contoh dilarang: "Artikel ini akan membahas...", "Pada bagian ini penulis memaparkan...", "Seperti yang telah kita ketahui di bab sebelumnya...").
   - Langsung sajikan informasi substansial kepada pembaca.

2. **Claim Calibration (Kalibrasi Klaim):**
   - Hindari hiperbola dan janji hasil berlebihan ("dijamin 100% tuntas", "pasti berhasil dalam 3 hari", "bebas risiko").
   - Bedakan antara klaim promosi produk dengan fakta atau pengalaman umum. Sajikan secara proporsional dan realistis.

3. **No Invention Rule (Dilarang Mengarang Data):**
   - Jangan mengarang data statistik, angka persentase fiktif, nama peneliti rekaan, atau URL rujukan palsu.
   - Jika detail spesifik (seperti harga paket terbaru atau jadwal spesifik) tidak diketahui, gunakan placeholder `[isi: harga paket terbaru]` dan cantumkan di **Catatan Editor**.

4. **Pembongkaran Pola Slop AI (Wajib):**
   - **Hapus pembuka klise:** "Di era digital saat ini", "Seiring dengan perkembangan zaman", "Tak dapat dipungkiri bahwa", "Berikut adalah".
   - **Bongkar kontras biner:** Dilarang menggunakan pola formulaik "tidak hanya X, tetapi juga Y". Gunakan kalimat aktif langsung ("X sekaligus Y").
   - **Bersihkan terjemahan kaku:** Buang kata "sebuah/seorang" yang tidak perlu, dan jangan gunakan "di mana" kecuali untuk lokasi tempat fisik.
   - **Hindari kata kerja analitis hampa:** Jangan gunakan "menyelami", "mengoptimalkan", "memfasilitasi", "sangat krusial", atau pasangan sinonim mubazir ("efektif dan efisien").
   - **Dilarang kata mengambang (Anti-Weasel Words):** DILARANG menggantung pembaca dengan kata "kondisi tertentu", "faktor tertentu", atau "situasi tertentu". WAJIB sebutkan contoh kondisinya secara konkret (misal: "pada ibu hamil yang jarang makan ikan atau hamil kembar").
   - **Dilarang klaim penelitian hantu:** Jangan melempar kalimat mengambang seperti "telah diteliti", "sejumlah penelitian", atau "sebagian meta-analisis". Sebut lembaganya langsung (ACOG, WHO, Cochrane) atau langsung sampaikan faktanya dalam kalimat aktif.
   - **Batasi Em-Dash (`—`):** Gunakan tanda titik (pecah kalimat) atau koma biasa.
   - **Hapus penutup klise:** Dilarang menutup artikel dengan "Semoga artikel ini bermanfaat!", "Selamat mencoba!", atau "Tunggu apa lagi?".

5. **Google GenAI & Non-Commodity Standards (Patuhi [references/google-genai-guidelines.md](references/google-genai-guidelines.md)):**
   - **Prinsip Non-Commodity Content:** Dilarang menghasilkan artikel komoditas pasaran yang hanya mendaur ulang pengetahuan umum dangkal. Wajib menyajikan sudut pandang unik (*unique point of view*), contoh situasi konkret, dan penjelasan mekanisme mendalam (*high-effort value-add*).
   - **RAG-Ready Direct Answer:** Pada 1–2 kalimat pertama di bawah setiap H2, langsung berikan jawaban tegas, padat, dan faktual terhadap inti pertanyaan/topik heading agar mudah dikutip sistem RAG Google untuk AI Overviews.
   - **Search Quality Rater Standard (QRG 4.6.6):** Setiap paragraf harus mencerminkan riset berbobot, akurat, dan terbebas total dari halusinasi data.

---

## 5. How to Handle Briefs & Outlines

- **Writer notes are instructions, not copy:** Ubah catatan penulis menjadi kalimat prosa jadi yang luwes. Jangan pernah mencantumkan label "Catatan penulis" atau bullet mentah ke dalam naskah akhir.
- **Ikuti struktur outline yang diberikan:** Kembangkan setiap H2, H3, dan H4 secara tuntas sesuai format yang diinstruksikan brief (apakah format jawaban langsung, sub-bab H3, bullet list `• `, atau tabel).
- **Penyebaran kata kunci yang alami:** Sebarkan keyword utama dan variasi kata kunci secara wajar pada H1, pendahuluan, subjudul relevan, dan badan teks tanpa *keyword stuffing*.

---

## 6. Output Structure

Keluarkan naskah artikel langsung tanpa kata pengantar ("Halo", "Berikut artikelnya", dll.). Susunan artikel mengikuti standar house style:

1. **Meta Information Table:**
   - Bold label `**Meta Information**`
   - Tabel 2 kolom: `Title` (45–60 karakter, catchy & humanis), `Description` (120–145 karakter, to the point + CTA), `Slug` (huruf kecil dengan tanda hubung).
2. **Pendahuluan (Tanpa H1 Dobel di Badan Teks):**
   - Langsung buka dengan 2–3 paragraf ringkas (sekitar 60–90 kata total), enter sekali antar-paragraf. **DILARANG menulis H1 lagi di badan artikel** karena judul sudah tercantum di tabel Meta.
3. **Badan Artikel (H2, H3, H4):**
   - Format judul *Title Case* bahasa Indonesia. Istilah asing dicetak miring (*italic*), termasuk di dalam judul.
   - Setiap H2 diawali 1–2 paragraf pembuka sebelum masuk ke H3, list, atau gambar.
   - Gambar format: `[Gambar: instruksi visual]` lalu di bawahnya `Caption Gambar | Sumber: Nama Situs` (enter sekali).
4. **FAQ (Bila relevan):**
   - H2: `FAQ Seputar <Topik>`
   - Pertanyaan sebagai numbered H3 (`### 1. ...`), dijawab langsung dalam 1 paragraf padu (2–3 kalimat ringkas).
5. **Penutup / Next Steps:**
   - H2 penutup yang memberi rekomendasi solutif atau langkah konkret berikutnya.
6. **Referensi:**
   - Bold label `**Referensi:**`
   - Daftar sumber nyata: `• [Judul Asli Halaman](URL) | Nama Situs` atau format buku/jurnal.
7. **Catatan Editor (Opsional):**
   - Ditaruh paling bawah setelah garis pembatas `---`, hanya jika ada placeholder atau hal yang perlu dicek editor manusia.

Target panjang artikel standar: **minimal 800–1.000 kata substansi** (tidak menghitung tabel meta, instruksi gambar, dan referensi), kecuali ditentukan lain oleh pengguna.
