# 14 · Kebijakan Spam Google Search

> Sumber: **"Spam policies for Google web search"** (Google Search Central, developers.google.com/search/docs/essentials/spam-policies), terakhir diperbarui **28 Agu 2026**, dicek Okt 2026. Ini **dokumen terpisah dari SQRG**: SQRG memandu rater menilai kualitas, sedangkan kebijakan ini menetapkan apa yang dianggap spam oleh sistem Google dan manual action. Ditulis ulang dan dipadatkan, bukan terjemahan kata per kata. Rujuk sebagai "Spam policies › <nama bagian>".
> Label **[Penerapan]** = tambahan untuk praktik SEO/konten, bukan isi kebijakan.
> Pembahasan spam versi SQRG ada di `03-pq-lowest.md` bagian 7. Padanan bahasa Inggris: `references/en/14-spam-policies.md`.

## Daftar isi
1. Cakupan dan konsekuensi
2. Peta ke SQRG
3. Menipu crawler vs pengguna: cloaking, sneaky redirect, teks dan link tersembunyi
4. Memanipulasi cakupan query: doorway abuse, keyword stuffing
5. Konten tanpa nilai tambah: scaled content abuse, scraping, thin affiliation
6. Meminjam otoritas: expired domain abuse, site reputation policy (dengan perubahan EEA)
7. Link spam
8. Keamanan dan kerugian pengguna: hacked content, malicious practices, misleading functionality, user-generated spam
9. Machine-generated traffic
10. Praktik lain yang bisa menyebabkan demotion atau penghapusan
11. Implikasi untuk pembuat konten dan audit

---

## 1. Cakupan dan konsekuensi

- **Definisi spam:** teknik untuk menipu pengguna atau memanipulasi sistem Google agar konten tampil menonjol. Kini secara eksplisit termasuk **upaya memanipulasi jawaban AI generatif di Google Search**, bukan hanya ranking.
- **Cakupan:** semua hasil web search (halaman, gambar, video, berita, dan konten lain), termasuk properti milik Google sendiri. Konten juga harus mematuhi kebijakan konten umum Google Search.
- **Penegakan:** sistem otomatis, ditambah review manusia bila perlu yang bisa berujung **manual action**. Situs yang melanggar bisa turun peringkat atau hilang dari hasil.
- Pengguna bisa melaporkan spam lewat search quality user report; Google terutama memakai laporan ini untuk memperbaiki deteksi otomatis.
- **Daftarnya tidak lengkap.** Google bisa bertindak terhadap praktik spam apa pun yang terdeteksi.

## 2. Peta ke SQRG

| Kebijakan spam | Bagian SQRG terkait (file) |
|---|---|
| Expired domain abuse | 4.6.3 (`03` §7.3) |
| Site reputation policy | 4.6.4 (`03` §7.4) |
| Scaled content abuse | 4.6.5 (`03` §7.5) |
| Scraping | 4.6.6–4.6.7 (`03` §7.6, §8) |
| Hacked content, user-generated spam | 4.6.2 (`03` §7.2) |
| Teks tersembunyi | 4.5.4 (`03` §6.4) |
| Malicious practices, scam dan fraud | 4.5.3, 4.5.5 (`03` §6.3, §6.5) |
| Misleading functionality | 4.5.3 tujuan/desain menipu (`03` §6.3) |
| Thin affiliation | 4.5.3, 4.6.6 (`03` §6.3, §7.6); `05` |
| Cloaking, sneaky redirect, doorway, keyword stuffing, link spam, machine-generated traffic | Tidak dibahas rinci di SQRG; file ini rujukan utamanya |

## 3. Menipu crawler vs pengguna

### 3.1 Cloaking
- **Apa itu:** menyajikan konten berbeda ke mesin pencari dan ke pengguna, untuk memanipulasi ranking dan menyesatkan pengguna.
- Contoh: crawler mendapat halaman wisata sementara pengguna mendapat halaman obat diskon; keyword disisipkan hanya jika user agent-nya mesin pencari.
- **Bukan cloaking:** paywall atau konten berbatas akses, **asalkan** Google bisa melihat konten penuh seperti pengguna yang berhak dan situs mengikuti panduan Flexible Sampling.
- Teknologi yang sulit di-crawl (JavaScript, gambar) sebaiknya dibuat bisa diakses keduanya, bukan "diakali" dengan versi khusus crawler.
- Situs yang diretas sering memakai cloaking supaya pemiliknya tidak sadar.

