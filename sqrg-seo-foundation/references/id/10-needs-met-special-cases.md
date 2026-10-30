# 10 · Kasus Khusus Needs Met

> Sumber: SQRG 11 Sep 2025, Part 3, bagian 14.0–24.0 (hal. 142–174). Ditulis ulang dan dipadatkan.
> Label **[Penerapan]** = tambahan untuk praktik SEO/konten, bukan isi SQRG.

## Daftar isi
1. Hubungan Page Quality dan Needs Met
2. Flag: porno, bahasa asing, gagal dimuat, flag tambahan
3. Banyak jenis hasil yang membantu
4. Query dengan intent website sekaligus kunjungan langsung
5. Spesifisitas query vs landing page
6. Freshness (kesegaran)
7. Query salah ketik dan query nama orang
8. URL query yang tidak harus Fully Meets
9. Query produk: riset dan browsing
10. Query kunjungan langsung: seberapa dekat itu "dekat"
11. Hasil berbahasa Inggris di locale non-Inggris
12. Hasil kamus dan ensiklopedia
13. Implikasi untuk pembuat konten

---

## 1. Hubungan Page Quality dan Needs Met (14.0, hal. 142–143)

- **Needs Met bergantung pada query dan hasil.** **Page Quality tidak bergantung pada query**; PQ dinilai dari landing page saja.
- Tidak semua result punya slider PQ. Jika ada, nilai dari landing page.
- **HM tidak pantas** untuk halaman yang tidak tepercaya atau punya ciri buruk lain (info usang atau tidak akurat). Standar HM sangat tinggi.
- Halaman dengan PQ sangat rendah sampai tidak membantu atau berbahaya (teks acak, penipuan) → **FailsM**, karena masalah PQ mengganggu kegunaannya. **Pengecualian:** query dengan intent website yang jelas; situs target tetap **FullyM**, karena orang berhak mencari situs apa pun.
- **Hasil yang tidak berguna selalu FailsM, walau PQ landing page-nya tinggi.** Tidak berguna ya tidak berguna.

**Contoh (hal. 143):**
- Gejala dehidrasi: artikel yang topiknya cocok tapi tidak tepercaya dan berpotensi menyesatkan → NM rendah, PQ rendah (YMYL tanpa bukti keahlian). Halaman situs medis yang sangat otoritatif → NM sangat membantu, PQ sangat tepercaya.
- Jumlah oktaf pada gitar: blok menampilkan jumlah oktaf **piano**, dengan link ke halaman piano yang bagus → **FailsM** untuk NM, sementara PQ landing page-nya Medium+ sampai High. **PQ tinggi tidak menyelamatkan jawaban yang salah konteks.**

## 2. Flag (15.0–15.6, hal. 144–151)

Flag dinilai dari **hasilnya saja**, tidak bergantung pada query.

**Porn (15.1–15.2):**
- Flag dipasang untuk semua halaman porno, apa pun query-nya (termasuk iklan porno yang mencolok). Standar budaya bisa berbeda per locale.
- Query yang jelas **tidak** mencari porno (kata umum tentang perempuan, keluarga, mainan, foto mobil, pertanyaan tentang hewan) → hasil porno = **FailsM**. Porno yang tidak diminta adalah pengalaman sangat buruk.
- Query yang **mungkin** bermakna porno (misalnya istilah anatomi) → nilai seolah makna non-porno yang dominan (misalnya info kesehatan/anatomi).
- Query yang **jelas** mencari porno → tetap nilai kegunaannya. Hasil porno tidak otomatis MM/HM; halaman yang mencoba mengunduh malware tetap rendah.

**Pelaporan gambar ilegal (15.3):** prosedur internal rater untuk melaporkan materi pelecehan seksual anak. Tidak relevan untuk SEO; tidak dirangkum di sini.

