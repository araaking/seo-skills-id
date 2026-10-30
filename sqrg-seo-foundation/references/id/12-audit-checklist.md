# Checklist Audit Konten Berbasis SQRG

> Alat kerja praktis yang diturunkan dari SQRG 11 Sep 2025. Urutannya mengikuti logika rater: **cek bahaya dan spam dulu, baru kualitas.** Angka di kurung menunjuk file referensi untuk detailnya.

## Cara pakai

1. Kumpulkan bahan: URL atau teks halaman, keyword target (jika ada), info penulis/situs, dan jika bisa, beberapa hasil teratas pesaing untuk kalibrasi.
2. Jalankan **Tahap 0–2** berurutan. Jika ada temuan merah di Tahap 1, laporkan sebagai prioritas utama; tahap lain tetap diisi agar perbaikannya lengkap.
3. Perkirakan rating PQ dan, jika ada keyword target, rating NM. Jika ragu antara dua rating, pilih yang lebih rendah.
4. Tulis laporan dengan template di bagian akhir.

---

## Tahap 0 · Konteks

- [ ] **Tujuan halaman** jelas dan bermanfaat? Tuliskan dalam satu kalimat. (01)
- [ ] **Tipe situs**: blog pribadi, media, toko online, lembaga, forum/UGC, situs resmi? Ekspektasinya berbeda. (02)
- [ ] **Tingkat YMYL**: jelas YMYL / mungkin / bukan. Kategori: kesehatan-keselamatan, keuangan, pemerintahan-kewargaan-masyarakat, lainnya. (01)
- [ ] **Intent keyword target**: Know, Know Simple, Do, Website, atau Visit-in-Person; interpretasi dominan dan minor yang wajar. (08)
- [ ] **Locale**: bahasa dan wilayah pembaca (default: Indonesia, bahasa Indonesia). (10)

## Tahap 1 · Saringan merah (pemicu Lowest) (03, 04)

Satu saja "ya" = risiko Lowest.

**Bahaya**
- [ ] Mendorong tindakan yang membahayakan diri/orang lain, atau meremehkan risikonya?
- [ ] Merendahkan atau menghasut kebencian terhadap kelompok tertentu (dengan nada serius atau berniat jahat)?
- [ ] Klaim yang jelas salah, bertentangan dengan konsensus ahli, atau teori tanpa dasar, di topik yang bisa merugikan? (Judul yang menyesatkan secara berbahaya juga dihitung.)

**Tidak tepercaya**
- [ ] YMYL atau situs yang menangani uang/data pribadi **tanpa info apa pun** tentang penanggung jawabnya?
- [ ] Profil penulis palsu, persona rekaan, foto penulis buatan AI, atau klaim kredensial yang tidak benar?
- [ ] Klaim "sudah kami uji/review independen" yang tidak bisa dibuktikan?
- [ ] Meniru brand lain, info bisnis palsu (misalnya alamat toko fisik fiktif), atau logo "terpercaya" palsu?
- [ ] Iklan disamarkan sebagai konten atau navigasi; tombol yang menipu?
- [ ] MC tertutup iklan/pop-up yang sulit ditutup, atau terdorong jauh ke bawah oleh iklan?
- [ ] Meminta data pribadi tanpa alasan sah?

**Spam**
- [ ] Seluruh/hampir seluruh MC disalin, diparafrase, di-embed, dibuat otomatis/AI, atau di-repost tanpa effort, orisinalitas, dan nilai tambah?
- [ ] Bagian dari produksi massal halaman bertemplat tanpa kurasi (cek beberapa halaman lain di situs)?
- [ ] Sisa output AI yang tidak diedit, kalimat terpotong, bagian template yang kosong, atau teks yang tidak koheren?
- [ ] Topik jauh di luar fokus situs, terutama YMYL di situs yang tidak relevan?
- [ ] Konten pihak ketiga yang dimuat terutama untuk menumpang otoritas domain (site reputation abuse)?
- [ ] Domain bekas yang isinya tidak nyambung dengan sejarahnya (expired domain abuse)?
- [ ] Keyword diulang-ulang secara tidak wajar; komentar spam; tanda peretasan?

**Spam teknis dan link** (14)
- [ ] Googlebot dan pengguna mendapat konten berbeda (cloaking), atau redirect yang hanya aktif untuk pengguna mobile / pengunjung dari Google (sneaky redirect)?
- [ ] Teks atau link disembunyikan dari manusia (putih di atas putih, CSS keluar layar, ukuran/opacity 0, link di satu karakter kecil)? Accordion, tab, tooltip, dan teks screen reader tidak masalah.
- [ ] Set halaman per kota/wilayah atau varian query yang nyaris sama dan bermuara ke satu tujuan (doorway)?
- [ ] Link berbayar, bersponsor, barter produk, atau partner tanpa `rel="sponsored"`/`nofollow`; anchor penuh keyword di guest post/rilis pers; tukar link atau link di widget/footer yang disebar ke banyak situs?
- [ ] Deskripsi/review affiliate disalin dari merchant tanpa tambahan apa pun (thin affiliation)?
- [ ] Back button hijacking, unduhan malware/unwanted software, atau "tool" yang tidak berfungsi dan menggiring ke iklan (misleading functionality)?
- [ ] Ada laporan Manual actions atau Security issues di Search Console?

## Tahap 2 · Kualitas (Low, Medium, High) (02, 05, 06)