### 3.2 Sneaky redirect
- **Apa itu:** redirect yang bertujuan menipu: menampilkan konten berbeda ke mesin pencari dan pengguna, atau mengirim pengguna ke tempat yang tidak sesuai kebutuhan awalnya.
- Contoh: crawler melihat satu halaman sementara pengguna dialihkan ke tempat lain; pengguna desktop mendapat halaman normal sementara pengguna mobile dikirim ke domain spam.
- **Redirect yang sah:** pindah alamat situs, menggabungkan beberapa halaman, mengarahkan pengguna yang sudah login ke halaman internal.
- Ujinya: apakah redirect itu dimaksudkan untuk menipu pengguna atau mesin pencari?

### 3.3 Hidden text and link abuse
- **Apa itu:** menaruh konten hanya untuk mesin pencari, tidak mudah dilihat manusia.
- Contoh: teks putih di latar putih; teks di balik gambar; teks digeser keluar layar dengan CSS; ukuran font atau opacity 0; link hanya pada satu karakter kecil (misalnya tanda hubung).
- **Boleh (bukan pelanggaran):** accordion/tab, slider/slideshow, tooltip yang muncul saat interaksi, teks khusus screen reader untuk aksesibilitas.

## 4. Memanipulasi cakupan query

### 4.1 Doorway abuse
- **Apa itu:** situs atau halaman yang dibuat untuk ranking di query spesifik yang mirip-mirip, lalu menggiring pengguna ke halaman perantara yang kurang berguna dibanding tujuan akhirnya.
- Contoh: banyak situs dengan variasi URL/beranda yang tipis; banyak domain atau halaman per kota/wilayah yang semuanya bermuara ke satu halaman; halaman yang dibuat untuk menggiring pengunjung ke bagian situs yang benar-benar berguna; halaman-halaman nyaris sama yang lebih mirip hasil pencarian daripada hierarki yang bisa dijelajahi.

### 4.2 Keyword stuffing
- **Apa itu:** menjejali halaman dengan keyword atau angka untuk memanipulasi ranking, sering berupa daftar, di luar konteks, atau tidak wajar.
- Contoh: daftar nomor telepon tanpa nilai tambah berarti; blok teks berisi daftar kota/wilayah yang ingin ditarget; frasa yang sama diulang sampai terbaca tidak wajar.

## 5. Konten tanpa nilai tambah

### 5.1 Scaled content abuse
- **Apa itu:** membuat banyak halaman terutama untuk memanipulasi ranking, bukan membantu pengguna; biasanya konten tidak orisinal dan bernilai rendah, **apa pun cara pembuatannya**.
- Contoh: AI generatif atau alat serupa menghasilkan banyak halaman tanpa nilai tambah; scraping feed/hasil pencarian/konten lain menjadi banyak halaman, termasuk lewat sinonim, terjemahan, atau penyamaran otomatis lain; menjahit konten dari berbagai halaman tanpa nilai tambah; menyebar konten ke banyak situs untuk menyembunyikan skala produksinya; banyak halaman yang tidak masuk akal bagi pembaca tetapi berisi keyword pencarian.
- Jika konten semacam itu ada di situsmu, keluarkan dari Search.

### 5.2 Scraping
- **Apa itu:** mengambil konten dari situs lain (sering otomatis) dan memuatnya untuk memanipulasi ranking.
- Contoh: menerbitkan ulang tanpa konten atau nilai orisinal, kadang tanpa menyebut sumber; menyalin dengan sedikit ubahan (ganti sinonim, penulisan ulang otomatis); memuat ulang feed tanpa manfaat unik; situs yang hanya meng-embed atau mengumpulkan video/gambar/media milik orang lain tanpa nilai tambah berarti.

### 5.3 Thin affiliation
- **Apa itu:** halaman dengan link affiliate yang deskripsi dan review produknya disalin langsung dari merchant, tanpa konten atau nilai orisinal.
- Sering bagian dari program yang membagikan konten sama ke banyak affiliate: template seragam yang berulang di satu situs atau lintas domain dan bahasa.
- **Menjadi affiliate bukan masalahnya.** Halaman affiliate yang baik memberi nilai tambah: info harga tambahan, review orisinal, pengujian dan rating yang ketat, navigasi produk/kategori, perbandingan produk.

## 6. Meminjam otoritas