**Foreign Language (15.4):**
- **Tidak** dipasang jika bahasa landing page adalah bahasa tugas, bahasa yang umum dipakai sebagian besar penduduk di lokasi tugas, atau bahasa Inggris. Contoh: untuk tugas berbahasa Katalan di Spanyol, halaman berbahasa Katalan, Spanyol, dan Inggris tidak diberi flag.
- Dipasang walau rater pribadi paham bahasanya, jika kebanyakan pengguna di locale tidak paham. Dinilai dari bahasa landing page, bukan tampilan blok. Jika ragu, jangan dipasang.
- Halaman berbahasa asing **biasanya FailsM** karena tidak bisa dipahami. **Kecuali** query jelas menginginkannya, misalnya pengguna AS mencari situs mesin pencari Tiongkok → FullyM + flag.
- **Video** sering tetap membantu walau berbahasa asing: lagu, film, atau pertandingan yang diminta bisa dinikmati tanpa memahami bahasanya. Tapi video orang yang **membicarakan** lagu/film itu dalam bahasa asing → FailsM + flag.
- Contoh: video penyanyi Kanada menyanyikan lagu berbahasa Prancis, halaman sebagian besar berbahasa Inggris → sesuai yang dicari, tanpa flag. Cuplikan film Filipina berbahasa Tagalog → membantu banyak pengguna AS yang mencarinya.

**Did Not Load (15.5):**
- Dipasang hanya jika landing page berisi pesan error server/aplikasi tanpa konten lain (tanpa navigasi, link home, SC, atau iklan), atau halaman kosong total. Dinilai dari landing page, bukan blok.
- **Tidak** dipasang untuk: peringatan malware, konten yang sudah dihapus atau kedaluwarsa (iklan baris lewat masa, post dihapus, produk tidak tersedia), atau konten yang butuh langganan.
- Halaman yang benar-benar tidak termuat → FailsM. Halaman error yang dikustomisasi adalah bagian dari situs yang berfungsi baik dan **bisa** tetap membantu.

**Contoh (hal. 150):**
- Sepatu salju anak warna tertentu → halaman error toko bereputasi baik dengan SC banyak, kotak pencarian, tips, dan info layanan pelanggan: NM tidak membantu (tidak ada info produk itu), PQ tetap baik. Tanpa flag.
- Ayat-ayat kitab suci → halaman "tidak ada hasil" di situs referensi terkenal, tapi berisi link ke semua ayat per kitab plus kotak pencarian dan tips: **sangat membantu**. Tanpa flag.
- Tiket teater → peringatan malware: FailsM dan PQ Lowest. Tanpa flag Did Not Load.
- Sebuah film horor → server tidak ditemukan, tanpa MC/SC/iklan: flag Did Not Load, FailsM, tanpa PQ.

**Flag tambahan (15.6):** sebagian tugas meminta flag **Upsetting-Offensive** (konten yang bisa menyinggung atau mengganggu pengguna tipikal di locale itu) dan **Not-for-Everyone** (konten yang kurang pantas di ruang publik, kantor, atau sekolah).

## 3. Banyak jenis hasil yang membantu (16.0, hal. 152)

- Beri HM untuk hasil sangat membantu di **semua** interpretasi dan intent yang wajar, termasuk minor yang wajar. Jangan berasumsi; riset query.
- Untuk satu interpretasi pun, orang berbeda punya intent berbeda (misalnya untuk sebuah film: review, obrolan media sosial, pemeran, cara menonton), dan satu orang bisa punya semuanya sekaligus.
- Hasil yang beragam membantu, bahkan untuk query dengan satu intent jelas: **format** berbeda (teks, video, gambar, audio), **pengalaman dan opini** berbeda (blog pribadi, post media sosial), **kedalaman** berbeda (video ringkas 10 detik vs dokumenter satu jam), **jenis situs** berbeda (korporat, nirlaba, pemerintah, media sosial, forum, blog pribadi).
- Query yang paling butuh keberagaman: yang mencari pengalaman/opini (apakah sebaiknya memelihara anjing), subjektif (musik terbaik untuk lari), eksplorasi/browsing (ide renovasi kamar mandi, jas hitam, cincin tunangan murah), dan tanpa satu jawaban benar (cara minta naik gaji).

## 4. Intent website sekaligus kunjungan langsung (16.1, hal. 152–154)

- Dua intent kuat: (1) ke situsnya (cari info, beli online, reservasi, janji temu, layanan pelanggan); (2) datang langsung.
- **Hasil yang hanya memenuhi satu intent tidak boleh FullyM.**
- Contoh: nama ritel besar, kantor layanan SIM/kendaraan, atau nama bank, dengan lokasi pengguna → blok daftar lokasi terdekat memenuhi intent kunjungan; situs resminya memenuhi intent online (belanja, perpanjang izin, bayar biaya, perbankan online). Keduanya sangat memuaskan, tidak ada yang FullyM.

## 5. Spesifisitas query vs landing page (17.0, hal. 154–157)

