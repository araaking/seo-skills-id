# Google Search, Konten AI, dan Fitur AI Search

Ringkasan pedoman resmi Google yang relevan untuk artikel buatan AI, dipisah tegas dari **heuristik internal tim**. Jangan menyebut heuristik internal sebagai "aturan Google".

Sumber resmi (dicek Oktober 2026):

1. *Optimizing your website for generative AI features on Google Search*: https://developers.google.com/search/docs/fundamentals/ai-optimization-guide (diperbarui 10 Juli 2026)
2. *Google Search's guidance on using generative AI content on your website*: https://developers.google.com/search/docs/fundamentals/using-gen-ai-content (diperbarui 1 Oktober 2026)
3. *AI features and your website*: https://developers.google.com/search/docs/appearance/ai-features
4. Blog Search Central, 21 Mei 2025, *Top ways to ensure your content performs well in Google's AI experiences on Search*: https://developers.google.com/search/blog/2025/05/succeeding-in-ai-search
5. *Search Quality Rater Guidelines* (versi 11 September 2025), bagian 3.4.1, 4.4, 4.6.5, 4.6.6, dan 5.2.2

---

## 1. Cara Kerja Fitur AI di Google Search (Resmi)

- AI Overviews dan AI Mode berakar pada sistem ranking dan kualitas inti Google Search.
- **Retrieval-augmented generation (RAG), disebut juga *grounding*:** sistem mengambil halaman relevan dari indeks, lalu model menyusun jawaban beserta tautan sumbernya.
- **Query fan-out:** model membuat sekumpulan kueri turunan secara bersamaan untuk menjawab berbagai sisi pertanyaan.
- Google menyatakan **tidak ada syarat tambahan atau optimasi khusus** agar halaman tampil di AI Overviews atau AI Mode. Halaman cukup memenuhi syarat untuk tampil di Search seperti biasa.

---

## 2. Konten Non-Komoditas (Resmi)

Google meminta konten yang **unik dan non-komoditas**, yaitu konten yang memberi wawasan yang tidak bisa didapat dari rangkuman ulang isi internet.

- **Inti versi Google adalah pengalaman dan keahlian langsung.** Ulasan tangan pertama memberi perspektif unik dari pengalaman pribadi, sedangkan rangkuman hanya mengulang informasi yang sudah ada. Google juga meminta agar konten tidak sekadar mendaur ulang apa yang sudah ditulis orang lain atau apa yang mudah dihasilkan model AI.
- **Wujudnya di artikel:** data internal, studi kasus, kutipan dokter atau praktisi yang nyata, foto atau proses sendiri, dan penjelasan alasan di balik sebuah fakta.
- **AI tidak punya pengalaman langsung.** Minta materinya ke user atau ambil dari outline (penanda `[Pengalaman]`). Jika belum ada, sisipkan slot `[isi: pengalaman/kutipan praktisi tentang …]` dan catat di Catatan Editor. **Dilarang mengarang** pengalaman, testimoni, atau kutipan.
- Struktur yang jelas (paragraf, section, dan heading yang logis) membantu pembaca manusia, dan itu yang disebut Google.
- Kedalaman disesuaikan dengan kategori topik. Artikel ringan tidak perlu penjelasan mekanisme ilmiah. Nilai tambahnya bisa berupa contoh praktis yang spesifik.

---

## 3. Review Manusia dan Akurasi (Resmi)

- Google menyatakan model generatif tidak mengambil fakta, melainkan memprediksi urutan kata yang mungkin berdasarkan data latihnya. Karena itu, **semua konten buatan AI harus dicek manual** soal akurasi dan kepercayaannya sebelum terbit. Pengecekan ini **termasuk metadata** seperti Title dan Meta Description.
- Konsekuensinya untuk skill ini:
  - AI dilarang mengarang angka, nama studi, kutipan, atau URL.
  - Setiap klaim penting yang belum bisa dicek ditandai `[Verifikasi: …]`.
  - Catatan Editor memuat daftar hal yang perlu dicek manusia, dan wajib ada untuk YMYL.
