# Google Generative AI Search & Content Guidelines (AI Overviews, RAG, & Non-Commodity Standards)

Panduan editorial wajib untuk skill `seo-article-writer`, disarikan langsung dari dokumentasi resmi **Google Search Central**:
1. *Optimizing your website for generative AI features on Google Search*
2. *Google Search's guidance on using generative AI content on your website*
3. *Search Quality Rater Guidelines (Section 4.6.5 & 4.6.6)*

---

## 1. Bagaimana Generative AI Search Google Bekerja

Fitur AI pada Google Search (seperti **AI Overviews** dan **AI Mode**) berakar langsung pada sistem perankingan dan penilaian kualitas inti (*core Search ranking systems*). Google menggunakan dua mekanisme utama:

* **Retrieval-Augmented Generation (RAG) & Grounding:**  
  Sistem Google mencari (*retrieve*) halaman web yang paling relevan, segar, dan berbobot dari indeks pencarian. Model AI kemudian meninjau informasi faktual dari halaman-halaman tersebut untuk menyusun rangkuman jawaban, lalu **menampilkan tautan sumber yang dapat diklik (*grounded citation*)**.
* **Query Fan-Out:**  
  Model AI menghasilkan sekumpulan kueri turunan secara serentak untuk menjawab berbagai sudut pandang topik secara tuntas (misal: mencari penyebab, cara pencegahan, dan alternatif solusi sekaligus).

---

## 2. Prinsip Non-Commodity Content (Anti-Konten Pasaran)

Google secara tegas membedakan antara konten komoditas murahan dengan konten bernilai tinggi:

### A. Commodity Content (Hindari Total)
Konten komoditas adalah artikel yang hanya memuat **pengetahuan umum dangkal yang bisa ditulis oleh siapa saja atau dihasilkan instan oleh AI gratisan** (contoh klise: artikel rangkuman umum tanpa sudut pandang baru). Konten seperti ini diklasifikasikan berbobot rendah dan tidak akan diprioritaskan oleh sistem RAG Google.

### B. Non-Commodity Content (Wajib Diterapkan)
Konten non-komoditas memberikan nilai tambah nyata (*value-add*) yang melampaui pengetahuan umum:
1. **Sudut Pandang Unik (*Unique Point of View*):** Menyajikan perspektif yang khas, tidak sekadar mengulang apa yang sudah ada di internet.
2. **Konteks & Contoh Situasi Nyata:** Menjelaskan alasan di balik suatu fenomena, bukan sekadar menyebutkan daftarnya.
3. **Perspektif Keahlian & Bukti:** Menyertakan penjelasan mekanisme mendalam (biologis, teknis, atau hukum) yang kredibel.
4. **Kerapian Visual & Semantik:** Menggunakan heading yang logis, paragraf bernapas, tabel perbandingan, dan daftar berbutir yang mudah dicerna manusia maupun mesin perayap.

---

## 3. RAG-Ready Architecture (Siap Dikutip AI Overviews)

Agar potongan teks (*passage*) artikel dipilih oleh algoritma RAG Google dan dijadikan sumber kutipan di AI Overviews:

* **Direct Answer di Awal Section (Passage-Level Clarity):**  
  Pada 1–2 kalimat pertama di bawah setiap H2, **langsung berikan jawaban tegas, padat, dan faktual** terhadap pertanyaan/topik heading tersebut. Jangan menunda jawaban di paragraf ketiga atau menyembunyikannya di balik basa-basi.
* **Kalimat Faktual yang Mandiri (*Stand-Alone Sentences*):**  
  Tulis kalimat penjelasan yang kaya fakta dan tidak ambigu, sehingga jika sistem AI Google mengambil 1 paragraf tersebut, maknanya tetap utuh dan jelas tanpa terpotong konteks.
* **Cakup Query Fan-Out secara Wajar:**  
  Bahas aspek-aspek penting yang relevan (seperti pencegahan, batas aman, kelompok rentan, perbandingan) tanpa memaksakan kata kunci yang berulang-ulang (*keyword stuffing*).

---

## 4. Standar Kualitas Rater (Section 4.6.5 & 4.6.6) & Anti-Halusinasi

Google Search Quality Raters mengevaluasi konten berdasarkan pedoman ketat:

1. **Anti-Scaled Content Abuse (Section 4.6.5):**  
   Memproduksi banyak artikel dengan bantuan otomatisasi tanpa memberikan nilai guna nyata (*little to no added value*) dianggap sebagai pelanggaran kebijakan spam. Setiap artikel wajib berbobot dan dirancang untuk kepuasan pembaca manusia (*people-first content*).
2. **Anti-Effortless Content (Section 4.6.6):**  
   Artikel yang dibuat dengan sedikit usaha (*little to no effort*) dan minim orisinalitas akan dinilai berpangkat rendah (*lowest quality*). Tulisan harus menunjukkan keseriusan riset dan kedalaman materi.
3. **Nol Halusinasi (*Zero Hallucination Rule*):**  
   Google menegaskan: *"Generative models don't retrieve facts, but predict a likely sequence of words."* Penulis AI wajib memverifikasi fakta. **DILARANG KERAS** mengarang angka statistik, nama studi fiktif, kutipan dokter rekaan, atau URL palsu.

---

## 5. Mitos yang Harus Diabaikan (Mythbusting AEO & GEO)

Google menegaskan bahwa trik-trik berikut **TIDAK PERLU** dan tidak membantu peringkat di Google Search:
* ❌ Tidak perlu memecah teks menjadi potongan kecil artifisial (*chunking* kaku).
* ❌ Tidak perlu membuat file khusus mesin seperti `llms.txt` (Google Search mengabaikannya).
* ❌ Tidak perlu menulis teks dengan gaya bahasa kaku yang ditujukan khusus untuk bot AI. Tulis untuk kenyamanan manusia.
* ❌ Tidak perlu mengejar sebutan (*inauthentic mentions*) palsu di web.

---

## 6. Checklist Kepatuhan Google GenAI

Sebelum artikel diserahkan:
- [ ] Apakah setiap H2 langsung memberikan jawaban faktual di awal paragraf (siap dikutip RAG)?
- [ ] Apakah artikel ini menyajikan *insight* mendalam (non-commodity), bukan sekadar rangkuman dangkal?
- [ ] Apakah semua klaim penting didasarkan pada data/sumber nyata tanpa ada halusinasi data?
- [ ] Apakah artikel terasa bermanfaat, memuaskan pembaca, dan terbebas dari kesan *effortless content*?