- Query bisa umum atau spesifik (kursi → kursi makan → model kursi tertentu dari merek furnitur tertentu). Hasil untuk query spesifik lebih mudah dinilai. **Rating berdasar kegunaan, bukan kecocokan tingkat spesifisitas.**
- Untuk kategori luas (kafe, restoran, hotel, buku, tempat wisata), **contoh yang populer dan menonjol** bisa dianggap sangat membantu.

**Contoh:**
- [credit cards] → halaman perusahaan kartu kredit populer bisa sangat membantu walau lebih spesifik (PQ High+ sampai Highest); daftar kartu terbaik dari situs keuangan konsumen yang direkomendasikan media besar cocok untuk kebanyakan pengguna (PQ High); kartu yang mensyaratkan keanggotaan serikat pekerja = interpretasi minor yang tidak mungkin, walau PQ-nya High.
- [hotels] → halaman hotel di situs agregator perjalanan populer = sangat membantu; homepage jaringan hotel besar = bisa sangat membantu; halaman **satu** cabang hotel tertentu = terlalu spesifik, kurang membantu (walau PQ-nya tetap tinggi).
- Nama ritel besar → halaman pencari lokasi toko = sangat membantu bagi yang ingin datang (dan halaman paling otoritatif soal lokasi toko); halaman satu jenis celana wanita di situs ritel itu = interpretasi tidak mungkin sampai "no chance".

## 6. Freshness (18.0, hal. 158–160)

| Jenis query | Contoh | Asumsi |
|---|---|---|
| Breaking news | Tornado, tsunami | Info dibutuhkan sekarang juga |
| Acara berulang | Olimpiade, ajang pencarian bakat, jadwal tim, formulir pajak, pemilu | Edisi terbaru atau yang akan datang |
| Info terkini | Populasi kota, utang negara, harga tiket pesawat, libur nasional berikutnya | Angka atau info paling mutakhir |
| Produk | Ponsel, model mobil, sistem operasi | Model/versi terbaru |

- Untuk query yang butuh konten baru, **hanya halaman terkini atau yang diperbarui** yang layak NM tinggi. Halaman lama, model/harga lama, atau info usang dianggap **basi** → NM rendah, kadang FailsM.
- Sebagian query punya intent ganda: berita terbaru **dan** info "abadi" (misalnya nama selebriti atau politisi: biografi atau gosip terbaru).
- **Freshness umumnya kurang berpengaruh pada PQ.** Arsip media bereputasi bisa ber-PQ tinggi. Tapi situs yang ditelantarkan atau konten yang tidak dirawat sehingga tidak akurat/menyesatkan → PQ rendah.
- Tanggal terbit bisa berbeda dengan tanggal pembaruan. Sebagian situs selalu menampilkan tanggal hari ini. Wayback Machine bisa membantu melihat riwayat perubahan.

**Contoh:**
- Lalu lintas sebuah kota besar: halaman kondisi hari ini = membantu; halaman kondisi kemarin = **basi dan tidak berguna**, walau baru sehari.
- Pemenang hadiah Nobel Perdamaian: halaman tentang pemenang terbaru = membantu; tentang pemenang beberapa tahun sebelumnya = basi (interpretasi sangat minor).
- Penyakit radang sendi: situs medis otoritatif yang rutin diperbarui = membantu; artikel berita medis belasan tahun lalu = sangat basi, **berpotensi berbahaya**.
- Tanggal lahir seorang presiden masa lalu: tidak butuh hasil segar; fakta yang tidak berubah.

## 7. Query salah ketik dan query nama orang (19.0–19.2, hal. 160–161)

- Salah ketik yang **jelas** (nama perusahaan logistik, tim olahraga, atau penyanyi yang salah eja) → nilai berdasar intent sebenarnya, bukan ejaan.
- Yang **tidak jelas** salah ketik → hormati query apa adanya.
- **Nama orang:** jangan otomatis menganggap salah ketik. Contoh: query dengan nama yang mirip nama komedian terkenal tapi ejaannya berbeda dianggap mencari orang dengan nama persis itu, karena banyak orang bernama demikian.
- Contoh: nama atlet legendaris dengan ejaan nama depan yang tidak lazim → halaman jaringan profesional yang mendaftar semua anggota dengan ejaan itu = sangat membantu. Hasil tentang atlet terkenalnya dianggap interpretasi minor yang tidak mungkin dan agak membantu. Hasil untuk orang yang lebih menonjol dengan nama itu layak rating lebih tinggi daripada yang kurang menonjol.

