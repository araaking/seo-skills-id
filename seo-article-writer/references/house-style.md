# House Style: Format Artikel

Format standar untuk semua artikel yang ditulis dengan skill `seo-article-writer`. File ini menjadi **satu-satunya sumber** untuk angka, urutan, dan aturan bentuk artikel. Jika SKILL.md atau file lain menyebut angka berbeda, ikuti file ini.

Aturan di sini tidak bergantung pada channel. Cara menyajikannya di chat, Google Docs, .docx, atau teks polos diatur di [output-channels.md](output-channels.md). Semua contoh di file ini ditulis dalam Markdown (channel A).

Lihat [contoh-artikel.md](contoh-artikel.md) untuk penerapan utuh pada tiga jenis topik.

---

## 1. Urutan Dokumen

1. **Meta Information** (label tebal + tabel)
2. Pendahuluan (tanpa H1 di badan artikel)
3. Bagian H2, dengan H3 bila perlu
4. Bagian FAQ (bila ada pertanyaan nyata yang relevan)
5. Bagian penutup berisi langkah lanjut
6. **Referensi** (wajib untuk YMYL dan artikel edukasi berbasis sumber, opsional untuk topik ringan)
7. **Catatan Editor** (wajib untuk YMYL atau bila ada penanda/placeholder yang tersisa; lihat bagian 14)

---

## 2. Meta Information

Label tebal `Meta Information`, lalu tabel asli 2 kolom:

```markdown
**Meta Information**

| Element | Content |
|---|---|
| Title | Penelitian Korelasional: Pengertian, Jenis, dan Contohnya |
| Description | Penelitian korelasional mengukur hubungan antarvariabel tanpa memanipulasinya. Pahami jenis desainnya, cara membaca nilai r, dan contohnya. |
| Slug | penelitian-korelasional |

Paragraf pendahuluan pertama dimulai di sini.
```

- **Title: 45–60 karakter.** Keyword utama di depan atau di posisi menonjol, diikuti subtopik utama. Title sekaligus menjadi judul artikel (H1 di CMS) dan nama file dokumen.
- **Description: 130–155 karakter.** Memuat keyword utama dan manfaat bagi pembaca dalam kalimat yang mengalir, ditutup ajakan halus. Hindari "Simak…" dan "…di sini" yang klise.
- **Slug:** huruf kecil, dipisah tanda hubung, ringkas, mengikuti keyword utama.
- Batas karakter ini sama dengan skill `seo-meta-generator`. Hitung panjangnya dengan kode bila bisa (misalnya `len()` di Python), jangan ditaksir.
- Jika outline memberi judul H1 yang lebih panjang dari 60 karakter, tambahkan baris `H1` di bawah Title berisi judul lengkapnya.
- Isi sel meta berupa teks polos: tanpa italic dan tanpa simbol Markdown.
- Tabel ini wajib tabel asli. Jangan menulisnya sebagai baris "Title - …".

---

## 3. Pendahuluan

Panjangnya 2–3 paragraf, sekitar 70–100 kata total. Tidak ada gambar di pendahuluan.

- **Keyword definisi** ("X adalah", "apa itu X", slug `x-adalah`) atau artikel **pillar/mandiri**: jawab langsung di 1–2 kalimat pertama. Contoh: "Infus whitening adalah pemberian vitamin C, glutathione, dan zat lain lewat infus dengan tujuan mencerahkan kulit." Hook boleh menyusul di kalimat berikutnya.
- **Artikel cluster** (definisinya sudah dibahas di artikel lain): buka langsung dengan hook berupa situasi nyata, keresahan, atau pertanyaan konkret pembaca.
- Sebut topik utama dan alasan pembaca perlu memahaminya.
- **Tutup pendahuluan dengan satu kalimat yang menyebut pertanyaan atau keputusan utama pembaca**, bukan pengumuman isi artikel. Contoh: "Sebelum memutuskan, ada tiga hal yang perlu dicek: status izin produknya, bukti manfaatnya, dan risikonya."
- **Dilarang** memakai "Artikel ini membahas/membedah/mengulas…", "Simak ulasan lengkapnya…", "Yuk, cari tahu…", "berikut", atau mengulang daftar H2.
- Hindari pembuka klise seperti "Di era modern saat ini" dan "Pernahkah kamu membayangkan…".