### 6.1 Expired domain abuse
- **Apa itu:** membeli domain kedaluwarsa dan memakainya ulang terutama untuk memanipulasi ranking dengan konten bernilai rendah atau tanpa nilai.
- Contoh: konten affiliate di domain bekas lembaga pemerintah; produk medis komersial di domain bekas lembaga amal kesehatan nirlaba; konten kasino di domain bekas sekolah dasar.

### 6.2 Site reputation policy
- **Apa itu:** konten pihak ketiga yang diterbitkan di situs host **terutama karena sinyal ranking yang sudah dimiliki host** (diperoleh dari konten first-party-nya), agar ranking-nya lebih baik daripada jika berdiri sendiri.
- **Pihak ketiga** = entitas yang terpisah dari host: pengguna situs, freelancer, layanan white-label, orang yang tidak dipekerjakan langsung oleh host.
- **Konten pihak ketiga saja tidak masalah.** Jadi masalah hanya jika alasan utama memuatnya adalah menumpang sinyal ranking host.

| Melanggar kebijakan | Tidak melanggar |
|---|---|
| Situs pendidikan memuat review pinjaman online bersponsor yang disebar pihak ketiga ke banyak situs | Kantor berita (wire service), layanan rilis pers |
| Situs medis memuat halaman iklan "kasino terbaik" pihak ketiga yang berkualitas rendah dan tidak terintegrasi, demi memanfaatkan sinyal host | Media berita yang memuat berita sindikasi |
| | Situs yang memang dibuat untuk UGC (forum, kolom komentar) |
| | Kolom, opini, artikel, dan karya editorial lain |
| | Advertorial/native ads yang ditujukan ke pembaca (misalnya dipromosikan di dalam publikasi), bukan untuk memanipulasi ranking |
| | Link affiliate yang diperlakukan dengan benar (lihat §7); unit iklan pihak ketiga |

**Cara review manusia menilai integrasi** (berlaku global). Pertanyaannya: apakah konten dibuat dengan masukan, pengawasan editorial, atau kontribusi yang cukup dari host sehingga benar-benar terintegrasi? Faktor yang bisa dipertimbangkan:
1. **Penyajian:** desain, format, tipografi, dan UX konsisten dengan host.
2. **Kualitas:** ada masalah kualitas di halaman itu yang tidak ada di domain utama.
3. **Kepengarangan:** ada pengakuan eksplisit siapa pemilik/penanggung jawab konten; ada tanda yang membantah klaim penulisnya.
4. **Duplikasi:** konten identik atau nyaris identik muncul di banyak situs lain.

Tidak ada satu faktor pun yang wajib atau cukup dengan sendirinya; bukti lain juga bisa dihitung (misalnya halaman itu bagian dari materi pemasaran pihak ketiga untuk memanipulasi ranking).

**Contoh kasus dari kebijakan (diparafrasekan):**
- **Kecil kemungkinan ditindak: bagian kupon yang terintegrasi.** Penerbit membuat bagian promo bersama mitra spesialis (meski di CMS berbeda) dalam subfolder yang ditautkan dari beranda dan artikel, dikelompokkan dengan kategori khas penerbit, diungkapkan jelas sebagai konten komersial, penerbit tercantum sebagai penanggung jawab editorial, dirujuk di konten editorial/newsletter, dan ada cara mudah melaporkan kode yang bermasalah.
- **Kemungkinan besar ditindak: artikel affiliate tanpa penulis dan tidak terintegrasi.** Media bisnis ternama memuat artikel marketplace minyak CBD tanpa penulis atau editor penanggung jawab, tanpa disclaimer komersial, tidak bisa dijangkau dari beranda atau rubrik, dan menduplikasi konten dari marketplace pihak ketiga.
- **Kecil kemungkinan ditindak: konten affiliate freelancer yang orisinal dan bernama penulis.** Rubrik masakan baru di situs berita, ditulis freelancer yang namanya tercantum dan mewawancarai chef, dengan tanggung jawab editorial yang jelas dan branding konsisten. Freelancer itu juga menulis untuk media lain, tetapi pilihan materinya khusus untuk host ini; link affiliate diberi tanda jelas.

