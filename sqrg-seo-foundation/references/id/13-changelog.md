# Changelog SQRG dan Konteks Terkait

> Bagian 1 diringkas dari Appendix 2 (hal. 182) SQRG 11 Sep 2025. Bagian 2 berasal dari sumber di luar SQRG dan diberi keterangan sumbernya.

## 1. Riwayat perubahan menurut PDF (dua tahun terakhir)

| Edisi | Ringkasan perubahan |
|---|---|
| **September 2025** (edisi yang dipakai skill ini) | Definisi YMYL diperbarui; contoh tambahan untuk memperjelas; perbaikan kecil (salah ketik, dll.) |
| **Januari 2025** | Bagian Lowest dan Low diselaraskan dengan Google Search Web Spam Policies, plus contoh ilustrasi (di sinilah expired domain abuse, site reputation abuse, scaled content abuse, dan definisi AI generatif masuk); panduan interpretasi dan intent minor untuk Needs Met diperluas; perbaikan kecil lain |
| **Februari 2024** | Ciri halaman tidak tepercaya diperbarui, plus contoh |
| **November 2023** | Definisi skala Needs Met disederhanakan dan diberi panduan jenis rating khusus; contoh dimodernisasi (platform populer, format video); panduan forum diperluas |

Catatan: laporan media menyebut update Februari 2024 terbit pada awal Maret 2024; PDF mencatatnya sebagai Februari 2024.

## 2. Konteks di luar SQRG (cek ulang sebelum dipakai sebagai fakta)

- **Status versi (dicek Oktober 2026):** menurut laporan ppc.land (Oktober 2026), edisi yang di-host Google masih bertanggal 11 September 2025. Klaim tentang "revisi Juni 2026" yang beredar di sejumlah blog marketing tidak tercermin di dokumen yang dipublikasikan.
- **Kebijakan spam dan fitur AI Google:** laporan yang sama menyebut bahwa pada 15 Mei 2026 Google menyatakan kebijakan spamnya, termasuk scaled content abuse, berlaku juga untuk konten yang tampil di AI Overviews dan AI Mode. Ini pernyataan kebijakan Google, bukan bagian dari SQRG.
- **Halaman spam policies (dicek Oktober 2026):** halaman "Spam policies for Google web search" terakhir diperbarui 28 Agu 2026. Definisi spam kini mencakup upaya memanipulasi jawaban AI generatif di Search, dan site reputation policy diubah untuk EEA (halaman bisa dikategorikan terpisah dari domain utama alih-alih terkena manual action; manual action lama di EEA di bawah kebijakan ini dicabut). Dirangkum di `14-spam-policies.md`.
- **Frekuensi update:** Google biasanya memperbarui guideline ini kira-kira setahun sekali, kadang lebih sering.
- **Hubungan dengan ranking:** Google konsisten menyatakan rating dari rater tidak memengaruhi ranking secara langsung; rating dipakai untuk mengevaluasi sistem pencarian.

Jika pengguna bertanya soal versi terbaru dan web search tersedia, cari dulu sebelum menjawab.

## 3. Cara memperbarui skill saat edisi baru terbit

1. Unduh PDF terbaru dari situs resmi Google dan baca halaman changelog (Appendix 2) untuk melihat bagian yang berubah.
2. Bandingkan daftar isi lama dan baru; catat bagian yang bergeser nomor atau halaman.
3. Perbarui hanya file referensi yang terdampak (lihat peta di `00-index.md`), termasuk nomor halaman.
4. Perbarui tanggal edisi di `00-index.md`, `SKILL.md`, dan bagian 1 file ini.
5. Perbarui **kedua versi bahasa** (`references/id/` dan `references/en/`) pada file dan nomor bagian yang sama, supaya tetap setara.
6. Jika ada konsep baru yang penting, tambahkan juga ke `11-core-summary.md` dan `12-audit-checklist.md`.
7. `14-spam-policies.md` mengikuti sumbernya sendiri: cek ulang tanggal "last updated" halaman spam policies Search Central, lalu perbarui tanggal dan bagian yang berubah di kedua versi bahasa file `14`.
