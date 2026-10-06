# SEO Skills ID

Koleksi custom AI skills (Antigravity / Claude / Cursor) berbahasa Indonesia untuk riset konten SEO, penyusunan outline berbasis SERP, penulisan draf artikel berkualitas tinggi, dan optimasi metadata pencarian.

## 📦 Daftar Skills

Repository ini terdiri dari tiga skill modular yang dapat digunakan secara independen maupun sebagai satu alur kerja terpadu (*SEO pipeline*):

```text
[Topik / Keyword / URL] 
       │
       ▼
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
* **Editorial Standards & Anti-Slop:** Bebas dari klise robotik AI (*"Di era modern saat ini"*, *"tidak hanya X tapi juga Y"*), menerapkan prinsip *claim calibration* dan gaya penulisan bernapas (2–3 kalimat per paragraf).
* **Format Bersih & Rapi:** Single line-break (`\n`) untuk Google Docs/Word, simbol bullet unicode bulat (`• `), dan tanpa H1 dobel di badan teks.
* **Terintegrasi:** Mendukung hierarki H2–H4 dan instruksi khusus dari outline.

### 3. `seo-meta-generator`
Skill khusus untuk membuat Meta Title (Title Tag), Meta Description, dan URL Slug yang optimal, memikat (High-CTR), dan mematuhi batasan Google SERP:
* **Multi-Page Type Support:** Mendukung artikel blog, landing page layanan/klinik, halaman produk e-commerce, homepage, dan local SEO.
* **3 Varian A/B Testing:** Menyajikan varian *Direct & Solutif*, *High CTR / Curiosity Hook*, dan *Authoritative / Kredibilitas*.
* **Batasan Karakter Ketat:** Title 45–60 karakter (aman di mobile), Description 130–155 karakter (lead with value + CTA), dan Slug kebab-case ringkas.
* **Standar Industri:** Menggabungkan pedoman resmi Google Search Central dan formula copywriting Edition Group.

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
   * Gunakan `seo-meta-generator` untuk meracik metadata halaman (baik untuk artikel blog maupun landing page).

---

## 📄 Lisensi
MIT License. Bebas digunakan, dimodifikasi, dan dikembangkan untuk kebutuhan editorial maupun agensi.