---

## 4. Heading

- **Struktur dan teks heading mengikuti outline** bila ada. House style hanya mengatur kapitalisasi, italic, dan penomoran.
- **H2** untuk topik utama dan **H3** untuk rincian turunan. H4 hanya dipakai bila outline memakainya. Jangan loncat level.
- **Tidak ada H1 di badan artikel.** Judul tinggal di Title atau baris H1 tabel meta.
- **H2 sebagian besar berupa pernyataan informatif**, misalnya "Penyebab *Chicken Skin* dan Pemicunya". Maksimal satu H2 berbentuk pertanyaan di luar FAQ, biasanya H2 definisi ("Apa Itu…?").
- **Penomoran H3** (`### 1. Desain Eksplanatori`) hanya untuk item paralel yang jumlahnya disebut di judul atau heading ("4 Cara…", "Dua Jenis…"), atau untuk langkah yang urutannya penting. Nomor ini bagian dari teks heading, bukan penomoran otomatis dokumen. H3 pertanyaan di FAQ tidak diberi nomor.
- **Title Case bahasa Indonesia:** huruf pertama setiap kata utama kapital. Kata tugas tetap kecil kecuali di awal: di, ke, dari, dan, atau, yang, untuk, pada, dengan, secara, agar, sebagai. Kata ulang dikapitalkan dua-duanya ("Ciri-Ciri").
- Istilah asing tetap miring di dalam heading: `## Cara Membaca *Scatter Plot*`.

---

## 5. Paragraf dan Ritme

Tujuannya teks yang enak dibaca: bukan balok teks padat, tapi juga bukan deretan paragraf satu kalimat. Angka di bawah adalah **patokan, bukan kuota**. Ritme yang terlalu seragam (setiap paragraf dua kalimat, setiap H3 satu paragraf) justru menjadi ciri tulisan AI.

- **Kalimat:** sebagian besar nyaman di 10–20 kata. Variasikan: jawaban pendek ("Tidak." atau "Hasilnya sementara.") dan sesekali kalimat 25 kata yang mengalir membuat teks terdengar manusiawi. Kalimat majemuk bertingkat dengan banyak koma ("…yang mana…, dan…, sedangkan…, sehingga…") dipecah menjadi dua kalimat.
- **Paragraf:** umumnya 2–4 kalimat (sekitar 30–60 kata). Paragraf satu kalimat boleh untuk jawaban langsung atau penekanan. Yang dihindari adalah beberapa paragraf satu kalimat berturut-turut.
- **Pisah paragraf saat ide bergeser.** Begitu subjek atau sudut pandang berganti, mulai paragraf baru. Jangan menyatukan dua ide demi memenuhi jumlah kalimat.
- **Gabungkan bila terlalu tipis.** Jika beberapa H3 masing-masing hanya berisi 1–2 kalimat, sajikan sebagai list atau tabel di bawah H2.

### Contoh Pemecahan Paragraf

**Kasus A: Jadwal sesi vs sensasi tindakan**

SALAH (dua ide disatukan, kalimat beranak-cucu):

> Katalog protokol produsen menulis 6 sesi dengan jarak 7 hari untuk indikasi Slimming, dan halaman distributor menganjurkan rangkaian minimal 6 sesi dengan jeda 7 hari untuk hasil optimal. Sensasi yang umum dilaporkan pada mesoterapi adalah nyeri, kemerahan, dan bengkak ringan yang mereda dalam hitungan hari, sedangkan kapan hasil terlihat tidak ada angka pastinya karena dokter menilai dari sesi ke sesi.