## 8. URL query yang tidak harus Fully Meets (20.0, hal. 161–162)

- Untuk URL query yang valid, rating **tidak** hanya FullyM atau FailsM. Mencari **info tentang situs itu** (review, berita) adalah intent yang wajar; rater pun memakai cara ini untuk riset reputasi.
- Hasil berisi review dan reputasi bisa sangat membantu. **Situs statistik traffic biasanya tidak membantu.**
- Contoh: URL toko perabot rumah → situsnya sendiri adalah target; halaman kode kupon untuk toko itu di situs kupon terkenal = sangat membantu terutama bagi pembeli rutin; halaman review toko itu di situs review terkenal = membantu bagi calon pembeli baru. URL situs penilaian dosen → situsnya adalah target; artikel ensiklopedia lengkap tentang situs itu (cara penilaian, perbandingan dengan evaluasi di kelas, kritik) = sangat membantu.

## 9. Query produk: riset dan browsing (21.0, hal. 163–164)

- Ada yang jelas Know (review produk), jelas Do (beli produk), jelas Website (produk + situs toko resmi). **Tapi kebanyakan query produk tidak menyebut intent secara eksplisit.**
- Banyak orang senang **browsing** produk online seperti cuci mata di toko. **Beri NM tinggi untuk hasil yang memungkinkan riset, browsing, dan memutuskan.** Untuk barang besar (mobil, peralatan rumah tangga besar), pembelian sering didahului riset (review, spesifikasi), memahami pilihan (merek, model, harga), dan membandingkan.
- **PQ hasil produk butuh perhatian ekstra.**
- Contoh: TV high definition tanpa ukuran/merek → halaman yang menjelaskan jenis-jenis TV plus review banyak model dari situs yang dikenal untuk ulasan elektronik. Jeans balita ukuran tertentu (spesifik) → halaman toko jeans berkualitas dengan banyak pilihan di ukuran itu. Manset kemeja → koleksi besar dari ritel bereputasi dengan filter gaya dan harga. Cincin tertentu dari merek perhiasan → hasil gambar cincin dari berbagai sudut dan bahan.

## 10. Kunjungan langsung: seberapa dekat itu "dekat" (22.0–22.1, hal. 164–166)

- Jika query tidak menyebut lokasi dan ada lokasi pengguna, hasil **di atau dekat lokasi pengguna** paling membantu.
- "Dekat" tergantung jenis tempat: SPBU, kedai kopi, supermarket → orang tidak mau jauh. Dokter, perpustakaan, restoran jenis tertentu, kolam renang umum, jalur hiking → mau sedikit lebih jauh. Klinik sangat spesialis → bisa jauh.
- **Lokasi penting:** upah minimum, pengguna di sebuah negara bagian AS → blok dengan angka yang benar untuk negara bagian itu (harus diverifikasi akurasinya) dan halaman resmi negara bagian itu = sangat membantu; halaman nasional berisi tarif semua negara bagian = sangat membantu meski perlu usaha mencari; halaman resmi negara bagian **lain** = tidak membantu.
- **Lokasi tidak penting:** lowongan kerja di perusahaan teknologi besar → blok tanpa info lowongan = FailsM; halaman karier resmi perusahaan = FullyM, di mana pun penggunanya.

## 11. Hasil berbahasa Inggris di locale non-Inggris (23.0–23.1, hal. 167–172)

**Prinsip:**
- NM mencerminkan kegunaan bagi pengguna **di locale itu**. Jika query dalam bahasa locale, **asumsikan pengguna ingin hasil dalam bahasa itu**.
- Hasil berbahasa Inggris hanya layak NM tinggi jika pengguna di locale itu memang mengharapkannya. Kecuali diminta query, hasil berbahasa Inggris dianggap **tidak berguna** jika kebanyakan pengguna tidak bisa membacanya.
- Setiap locale punya pertimbangan unik: bahasa resmi, bahasa daerah, dialek, aksara, dan bahasa keyboard. **Jika ragu, anggap pengguna lebih suka bahasa tugas** kecuali query jelas menunjukkan sebaliknya.

