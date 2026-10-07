# YMYL Claim Gate (Wajib untuk Kategori 4)

Berlaku untuk topik kesehatan, obat, suplemen, tindakan klinik atau estetika, keuangan, dan hukum. Tujuannya mencegah artikel YMYL terdengar meyakinkan padahal klaimnya tidak bersumber, buktinya berasal dari rute pemberian lain, atau status regulasinya disembunyikan.

Kasus nyata yang melatarbelakangi file ini: sebuah artikel *infus whitening* menulis "Kolagen menjaga kulit tetap kenyal" dan "Glutathione mendetoksifikasi tubuh" sebagai fakta. Artikel yang sama menutup risikonya dengan "efek samping serius jarang terjadi", tanpa sumber dan tanpa menyebut posisi BPOM.

---

## 1. Tingkat Sumber

| Tingkat | Contoh | Boleh dipakai untuk |
|---|---|---|
| **P1** | Regulator dan pemerintah (BPOM, Kemenkes, OJK, BI, peraturan resmi), pedoman perhimpunan profesi (IDI, PERDOSKI, AAD, ACOG), WHO, ulasan sistematis atau uji klinis di jurnal | Semua klaim, termasuk efektivitas, keamanan, dosis, dan status regulasi |
| **P2** | Situs rumah sakit, perhimpunan profesi, portal kesehatan yang ditinjau dokter, media nasional dengan dewan redaksi | Penjelasan umum dan prosedur. Untuk klaim keamanan dan efektivitas, utamakan P1 |
| **P3** | Situs klinik, penjual, *marketplace*, blog brand | Hanya sebagai **klaim pihak tersebut**, diatribusikan ("klinik X mempromosikan…"). Tidak boleh menjadi dasar klaim keamanan, efektivitas, atau dosis |

Tingkatan ini sama dengan Prioritas 1–3 di skill `seo-content-outline`.

---

## 2. Sepuluh Aturan Gerbang

1. **Status regulasi dulu.** Untuk obat, injeksi atau infus, suplemen, alat kesehatan, dan tindakan klinik, cari dan tulis status resminya **sebelum atau di dalam** pembahasan manfaat:
   - Apakah produk atau zatnya punya izin edar BPOM, dan untuk indikasi apa.
   - Apakah penggunaan untuk tujuan yang dibahas artikel termasuk *off-label*.
   - Tulis statusnya **secara kondisional sesuai sumber**. Contoh: BPOM menyatakan suntik putih yang beredar **tanpa izin edar** adalah produk ilegal. Jangan menggeneralisasi menjadi "semua infus whitening ilegal".
   - Urutan sumber: BPOM, Kemenkes, lalu IDI/perhimpunan spesialis. Regulator asing (FDA Filipina, FDA/CDC AS) hanya dipakai bila sumber Indonesia tidak membahas, dan negaranya disebut.
   - Tidak ketemu: tulis `[Verifikasi: status izin edar BPOM untuk X]` dan masukkan ke Catatan Editor.
2. **Satu klaim, satu sumber.** Klaim efektivitas, keamanan, efek samping, dosis, durasi, atau kontraindikasi wajib punya sumber P1 atau P2 yang tercantum di Referensi. Klaim tanpa sumber punya tiga pilihan: dihapus, ditulis beserta status buktinya ("belum ada uji klinis yang membuktikan…"), atau ditandai `[Verifikasi]`. Klaim tanpa sumber tidak boleh diubah menjadi kalimat fakta yang lugas.
3. **Rute harus cocok.** Bukti dari pemakaian oral, topikal, atau suntikan di kulit **tidak berlaku** untuk infus atau IV, dan sebaliknya. Jika rute yang dibahas belum punya bukti, katakan itu.
4. **Pisahkan tiga lapis klaim.**
   - (a) Klaim klinik atau produsen: atribusikan ("klinik mempromosikan…").
   - (b) Fungsi fisiologis umum suatu zat: boleh ditulis, dengan sumber.
   - (c) Bukti klinis untuk tujuan yang dibahas: sebut kekuatannya (belum ada uji, uji kecil, atau ulasan sistematis).
   - Jangan menjadikan (b) seolah-olah (c).