**Konsekuensi tergantung lokasi pengguna** (perubahan diumumkan Agu 2026):
- **Di luar EEA:** halaman yang dinilai melanggar bisa terkena **manual action** pada hasil yang ditampilkan ke pengguna di luar EEA.
- **Di dalam EEA:** halaman bisa **dikategorikan terpisah dari domain utama** dan dinilai berdasarkan kualitasnya sendiri (misalnya konten kasino bersaing dengan konten kasino lain), **tanpa dampak manual action**.
- Google biasanya mengasumsikan halaman baru dan halaman individual setara kualitasnya dengan bagian lain domain; kategorisasi terpisah menghapus asumsi itu. Bagian tersebut tidak langsung kehilangan sinyal situs utama; seiring waktu sistem belajar memberi ranking tiap bagian secara terpisah. Kategorisasi itu sendiri bukan sinyal ranking.
- Situs yang terdampak diberi tahu lewat laporan Manual actions dan pusat pesan Search Console, lalu bisa memperbaiki atau mengajukan reconsideration request. Di EEA ada proses reconsideration yang lebih cepat dengan alasan yang lebih rinci, dan situs yang memenuhi syarat bisa memakai mediasi (penyelesaian sengketa alternatif).
- **Poin FAQ:** manual action di luar EEA tidak memengaruhi ranking di EEA dan tidak dipakai sebagai sinyal di EEA; `noindex` untuk konten yang terkena manual action di luar EEA tidak wajib, dan tidak memasangnya tidak dianggap circumvention; manual action lama di EEA di bawah kebijakan ini dicabut dan tidak dipakai sebagai sinyal ranking.

## 7. Link spam

**Apa itu:** membuat link ke atau dari situs terutama untuk memanipulasi ranking. Contoh:
- Jual-beli link untuk ranking: uang, barang, atau jasa ditukar dengan link atau postingan berisi link, termasuk mengirim produk gratis dengan syarat ditulis ulasan berlink.
- Tukar link berlebihan, atau halaman partner yang ada hanya untuk saling menautkan.
- Program atau layanan otomatis untuk membuat link.
- Mewajibkan link dalam syarat layanan atau kontrak tanpa memberi pemilik konten pilihan untuk menandai (nofollow) link keluarnya.
- Iklan teks atau link teks yang tidak memblokir kredit ranking.
- Advertorial/native ads berbayar dengan link yang meneruskan kredit ranking, atau anchor penuh keyword di artikel, guest post, atau rilis pers yang disebar ke situs lain.
- Link dari direktori atau situs bookmark berkualitas rendah.
- Link penuh keyword, tersembunyi, atau berkualitas rendah di widget yang disebar ke banyak situs.
- Link yang disebar luas di footer atau template berbagai situs.
- Komentar forum dengan link teroptimasi di isi atau tanda tangan.
- Konten bernilai rendah yang dibuat terutama untuk memanipulasi sinyal link.

**Boleh:** link berbayar untuk iklan dan sponsor itu wajar, **asalkan ditandai** dengan `rel="sponsored"` atau `rel="nofollow"` pada tag `<a>`.

## 8. Keamanan dan kerugian pengguna

### 8.1 Hacked content
Konten yang ditaruh di situs tanpa izin lewat celah keamanan. Jenisnya:
- **Code injection:** JavaScript berbahaya di halaman atau iframe.
- **Page injection:** halaman spam atau phishing baru ditambahkan ke situs; halaman lama bisa tampak normal.
- **Content injection:** ubahan halus pada halaman yang ada, misalnya link/teks tersembunyi atau cloaking.
- **Redirect:** kode sisipan yang mengalihkan sebagian pengguna ke halaman berbahaya, sering bergantung pada referrer, user agent, atau perangkat (misalnya hanya pengunjung dari hasil Google yang dialihkan).

### 8.2 Malicious practices
Praktik yang membuat hasil berbeda dari harapan pengguna dan merugikan pengalaman, keamanan, atau privasinya:
- **Malware:** software yang dirancang merusak perangkat atau penggunanya. Pemilik situs kadang menyimpannya tanpa sadar.
- **Unwanted software:** file eksekusi/aplikasi yang menipu atau mengganggu, misalnya mengganti beranda browser atau membocorkan data pribadi tanpa pemberitahuan.
- **Back button hijacking:** memanipulasi riwayat browser sehingga pengguna tidak bisa langsung kembali ke halaman asalnya.

### 8.3 Misleading functionality
Situs yang berpura-pura menyediakan konten atau layanan yang sebenarnya tidak ada. Contoh: "generator kredit app store" palsu; alat "gabung PDF", timer, atau kamus yang ternyata menggiring pengguna ke iklan menipu.