**Contoh (locale Hindi-India dan Korea):**
- Nama tokoh ditulis dalam aksara lokal → artikel ensiklopedia berbahasa lokal sangat membantu; versi berbahasa Inggris dengan isi serupa sedikit gunanya karena sedikit yang bisa membacanya.
- **Nama diri diketik dalam huruf Latin** (pesepak bola terkenal, judul film + tahun) → pengguna tetap ingin hasil berbahasa lokal (artikel lokal, review dan toko lokal).
- **Query campuran** (bahasa lokal ditulis dalam huruf Latin dengan beberapa kata Inggris, misalnya pertandingan kriket wanita; atau merek + "tablet") → tetap ingin hasil berbahasa lokal, misalnya halaman produk merek itu dalam bahasa lokal.
- **Kapan hasil Inggris memuaskan:** situs resmi organisasi global yang memang dicari (misalnya "situs universitas terkenal" diketik dalam aksara lokal → situs resminya yang berbahasa Inggris memuaskan penuh); info teknis yang lazim ditulis dalam bahasa Inggris (nomor part, spesifikasi, rumus). Contoh: tutorial berbahasa Korea tentang memulihkan sistem operasi switch jaringan, dengan perintah konsol persis dalam bahasa Inggris → sangat membantu.
- Di locale yang bahasa Inggrisnya resmi atau dominan (misalnya Singapura), hasil berbahasa Inggris bisa sangat membantu.

## 12. Hasil kamus dan ensiklopedia (24.0, hal. 172–174)

- Kamus dan ensiklopedia sering relevan secara topik, tapi **tidak membantu untuk kata umum yang sudah dipahami kebanyakan orang**. NM tinggi hanya jika intent-nya "apa itu" atau "apa artinya".
- Untuk kata yang sangat umum, hasil definisi kamus bisa cukup **SM**.
- Contoh: kosakata sulit yang sering muncul di ujian masuk kampus → hasil kamus sangat membantu. Kata "pelangi" → kebanyakan orang sudah tahu artinya; gambar atau deskripsi sederhana lebih membantu daripada kamus. "Kafetaria" dengan lokasi pengguna → kebanyakan mencari tempat makan; artikel ensiklopedia yang mendalam pun kurang membantu. Sejarah mesin ATM → artikel ensiklopedia dengan bagian sejarah yang lengkap sangat membantu. ATM terdekat → artikel ensiklopedia **FailsM** karena tidak ada info lokasi.

## 13. Implikasi untuk pembuat konten

**[Penerapan]**
- **Konten yang cocok topik tapi salah konteks tetap gagal.** Jawab persis yang ditanyakan (gitar, bukan piano; tahun yang diminta, bukan tahun lain).
- **Tulis dalam bahasa Indonesia untuk query berbahasa Indonesia**, termasuk query yang memakai nama diri atau istilah Inggris dalam huruf Latin (misalnya merek + "review", judul film, nama tokoh). Istilah teknis, perintah, kode, nomor part, dan spesifikasi boleh dibiarkan dalam bahasa Inggris; itulah yang dicari pengguna.
- **Bahasa daerah dan campuran:** untuk audiens Indonesia, bahasa Indonesia adalah default yang paling aman. Jika menargetkan pembaca berbahasa daerah tertentu, sesuaikan dengan kebutuhan pembacanya.
- **Halaman produk dan kategori:** dukung browsing dan riset (filter, foto dari berbagai sudut, spesifikasi, perbandingan, review), bukan hanya tombol beli.
- **Halaman kategori luas** (misalnya "hotel di Bali", "kafe di Jakarta Selatan"): tampilkan contoh yang populer dan menonjol, bukan satu tempat yang terlalu spesifik.
- **Konten lokal:** angka yang berbeda per wilayah (UMR/UMP, tarif, aturan daerah) harus spesifik per wilayah, akurat, dan merujuk sumber resmi daerah itu.
- **Freshness:** konten tentang acara berulang (pemilu, ujian masuk PTN, pendaftaran CPNS, jadwal libur), harga, dan model produk wajib diperbarui. Untuk topik medis, perbarui sesuai pedoman terbaru; konten medis yang usang bisa berbahaya.
- **Halaman error dan "stok habis":** sediakan navigasi, pencarian, dan alternatif. Halaman error yang membantu tetap bisa bernilai.
- **Artikel definisi:** hanya layak dibuat jika istilahnya memang dicari artinya. Untuk kata umum, intent-nya biasanya lain (tempat, produk, gambar).
- **Brand sendiri:** pastikan ada halaman yang memenuhi kedua intent (info lokasi/cabang dan layanan online), dan pantau review serta reputasi brand yang muncul untuk query nama domain.