5. **Risiko serius wajib disebut, kalimat penenang dilarang.** Sebutkan risiko serius yang dinyatakan regulator beserta sumbernya, dengan tingkat keparahan aslinya. Dilarang menulis kalimat penenang tanpa data seperti "efek samping serius jarang terjadi" atau "aman bila dilakukan di klinik resmi".
6. **Jumlah butir tunduk pada bukti.** Jumlah H3 atau butir manfaat dan kandungan mengikuti jumlah klaim yang bersumber, bukan kuota outline atau target kata. Bila bukti hanya mendukung dua manfaat, tulis dua.
7. **Penanda dari outline tidak boleh hilang diam-diam.**
   - `[Verifikasi]`: cari sumbernya. Jika tidak ketemu, tulis versi terkalibrasi dan masukkan ke Catatan Editor.
   - `[Review medis]`: tulis section-nya dengan kalibrasi ketat, lalu tambahkan "Bagian <H2> perlu ditinjau tenaga medis" di Catatan Editor.
   - `[Pengalaman]`: jangan dikarang. Minta materinya ke user, atau biarkan sebagai `[isi: pengalaman/kutipan praktisi tentang …]` dan catat di Catatan Editor.
8. **Kutip regulatornya langsung.** Kutip pernyataan regulator itu sendiri. Jangan mengutip ulang daftar pustaka di dalam halamannya tanpa membuka sumber aslinya.
9. **Catatan Editor YMYL selalu ada.** Isinya: status regulasi yang ditemukan, daftar klaim `[Verifikasi]`, placeholder yang tersisa, "Cek ulang Title dan Description", dan "Perlu ditinjau dokter/apoteker sebelum terbit".
10. **Tanpa akses web:** jangan menulis klaim efektivitas atau keamanan sebagai fakta. Tulis versi terkalibrasi, tandai `[Verifikasi]`, dan sebutkan di Catatan Editor bahwa riset sumber belum dilakukan.

---

## 3. Nada untuk YMYL

Tenang, jelas, dan terkalibrasi, bukan "otoritatif" yang terdengar pasti. Paragraf pertama di bawah H2 tetap langsung menjawab heading, tetapi jawabannya menyebut status bukti bila buktinya terbatas.

- Jangan memberi diagnosis individual, dosis tanpa resep, atau janji hasil.
- Contoh konkret (kelompok rentan, kondisi, angka) pada YMYL **harus bersumber**. Jika tidak ada sumber, tulis bahwa datanya belum tersedia. Jangan mengarang contoh demi memenuhi aturan anti-kata-mengambang.

---

## 4. Contoh SALAH vs BENAR

**Rute tidak cocok**

- SALAH: "Kolagen menjaga kulit tetap kenyal, halus, dan terhidrasi."
- BENAR: "Sejumlah klinik mencantumkan kolagen dalam paket infus. Bukti manfaat kolagen untuk kulit sejauh ini berasal dari suplemen oral, bukan infus."

**Fungsi umum dijadikan bukti klinis**

- SALAH: "Glutathione membantu mendetoksifikasi tubuh dan mencerahkan kulit."
- BENAR: "Glutathione adalah antioksidan yang dibuat tubuh sendiri. Pemberiannya lewat infus untuk mencerahkan kulit belum didukung uji klinis yang memadai [Verifikasi: ulasan sistematis glutathione IV untuk pencerah kulit]."

**Kalimat penenang tanpa data**

- SALAH: "Efek samping serius jarang terjadi selama prosedur dilakukan oleh tenaga profesional."
- BENAR: "BPOM mencatat risiko serius dari suntik putih tanpa izin edar, antara lain reaksi alergi berat (anafilaksis), infeksi hingga sepsis, serta gangguan ginjal dan hati. Konsultasikan riwayat alergi dan penyakit ginjal ke dokter sebelum tindakan."

**Status regulasi digeneralisasi**

- SALAH: "Infus whitening dilarang BPOM."
- BENAR: "BPOM menyatakan suntik putih yang beredar tanpa izin edar adalah produk ilegal, dan klaim pemutih instan tidak diakui secara ilmiah."

---

## 5. Sumber Rujukan yang Sudah Dicek (Contoh Topik Suntik/Infus Putih)

- BPOM, "Suntik Putih: Ilusi Cantik Instan yang Mematikan": https://intelijen.pom.go.id/hot-issue/suntik-putih-ilusi-cantik-instan-yang-mematikan (halaman bertanggal 30 September 2025, dicek Oktober 2026; memuat pernyataan produk tanpa izin edar ilegal dan daftar risiko serius)
- FDA Filipina, Advisory No. 2019-182: https://www.fda.gov.ph/fda-advisory-no-2019-182-unsafe-use-of-glutathione-as-skin-lightening-agent/ (tidak ada produk injeksi yang disetujui untuk pencerah kulit)

Daftar ini hanya contoh. Untuk topik lain, cari ulang sumber P1 saat menulis dan jangan memakai sumber dari ingatan.
