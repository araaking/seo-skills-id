---
name: seo-meta-generator
description: Buat Meta Title (Title Tag), Meta Description, dan URL Slug yang optimal, memikat (High-CTR), dan mematuhi standar Google SERP. Mendukung artikel blog, landing page layanan/klinik, halaman produk e-commerce, homepage, dan local SEO. Menyajikan 3 varian sudut pandang (Direct, High CTR, Otoritatif) lengkap dengan penghitungan karakter dan rekomendasi varian terbaik. English triggers - meta tag generator, title tag generator, meta description, SEO snippet optimizer, slug generator.
---

# SEO Meta Generator

Ubah topik, kata kunci, draf artikel, atau rincian landing page menjadi paket metadata SEO siap pakai: **Meta Title (Title Tag)**, **Meta Description**, dan **URL Slug**.

Skill ini menerapkan prinsip resmi dari **Google Search Central** (anti-keyword stuffing, akurasi ringkasan, pencegahan Google rewriting) dan formula copywriting **Edition Group** (mobile-first character limits, front-loading keyword, dan CTR psychological triggers).

**Sebelum menyusun metadata, baca panduan teknis dan formula per tipe halaman di [references/meta-best-practices.md](references/meta-best-practices.md).**

---

## Batasan Karakter Keras (Strict Limits)

| Parameter | Batas Aman | Alasan Teknis |
|---|---|---|
| **Meta Title** | **45–60 karakter** | Mencegah pemotongan judul (`...`) di Google SERP desktop (600px) dan terutama layar seluler/mobile (45–55 karakter). |
| **Meta Description** | **130–155 karakter** | Memastikan pesan manfaat dan kalimat ajakan bertindak (CTA) terbaca utuh tanpa terpotong elipsis di perangkat mana pun. |
| **URL Slug** | **3–5 kata kunci** | Format *kebab-case* (huruf kecil dipisah tanda hubung `-`), ringkas, dan membuang kata sambung tak penting. |

---

## Alur Kerja & Deteksi Tipe Halaman

Skill ini secara otomatis mengidentifikasi intensi pencarian berdasarkan jenis halaman yang diminta:

1. **Artikel Blog / Edukasi (Informational):**
   * *Fokus:* Menjawab rasa penasaran pembaca, penjelasan langkah, atau cek fakta.
   * *CTA:* "Simak ulasannya!", "Baca panduan lengkapnya di sini!", "Cek faktanya!".
2. **Landing Page Layanan / Klinik / Bisnis (Commercial & Service):**
   * *Fokus:* Menawarkan solusi, menonjolkan kredibilitas dokter/ahli/legalitas, dan mendorong booking/konsultasi.
   * *CTA:* "Konsultasi sekarang!", "Booking jadwalmu hari ini!", "Hubungi tim ahli kami!".
3. **Produk E-commerce / Katalog (Transactional):**
   * *Fokus:* Keaslian produk, izin BPOM/garansi, spesifikasi penting, dan promo gratis ongkir.
   * *CTA:* "Beli sekarang!", "Dapatkan promo hari ini!", "Pesan di sini!".
4. **Homepage / Brand (Navigational):**
   * *Fokus:* Posisi payung bisnis dan keunggulan utama perusahaan.
   * *CTA:* "Kunjungi situs resmi!", "Pelajari profil kami!".
5. **SEO Lokal / Cabang (Local Intent):**
   * *Fokus:* Layanan spesifik di kota atau daerah tertentu.
   * *CTA:* "Cek lokasi terdekat!", "Jadwalkan kunjungan!".

---

## Kerangka 3 Varian Output (A/B Testing)

Untuk setiap permintaan, sajikan **3 varian sudut pandang** yang berbeda agar pengguna memiliki pilihan strategi:

* **Varian 1: Direct & Solutif (Straightforward)**
  * Menembak kata kunci dan jawaban/solusi secara tegas tanpa berbelit-belit. Sangat disukai algoritma Google dan pencari yang butuh informasi instan.
* **Varian 2: High CTR / Hook Penasaran (Humanis & Memikat)**
  * Menggunakan sudut pandang keresahan nyata, rasa ingin tahu alami (*curiosity gap*), atau penegasan solutif tanpa menggunakan *clickbait* palsu.
* **Varian 3: Authoritative / Kredibilitas (Otoritatif & Brand)**
  * Menonjolkan rujukan medis/ahli, keamanan berizin resmi (BPOM/Kemenkes/OJK), atau reputasi brand.

---

## Aturan Editorial & Anti-Slop pada Metadata

1. **Lead with Value:** Buka Meta Description langsung dengan hal yang paling dipedulikan pencari (manfaat/jawaban nyata). DILARANG menggunakan pembuka klise seperti:
   * ❌ *"Dalam artikel ini kami membahas..."*
   * ❌ *"Apakah Anda sedang mencari informasi tentang..."*
   * ❌ *"Di era modern seperti sekarang ini..."*
2. **No Keyword Stuffing:** Jangan mengulang kata kunci lebih dari 2 kali atau membuat daftar koma-komaan.
3. **Front-Loading Alami:** Posisikan kata kunci sedekat mungkin ke awal Title Tag, tetapi tetap prioritaskan kenyamanan membaca manusia.
4. **Hitung Karakter Nyata:** Selalu cantumkan jumlah karakter riil di samping teks agar pengguna yakin bahwa batasan SERP dipatuhi.

---

## Format Output Standar

Sajikan output langsung tanpa basa-basi pengantar ("Halo", "Tentu, berikut...", dsb.):

```markdown
### 📋 Ringkasan Input & Intensi
* **Topik / Keyword:** [Kata kunci utama]
* **Tipe Halaman:** [Artikel Blog / Landing Page Layanan / Produk / Homepage]
* **Search Intent:** [Informasional / Komersial / Transaksional]
* **Brand Anchor:** [Nama Brand / Opsional]

---

### 🎯 3 Varian Metadata SEO

#### Varian 1: Direct & Solutif (Straightforward)
* **Meta Title:** [Judul langsung to the point] (`[XX] karakter`)
* **Meta Description:** [Deskripsi solusi padat + CTA] (`[XXX] karakter`)
* **Karakter:** Ringkas, tegas, cocok untuk pencari yang butuh kepastian cepat.

#### Varian 2: High CTR / Hook Penasaran (Memikat & Humanis)
* **Meta Title:** [Judul dengan hook memikat/cek fakta] (`[XX] karakter`)
* **Meta Description:** [Deskripsi menyentuh keresahan pembaca + CTA] (`[XXX] karakter`)
* **Karakter:** Memancing klik tinggi di SERP yang kompetitif tanpa clickbait murahan.

#### Varian 3: Authoritative / Kredibilitas (Otoritatif & Brand)
* **Meta Title:** [Judul menonjolkan bukti/dokter/standar resmi] (`[XX] karakter`)
* **Meta Description:** [Deskripsi berbasis rujukan ahli/legalitas + CTA] (`[XXX] karakter`)
* **Karakter:** Menonjolkan kepercayaan tinggi (*trust signal*), sangat direkomendasikan untuk topik YMYL/layanan berbayar.

---

### 🔗 Rekomendasi URL Slug
* `slug-ramah-seo-ringkas`

### 💡 Rekomendasi Penggunaan
[Sebutkan varian nomor berapa yang paling direkomendasikan untuk intent topik ini beserta alasan singkatnya, serta tabel format ringkas siap copy-paste ke CMS.]

| Parameter | Konten Terpilih |
|---|---|
| **Title** | [Varian Terpilih] |
| **Description** | [Varian Terpilih] |
| **Slug** | [Slug Terpilih] |
```