**Main Content**
- [ ] **Effort** terlihat: riset, pengujian, foto/video sendiri, data, contoh, editing yang rapi.
- [ ] **Orisinalitas**: ada sesuatu yang tidak ada di hasil teratas lain (data unik, pengalaman langsung, analisis, contoh lokal).
- [ ] **Skill**: penjelasan cukup terampil sehingga pembaca benar-benar bisa memakai isinya.
- [ ] **Akurasi**: fakta benar; untuk YMYL, sesuai konsensus ahli dan pedoman resmi terbaru; sumber dicantumkan.
- [ ] Kalibrasi: apakah halaman ini lebih baik dari halaman tipikal di topik yang sama? Jika hanya setara, kemungkinan **Medium**.

**Struktur dan pengalaman**
- [ ] Jawaban atau isi utama ada di atas, bukan tertimbun intro panjang.
- [ ] Tidak ada filler: definisi umum, fakta yang semua orang tahu, paragraf pengantar yang berputar-putar.
- [ ] Iklan dan SC tidak mengganggu, terutama di mobile; tidak ada iklan bergambar vulgar atau mengejutkan.
- [ ] Fitur (kalkulator, filter, keranjang, form) berfungsi.

**Judul**
- [ ] H1 dan title tag merangkum isi secara jujur; tanpa superlatif atau klaim heboh yang tidak dipenuhi isi.

**E-E-A-T dan identitas**
- [ ] Penulis jelas: nama, peran, pengalaman/kredensial yang relevan dengan topik.
- [ ] Untuk YMYL yang memberi saran: penulis atau reviewer punya keahlian yang sesuai.
- [ ] Untuk konten pengalaman: pengalaman langsung terlihat dari isi (foto, detail, proses), dan tidak memberi saran yang seharusnya dari ahli.
- [ ] Penerbit jelas: About, Kontak, kebijakan redaksi. Untuk media: Redaksi. Untuk toko: layanan pelanggan, pembayaran, pengiriman, retur.
- [ ] Konflik kepentingan diungkapkan (affiliate, sponsor, produk sendiri). Ingat: pengungkapan tidak menyelamatkan konten tanpa nilai tambah.

**Reputasi** (riset dengan operator `-site:`)
- [ ] Apa kata sumber independen tentang situs dan penulis? Untuk YMYL, apa kata ahli atau lembaga di bidangnya?
- [ ] Review pelanggan: baca isinya, bukan hanya bintangnya. Laporan penipuan yang kredibel = merah.

## Tahap 3 · Needs Met untuk keyword target (08, 09, 10)

- [ ] Menjawab **interpretasi dominan** dan intent utama secara langsung.
- [ ] Semua **aspek kunci query** terpenuhi: tahun, lokasi, jumlah, perbandingan, kata pembatas ("tanpa", "untuk pemula", "terdekat").
- [ ] Format sesuai: jawaban singkat di awal untuk Know Simple; panduan komprehensif untuk Know; alat/langkah/CTA untuk Do; info lokasi akurat untuk Visit-in-Person.
- [ ] **Segar** jika query butuh info terbaru (harga, regulasi, produk, acara berulang); tanggal pembaruan jujur.
- [ ] Bahasa sesuai locale; istilah teknis Inggris hanya di tempat yang memang lazim.
- [ ] Untuk query tanpa satu jawaban benar: menyajikan pengalaman, perspektif, atau pilihan yang beragam.
- [ ] Untuk query produk/kategori: mendukung browsing dan riset (pilihan, foto, spesifikasi, review, perbandingan).
- [ ] Perkiraan NM: FullyM / HM / MM / SM / FailsM, beserta alasannya.

## Tahap 4 · Kasus khusus (pilih yang relevan)

- **Review/affiliate:** bukti pemakaian atau pengujian langsung, kriteria penilaian, kelebihan dan kekurangan yang jujur, foto sendiri. Daftar "terbaik" yang hanya merangkum review orang lain = Low. (03, 05)
- **Programmatic SEO/konten AI massal:** data unik per halaman, QA template (tidak ada bagian kosong), editing manusia, sampling beberapa halaman. (03, 04)
- **E-commerce:** info produk lengkap, review pengguna, layanan pelanggan, kebijakan retur; konsisten di semua halaman kebijakan. (01, 06, 10)
- **Forum/UGC/kolom komentar:** moderasi spam dan perilaku kasar; jawaban substantif; jawaban bersponsor tidak menyamar. (07)
- **Halaman error/404/stok habis:** penjelasan, pencarian, alternatif; pastikan bukan masalah sistemik. (07, 10)
- **Konten pihak ketiga/sponsor:** relevan dengan situs dan pembacanya, diberi label jelas, tidak menyamar sebagai review independen. (03, 04)

---

## Template laporan audit

Gunakan struktur ini (sesuaikan panjangnya dengan permintaan):

**Ringkasan:** satu paragraf: tujuan halaman, tingkat YMYL, perkiraan rating PQ (dan NM jika ada keyword), serta masalah terbesar.

**Temuan merah (risiko Lowest):** daftar temuan beserta bukti dari halaman dan rujukan bagian SQRG (misalnya "SQRG 4.6.6, hal. 42"). Jika tidak ada, tulis "tidak ditemukan".

**Faktor penurun:** yang membuat halaman Low atau tertahan di Medium.

**Faktor penguat:** yang sudah baik dan perlu dipertahankan.

**Needs Met:** seberapa baik halaman menjawab keyword target, aspek query yang terlewat, dan masalah kesegaran atau bahasa.

**Prioritas perbaikan:** urutkan dari dampak terbesar: (1) hilangkan pemicu Lowest, (2) perbaiki akurasi dan E-E-A-T untuk YMYL, (3) tambah nilai orisinal, (4) rapikan struktur, filler, judul, dan iklan, (5) perkuat sinyal reputasi.

**Catatan jujur:** rating adalah perkiraan berdasarkan standar rater, bukan prediksi ranking. Sebutkan juga hal yang tidak bisa dicek (misalnya reputasi yang butuh riset di luar, atau konten di balik login).