BENAR (dua paragraf, atribusi dan kalibrasinya tetap ada):

> Katalog produsen menganjurkan rangkaian minimal 6 sesi dengan jeda 7 hari. Dokter menilai respons kulit dari sesi ke sesi, jadi belum ada angka pasti kapan hasilnya mulai terlihat.
>
> Sensasi yang umum dilaporkan selama tindakan adalah nyeri ringan, kemerahan, atau bengkak di area suntikan. Menurut katalog yang sama, keluhan ini biasanya mereda dalam beberapa hari.

**Kasus B: Klaim produsen vs fungsi zat di tubuh**

SALAH (klaim produsen dan fisiologi ditumpuk menjadi satu balok):

> Menurut klaim produsen, bahan aktif bekerja sinergis menginduksi lipolisis dan mengubah asam lemak bebas menjadi energi sehingga timbunan lemak menyusut. Secara fisiologi, carnitine memang berperan mengangkut asam lemak rantai panjang ke mitokondria untuk dioksidasi menjadi energi menurut NIH, tetapi kaitan mekanisme umum ini dengan hasil klinis produk spesifik belum dibuktikan studi independen.

BENAR (dua paragraf, klaim produsen tetap diatribusikan dan status buktinya tetap disebut):

> Produsen mengklaim kombinasi bahan aktifnya memecah timbunan lemak menjadi asam lemak bebas yang kemudian dibakar menjadi energi. Klaim ini berasal dari materi promosi produsen.
>
> Menurut [NIH](https://contoh.com/halaman-nih-carnitine), carnitine memang mengangkut asam lemak rantai panjang ke mitokondria untuk diolah menjadi energi. Namun, kaitan fungsi umum ini dengan hasil suntikan produk tersebut belum dibuktikan uji klinis independen.

---

## 6. List

- **List adalah list asli.** Di Markdown pakai `- ` (atau `1. ` untuk langkah berurutan). Di Docs/Word gunakan format list dokumen. **Jangan mengetik `•`** kecuali di channel teks polos (lihat output-channels.md).
- **Kalimat pengantar list** sebaiknya menjadi kalimat terakhir paragraf sebelumnya dan diakhiri titik dua, bukan paragraf satu kalimat tersendiri.
- **"Berikut" maksimal sekali per artikel.** "Berikut adalah…" dan "Berikut ini merupakan…" selalu dilarang. Variasikan, misalnya "Tampilannya cenderung memburuk ketika:" atau "Halaman produk yang meyakinkan biasanya memuat empat jenis visual:".
- **Dua bentuk butir yang sah:**
  1. **Butir ringkas** (3–10 kata), diawali huruf kapital, tanpa titik di akhir.
  2. **Label tebal + penjelasan** 1–2 kalimat, diakhiri titik, dipakai bila tiap butir perlu alasan atau sumber. Contoh: `- **Paparan sinar UV:** memicu melanosit membentuk melanin lagi.`
- Jangan mencampur dua bentuk dalam satu list. Sebuah list minimal berisi 2 butir.
- Jumlah butir mengikuti fakta, bukan ritme tiga serangkai.

Contoh benar:

```markdown
Tampilannya cenderung memburuk ketika:

- Udara dingin dan kering
- Kulit jarang diberi pelembap setelah mandi
- Mandi air panas terlalu lama
```

---

## 7. Tabel di Badan Artikel

- Pakai tabel untuk perbandingan dua opsi atau lebih, atau data dengan beberapa atribut (minimal 3 baris).
- Selalu ada paragraf sebelum tabel yang menjawab inti bagian tersebut. Tabel melengkapi teks, bukan menggantikannya.
- Baris pertama adalah header. Isi sel ringkas.
- Tabel wajib tabel asli di semua channel kecuali teks polos.

---

## 8. Tipografi dan Gaya Bahasa

- **Istilah asing dicetak miring** di badan artikel dan heading setiap kali muncul (*scatter plot*, *skincare*, *online*, *marketplace*, *bundling*). Sel tabel meta tidak diberi italic.
- Jangan memiringkan nama orang, merek, singkatan umum (SPSS, SEO, BPOM, SPF), atau kata serapan baku (variabel, korelasi, data, dokter, video).
- Untuk artikel populer, pakai sudut pandang "kamu/-mu" secara konsisten (jangan berganti ke "kita" atau "Anda"). Untuk artikel bisnis formal atau ilmiah, pakai gaya netral-profesional.
- **Tanpa meta-writing:** jangan menulis "Dalam artikel ini…", "Pada bagian ini kita akan…", atau "Artikel ini membedah…". Langsung tulis substansinya.
- Batasi em dash (`—`): maksimal satu per paragraf dan tidak dipakai di heading. Ganti dengan titik, koma, atau tanda kurung.

---

## 9. Gambar dan Caption

- Saran gambar ditaruh **setelah paragraf pembuka sebuah bagian**, tidak pernah tepat di bawah heading. Paragraf pertama setelah heading selalu berisi jawaban langsung.
- Format, dengan masing-masing sebagai paragraf terpisah:

```markdown
[Gambar: ilustrasi tiga scatter plot berdampingan untuk korelasi positif, negatif, dan nol]

Contoh Pola Korelasi Positif, Negatif, dan Nol | Sumber: Nama Situs
```

- Baris pertama berisi instruksi visual untuk tim grafis. Baris kedua berisi caption plus sumber. Jika gambar dibuat tim internal, hapus bagian sumbernya.
- Untuk artikel 1.000–1.500 kata, biasanya 3–5 gambar. Jangan menyebut sumber gambar yang tidak pernah dibuka.

---

## 10. Menyebut Sumber, Link, dan Baca Juga

### Sumber di dalam kalimat adalah link

- Setiap kali badan artikel menyebut sumber (jurnal, media, lembaga, regulator, atau pernyataan seorang dokter yang dimuat di sebuah halaman), **nama sumbernya menjadi link inline** ke halaman yang benar-benar dibuka saat menulis. Contoh: `[*International Journal of Dermatology*](https://pubmed.ncbi.nlm.nih.gov/39444151/)`.
- Yang ditautkan adalah **nama sumbernya** (satu sampai lima kata), bukan satu kalimat penuh. Tautkan pada penyebutan pertama di setiap bagian H2, supaya paragraf tetap jelas bila dibaca terpisah. Jangan menautkan nama yang sama berkali-kali dalam satu paragraf.
- Link menuju **halaman spesifik** (artikel, abstrak, atau dokumen yang memuat klaimnya), bukan beranda situs.
- **Klaim status regulasi** (izin edar, larangan, peringatan) ditautkan ke halaman regulatornya sendiri (BPOM, Kemenkes, OJK). Kutipan media saja tidak cukup untuk klaim semacam ini.
- Buku, jurnal cetak, atau sumber tanpa URL ditulis nama dan tahunnya tanpa link.
- URL belum ada atau belum dibuka: tulis `[isi: URL sumber X]` dan catat di Catatan Editor. **Dilarang menebak URL.**
- Setiap sumber yang ditautkan tetap tercantum di Referensi.
- Utamakan sumber primer. Bila hanya ada kutipan sekunder, misalnya media yang mengutip seorang dokter, tautkan halaman yang benar-benar dibuka dan sebut siapa yang berbicara: "dr. X menjelaskan kepada [Nama Media](URL) bahwa…". Jangan menumpuk rantai "Menurut A yang mengutip B".

### Menulis sumber dengan bahasa yang wajar

- **Sumber jadi subjek, lalu kata kerja aktif yang umum:** menemukan, menyimpulkan, melaporkan, menyarankan, menyatakan, mencatat.
- **Satu kalimat satu temuan.** Jangan menumpuk jenis studi, nama jurnal, tahun, objek kajian, temuan, dan tafsir dalam satu kalimat. Taruh temuannya di kalimat pertama, lalu artinya bagi pembaca di kalimat kedua.
- **Tanpa "satu" atau "sebuah" di depan jenis studi** (jiplakan *a systematic review*). Tulis "Tinjauan sistematis di [Nama Jurnal] (2025) menemukan…".
- **Tanpa "alias", "yakni", atau "bersifat X"** untuk menjelaskan ulang kata yang baru ditulis. Pilih satu kata sehari-hari ("hilang", "tidak bertahan"). Jika istilah teknis memang perlu, beri padanannya dalam tanda kurung.
- **Tulis temuan persis seperti yang dinyatakan sumber.** Buka abstrak atau halamannya sebelum menulis. Jangan menambah kesimpulan yang tidak ada di sumber, dan jangan memindahkan kesimpulan satu rute atau kelompok ke rute atau kelompok lain. Jika sumbernya hanya menemukan satu uji kecil, sebut apa adanya.

SALAH (nyata dari satu draf, padat dan kaku, dan temuannya tidak sesuai sumber):

> Satu tinjauan sistematis di International Journal of Dermatology (2025) terhadap bukti glutathione intravena mencatat perbaikan warna kulit yang didapat bersifat reversibel, alias kembali ke kondisi semula begitu pemberian dihentikan.

BENAR (abstrak PubMed 39444151 diperiksa Oktober 2026):

> Tinjauan sistematis di [*International Journal of Dermatology*](https://pubmed.ncbi.nlm.nih.gov/39444151/) (2025) hanya menemukan satu uji berpembanding plasebo untuk glutathione intravena, dan hasilnya tidak berbeda bermakna secara statistik dari plasebo. Para penulisnya menyimpulkan glutathione intravena dikontraindikasikan (tidak boleh dipakai) untuk mencerahkan kulit karena kurang efektif dan menimbulkan efek samping.

SALAH (sumber tanpa link, rantai kutipan, dan penguat kosong "pada dasarnya"):

> Menurut Media Indonesia yang mengutip dr. Gregory Budiman, M.Biomed, pemberian obat lewat jalur intravena pada dasarnya diperuntukkan bagi pasien yang kondisinya tidak memungkinkan menerima obat lewat mulut, bukan untuk tujuan estetika rutin.

BENAR:

> dr. Gregory Budiman, M.Biomed menjelaskan kepada [Media Indonesia](https://contoh.com/artikel-media-indonesia) bahwa obat intravena disiapkan untuk pasien yang tidak bisa menerima obat lewat mulut, bukan untuk perawatan estetika rutin. Dokter bedah plastik dr. Tompi juga tidak merekomendasikan infus whitening dan meminta masyarakat memastikan izin edar BPOM sebelum menjalani tindakan suntik apa pun [isi: URL sumber pernyataan dr. Tompi].

### Internal link dan Baca Juga

- **Link internal:** tautkan istilah penting saat pertama kali muncul ke artikel lain di situs yang sama, hanya ke URL yang benar-benar diberikan user atau ditemukan di situsnya.
- **Baca Juga:** 1–2 kali per artikel, di akhir sebuah bagian H2:

```markdown
**Baca Juga:** [Judul Asli Artikel Terkait](https://contoh.com/artikel)
```

- Jika URL belum ada, tulis `**Baca Juga:** [isi: artikel tentang topik X]` dan catat di Catatan Editor.

---

## 11. FAQ

- H2 memakai heading FAQ dari outline. Jika tidak ada, pakai `Pertanyaan Seputar <Topik Spesifik>`, bukan sekadar label "FAQ".
- Setiap pertanyaan menjadi H3 tanpa nomor, diambil dari pertanyaan nyata (People Also Ask atau outline), bukan karangan.
- Kalimat pertama jawaban langsung menjawab pertanyaannya. Panjang jawaban 2–3 kalimat (sekitar 30–50 kata), dan boleh dibuka dengan "Ya." atau "Tidak."

---

## 12. Bagian Penutup

H2 penutup berisi langkah nyata berikutnya bagi pembaca, bukan rangkuman ulang berjudul "Kesimpulan". Pakai heading pernyataan:

- Kesehatan: "Tanda Kamu Perlu ke Dokter Kulit" atau "Konsultasi Dokter sebelum Memutuskan Tindakan"
- Bisnis/tools: "Langkah Pertama Minggu Ini"
- Konsep/metodologi: "Kapan Metode Ini Tepat Dipakai"

Tanpa salam penutup ("Semoga bermanfaat!") dan tanpa janji hasil.

---

## 13. Referensi

```markdown
**Referensi:**

- [Judul Asli Halaman](https://contoh.com/halaman) | Nama Situs
- Nama Penulis, Inisial. (Tahun). *Judul Buku*. Nama Penerbit.
```

- Masukkan hanya sumber yang benar-benar dibuka dan dipakai saat menulis. Judul ditulis sesuai judul asli halaman.
- Jangan membuat referensi palsu, dekoratif, atau hasil tebakan URL.
- Untuk YMYL, setiap klaim efektivitas, keamanan, dosis, atau status regulasi harus bisa ditelusuri ke salah satu entri Referensi (lihat [ymyl-claim-gate.md](ymyl-claim-gate.md)).

---

## 14. Catatan Editor

Bagian paling bawah, dipisah garis, **tidak untuk dipublikasikan**.

**Wajib** dibuat bila:

- Topiknya YMYL (kesehatan, obat, tindakan klinik, keuangan, hukum)
- Ada placeholder `[isi: …]`, `[Verifikasi: …]`, atau `[Pengalaman: …]` yang belum terisi
- Outline memberi penanda **[Review medis]**

Isinya, dalam bentuk list:

- Klaim atau data yang belum terverifikasi beserta jenis sumber yang perlu dicari
- Status regulasi yang ditemukan (YMYL)
- Placeholder yang harus diisi (harga, tautan internal, pengalaman, atau kutipan praktisi)
- Untuk YMYL: "Perlu ditinjau dokter/apoteker sebelum terbit" dan "Cek ulang Title dan Description"

```markdown
---

**Catatan Editor (tidak untuk dipublikasikan)**

- [Verifikasi: golongan obat adapalen di PIONAS BPOM]
- Perlu ditinjau dokter kulit sebelum terbit
```

---

## 15. Panjang Artikel

- Default **minimal 1.000 kata substansi**. Tabel meta, instruksi gambar, Referensi, dan Catatan Editor tidak dihitung. Ikuti target dari user atau outline bila ada.
- Pada topik YMYL, target kata **tidak boleh** dipenuhi dengan klaim tambahan yang tidak bersumber. Lebih baik artikel lebih pendek daripada berisi pengisi yang menyesatkan.

---

## 16. Spesifikasi Tampilan (Google Docs dan .docx)

Berlaku untuk channel Google Docs dan .docx. Cara menerapkannya ada di output-channels.md.

| Elemen | Pengaturan |
|---|---|
| Teks badan | Arial 11 pt, line spacing 1.15, spacing after 10 pt, spacing before 0, rata kiri-kanan |
| H2 | Style Heading 2, Arial 16 pt, tebal, hitam, *keep with next* |
| H3 | Style Heading 3, Arial 14 pt, tebal, hitam, *keep with next* |
| List | List asli (bullet atau numbering), tanpa simbol yang diketik |
| Tabel | Tabel asli, garis 1 px, baris header tebal |
| Instruksi gambar dan caption | Rata tengah, 11 pt reguler |
| Referensi | List asli, 10–11 pt |
| Jarak | Hanya dari pengaturan paragraf, tanpa paragraf kosong |