### 8.4 User-generated spam
Spam yang ditambahkan pengguna lewat saluran untuk konten pengguna, sering tanpa disadari pemilik: akun spam di layanan hosting terbuka, postingan spam di forum, spam komentar blog, file spam di layanan file hosting.

## 9. Machine-generated traffic

Mengirim query otomatis ke Google tanpa izin tertulis, termasuk **scraping hasil pencarian untuk cek ranking**. Ini melanggar kebijakan spam dan Persyaratan Layanan Google.

**[Penerapan]** Relevan saat memilih rank tracker dan tool SERP: utamakan API resmi atau penyedia yang beroperasi dalam akses yang diizinkan.

## 10. Praktik lain yang bisa menyebabkan demotion atau penghapusan

- **Legal removals:** banyaknya permintaan penghapusan hak cipta yang sah bisa membuat konten lain di situs yang sama diturunkan. Sinyal serupa berlaku untuk pencemaran nama baik, barang palsu, dan penghapusan atas perintah pengadilan. CSAM selalu dihapus, dan situs dengan porsi CSAM signifikan diturunkan seluruhnya.
- **Personal information removals:** situs dengan praktik penghapusan yang eksploitatif (misalnya memungut biaya untuk menghapus data pribadi) dan volume penghapusan tinggi akan diturunkan, dan Google mencari pola serupa di situs lain. Demotion serupa bisa berlaku untuk konten doxxing dan citra eksplisit tanpa persetujuan, termasuk konten eksplisit palsu.
- **Policy circumvention:** terus melanggar lewat subdomain, subdirektori, atau situs baru/lama, atau cara lain untuk tetap menyebarkan konten yang melanggar. Konsekuensinya bisa berupa hilangnya kelayakan fitur seperti Top Stories dan Discover, serta penghapusan bagian situs yang lebih luas.
- **Scam dan fraud:** meniru bisnis atau layanan resmi, info bisnis yang sengaja dipalsukan, atau menarik pengguna dengan dalih palsu. Contoh: meniru perusahaan terkenal agar pembayaran masuk ke pihak yang salah; situs "layanan pelanggan resmi" palsu atau info kontak palsu.

## 11. Implikasi untuk pembuat konten dan audit

**[Penerapan]**
- **Kebijakan spam vs SQRG:** SQRG menjelaskan penilaian kualitas; kebijakan spam menjelaskan apa yang bisa memicu demotion atau manual action. Audit sebaiknya mengecek keduanya: SQRG untuk kualitas, file ini untuk spam teknis, link, dan distribusi.
- **Halaman programmatic dan halaman lokasi:** set halaman per kota/wilayah harus punya nilai lokal nyata di tiap halaman (ketersediaan layanan sebenarnya, data lokal, bukti lokal). Template yang hanya mengganti nama kota terlihat seperti doorway dan bisa juga scaled content abuse.
- **Link berbayar dan kerja sama:** setiap postingan bersponsor, barter produk untuk review, penempatan partner, dan link affiliate sebaiknya memakai `rel="sponsored"` (atau `nofollow`). Jangan pernah mensyaratkan link do-follow dalam kesepakatan.
- **Guest post dan rilis pers:** hindari anchor penuh keyword yang mengarah ke halaman money page.
- **Bagian pihak ketiga** (kupon, review partner, konten freelancer di topik baru): integrasikan ke navigasi, desain, dan tanggung jawab editorial; cantumkan penulis dan editor penanggung jawab; beri label konten komersial; jangan menerbitkan teks yang sama dengan yang disebar partner ke tempat lain.
- **Konten AI:** kebijakan ini menyasar volume tanpa nilai "apa pun cara pembuatannya", dan kini eksplisit mencakup manipulasi jawaban AI generatif. Jangan membuat halaman yang tujuan utamanya dicomot AI Overviews/AI Mode tanpa melayani pembaca.
- **Cek teknis saat audit:** bandingkan apa yang diterima Googlebot dengan yang dilihat pengguna (URL Inspection, ganti user agent); uji redirect di mobile dan desktop serta dari rujukan Google; cari teks/link tersembunyi di DOM; cek laporan Manual actions dan Security issues di Search Console.
- **Keamanan dan UGC:** pantau halaman sisipan (misalnya pencarian `site:` untuk URL aneh), moderasi komentar dan forum, pakai `rel="ugc"`/`nofollow` untuk link dari pengguna.
- **Cek ranking:** hindari tool yang men-scrape Google tanpa izin (machine-generated traffic).