- Google juga menyarankan memberi konteks kepada pembaca tentang cara konten dibuat bila otomasi berperan besar. Keputusan pengungkapan ini ada di tangan tim editorial.

---

## 4. Search Quality Rater Guidelines (Rujukan, Bukan Faktor Ranking Langsung)

Penilaian rater dipakai Google untuk mengevaluasi sistemnya. Penilaian itu **tidak langsung memengaruhi ranking** sebuah halaman.

- **4.6.5 Scaled Content Abuse:** memproduksi banyak halaman dengan otomasi tanpa nilai tambah bagi pengunjung.
- **4.6.6:** konten utama yang dibuat dengan **sedikit usaha, sedikit orisinalitas, dan sedikit nilai tambah**, termasuk konten yang disalin, diparafrasekan, atau dihasilkan AI. Rater memberinya nilai *Lowest*. Bagian ini membahas usaha dan orisinalitas, **bukan akurasi**.
- **4.4 Harmfully Misleading Information:** ada standar akurasi yang sangat tinggi untuk topik YMYL yang jelas. Inilah rujukan akurasi untuk artikel kesehatan, keuangan, dan hukum.
- **3.4.1:** sebagian informasi dan saran YMYL harus berasal dari ahli. Pengalaman langsung bisa bernilai tinggi bila sejalan dengan konsensus ahli.
- **5.2.2 Filler:** isian yang menambah panjang tanpa menambah nilai membuat pengalaman pembaca buruk. Jangan memenuhi target kata dengan butir tambahan.

---

## 5. Hal yang Google Nyatakan Tidak Perlu (Resmi)

Dari dokumen resmi Google Search Central, bagian *Mythbusting generative AI search*:

- Membuat file `llms.txt`
- Memecah konten menjadi potongan kecil khusus untuk AI (*chunking*)
- Menulis ulang konten dengan gaya khusus untuk sistem AI
- Mengejar sebutan (*mentions*) yang tidak autentik
- Terlalu fokus pada *structured data*, yang tidak diwajibkan untuk fitur AI search

Google juga mengingatkan bahwa membuat halaman terpisah untuk tiap variasi kueri *fan-out* demi memanipulasi ranking atau jawaban AI termasuk **scaled content abuse**.

---

## 6. Heuristik Keterbacaan Tim (Bukan Pedoman Resmi Google)

Kebiasaan berikut dipakai karena memudahkan pembaca. Jangan diklaim sebagai syarat tampil di AI Overviews.

- **Jawaban langsung di awal bagian:** 1–2 kalimat pertama di bawah setiap H2 langsung menjawab heading. Untuk YMYL, jawabannya **terkalibrasi**, artinya menyebut status bukti bila buktinya terbatas ("belum ada uji klinis yang membuktikan…"), bukan tegas tanpa sumber.
- **Paragraf yang utuh maknanya:** setiap paragraf tetap jelas bila dibaca tersendiri, tanpa bergantung pada "hal tersebut di atas".
- **Cakupan subtopik yang wajar:** bahas subtopik yang benar-benar dibutuhkan pembaca dalam satu artikel. Jangan memecah setiap variasi kueri menjadi halaman terpisah.

---

## 7. Checklist

- [ ] Setiap H2 dibuka dengan jawaban langsung, dan untuk YMYL jawabannya terkalibrasi tanpa klaim tegas yang tidak bersumber.
- [ ] Ada nilai tambah non-komoditas (contoh spesifik, data, atau pengalaman), dan tidak ada pengalaman atau kutipan yang dikarang.
- [ ] Semua klaim penting bersumber atau ditandai `[Verifikasi]`, termasuk Title dan Description.
- [ ] Tidak ada butir pengisi demi target kata.
- [ ] Tidak ada heuristik internal yang disebut sebagai "aturan Google".
