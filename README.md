# SEO Skills ID

Koleksi custom AI skills (Antigravity / Claude / Cursor) berbahasa Indonesia untuk riset konten SEO, penyusunan outline berbasis SERP, penulisan draf artikel berkualitas tinggi, optimasi metadata pencarian, dan audit kualitas konten berbasis standar Google.

## 📦 Daftar Skills

Repository ini terdiri dari empat skill modular yang dapat digunakan secara independen maupun sebagai satu alur kerja terpadu (*SEO pipeline*):

```text
                 4. sqrg-seo-foundation  ──> Standar kualitas (SQRG + Spam Policies)
                         ┆ dipakai di setiap tahap & untuk audit
[Topik / Keyword / URL]  ┆
       │                 ┆
       ▼                 ┆
1. seo-content-outline  ──> Menghasilkan Cetak Biru (Blueprint / Brief / Sitasi per Poin)
       │
       ▼
2. seo-article-writer   ──> Menulis Naskah Artikel Lengkap (1.000+ kata, EEAT, Anti-Slop)
       │
       ▼
3. seo-meta-generator   ──> Menghasilkan Meta Title, Description, & Slug (Artikel & Landing Page)
```

---

### 1. `seo-content-outline`
Skill untuk meriset topik atau keyword SEO lalu menyusun outline artikel yang siap dieksekusi penulis:
* **Fokus Riset:** Identifikasi search intent (dominan & sekunder), penentuan angle unik, pemetaan keyword, dan penanganan kanibalisasi topik (cluster vs pillar).
* **Cetak Biru Informatif:** Struktur heading H1–H4 yang jelas, mandiri, dan tidak kaku.
* **Sitasi Inline:** Setiap poin pembahasan langsung dilengkapi referensi `[situs](URL)` atau penanda `[Verifikasi]`.
* **Universal (Multi-Niche):** Mendukung topik umum, gaya hidup, bisnis, teknologi, otomotif, hingga topik sensitif/medis (YMYL).

### 2. `seo-article-writer`
Skill untuk mengeksekusi penulisan naskah artikel SEO lengkap berbasis brief atau outline:
* **Editorial Standards & Anti-Slop:** Bebas dari klise robotik AI (*"Di era modern saat ini"*, *"tidak hanya X tapi juga Y"*, *"Artikel ini membedah…"*), dengan ritme paragraf yang bervariasi dan prinsip *claim calibration*.
* **Output Siap Pakai di Mana Saja:** Format disesuaikan dengan tujuan, yaitu Markdown siap salin di chat (Claude/ChatGPT), Google Docs lewat connector (Claude Cowork) atau Google Workspace API (Hermes agent, script), file .docx, atau teks polos. Hasilnya berupa list asli (tanpa bullet ganda), tabel meta asli, heading asli, tanpa paragraf kosong, dan selalu diperiksa ulang setelah ditulis.
* **YMYL Claim Gate:** Untuk topik kesehatan, obat, tindakan klinik, keuangan, dan hukum, artikel wajib memuat status regulasi (BPOM/Kemenkes), sumber per klaim, kecocokan rute pemberian, risiko serius, serta Catatan Editor untuk review dokter.
* **Terintegrasi:** Mengikuti struktur heading outline dan menghormati penanda `[Verifikasi]`, `[Review medis]`, dan `[Pengalaman]` dari `seo-content-outline`.

### 3. `seo-meta-generator`
Skill khusus untuk membuat Meta Title (Title Tag), Meta Description, dan URL Slug yang optimal, memikat (High-CTR), dan mematuhi batasan Google SERP:
* **Multi-Page Type Support:** Mendukung artikel blog, landing page layanan/klinik, halaman produk e-commerce, homepage, dan local SEO.
* **3 Varian A/B Testing:** Menyajikan varian *Direct & Solutif*, *High CTR / Curiosity Hook*, dan *Authoritative / Kredibilitas*.
* **Batasan Karakter Ketat:** Title 45–60 karakter (aman di mobile), Description 130–155 karakter (lead with value + CTA), dan Slug kebab-case ringkas.
* **Standar Industri:** Menggabungkan pedoman resmi Google Search Central dan formula copywriting Edition Group.

### 4. `sqrg-seo-foundation`
Basis pengetahuan dan alat audit kualitas konten berdasarkan dua dokumen Google, ditulis ulang dengan bahasa sendiri dalam dua bahasa (`references/id/` dan `references/en/`):
* **Search Quality Rater Guidelines (edisi 11 Sep 2025):** Page Quality, E-E-A-T, YMYL, kriteria Lowest sampai Highest, konten AI dan produksi massal, search intent, dan skala Needs Met, lengkap dengan rujukan bagian dan halaman PDF.
* **Spam Policies Google Search (diperbarui 28 Agu 2026):** cloaking, doorway, sneaky redirect, teks tersembunyi, link spam, scaled content abuse, thin affiliation, site reputation policy (termasuk perubahan EEA), dan praktik lain yang memicu demotion.
* **Checklist Audit Bertahap:** urutan cek ala rater (bahaya dan spam dulu, baru kualitas), plus template laporan audit.
* **Pendamping Pipeline:** dipakai sebagai standar kualitas saat membuat outline dan menulis artikel, serta untuk menjawab "kenapa halaman ini susah ranking" atau "aman nggak pakai AI untuk artikel kesehatan".

---

## 🚀 Cara Pemasangan & Penggunaan

1. Clone repository ini ke direktori kerja Anda:
   ```bash
   git clone git@github.com:araaking/seo-skills-id.git
   ```
2. Pasang folder skill ke direktori custom skill AI assistant Anda (misalnya Antigravity, Claude Code, atau Cursor).
3. Panggil skill sesuai tahap pengerjaan:
   * Gunakan `seo-content-outline` saat memulai perencanaan topik/keyword.
   * Gunakan `seo-article-writer` dengan melampirkan hasil outline untuk memproduksi artikel utuh.
   * Gunakan `seo-meta-generator` untuk meracik metadata halaman (baik untuk artikel blog maupun landing page). Artikel dari `seo-article-writer` sudah memuat tabel meta; pakai skill ini bila butuh 3 varian A/B atau metadata untuk halaman non-artikel.
   * Gunakan `sqrg-seo-foundation` untuk mengaudit artikel/halaman/situs, mengecek E-E-A-T dan YMYL, atau sebagai standar kualitas di tahap mana pun.

---

## 📄 Lisensi
MIT License. Bebas digunakan, dimodifikasi, dan dikembangkan untuk kebutuhan editorial maupun agensi.
