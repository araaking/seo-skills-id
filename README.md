# SEO Skills ID

Koleksi custom AI skills (Antigravity / Claude / Cursor) berbahasa Indonesia untuk riset konten SEO, penyusunan outline berbasis SERP, dan penulisan draf artikel berkualitas tinggi.

## 📦 Daftar Skills

Repository ini terdiri dari dua skill utama yang bekerja sebagai satu alur kerja (*pipeline*):

```text
[Topik / Keyword] 
       │
       ▼
1. seo-content-outline  ──> Menghasilkan Cetak Biru (Blueprint / Brief / Sitasi per Poin)
       │
       ▼
2. seo-article-writer   ──> Menulis Naskah Artikel Lengkap (1.000+ kata, EEAT, format rapi)
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
* **Editorial Standards:** Bebas dari klise robotik AI, menerapkan prinsip *claim calibration* dan anti-slop.
* **Format Bersih & Rapi:** Paragraf bernapas (2–3 kalimat per paragraf), single line-break (`\n`) untuk Google Docs/Word, dan simbol bullet unicode bulat (`• `).
* **Meta Information:** Tabel siap pakai berisi Title Tag, Meta Description, dan URL Slug.

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

---

## 📄 Lisensi
MIT License. Bebas digunakan, dimodifikasi, dan dikembangkan untuk kebutuhan editorial maupun agensi.
