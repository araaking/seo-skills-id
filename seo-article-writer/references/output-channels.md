# Output Channels: Cara Menyajikan Artikel di Tiap Tujuan

Isi artikel sama di semua tujuan. Aturan kontennya ada di [house-style.md](house-style.md). File ini hanya mengatur **cara menyajikannya** di tiap channel: chat, Google Docs lewat connector, Google Docs lewat API, file .docx, atau teks polos.

Hampir semua kerusakan format terjadi karena cara satu channel dipakai di channel lain:

- Penanda `•` yang diketik masuk ke list asli Google Docs, sehingga tampil `● •` (bullet ganda).
- Tabel Markdown tidak pernah menjadi tabel di Docs, lalu diratakan menjadi baris "Title - …".
- Paragraf kosong yang disisipkan untuk memberi jarak menghasilkan celah raksasa.
- Satu Enter tanpa baris kosong di Markdown membuat paragraf menyatu.

---

## 1. Tentukan Channel Sebelum Menulis

| Situasi | Channel |
|---|---|
| Artikel ditulis sebagai jawaban di chat (Claude, ChatGPT, Gemini, dan sejenisnya) tanpa tool dokumen | **A. Chat, Markdown siap salin** (default) |
| Ada connector Google Drive/Google Docs (misalnya Claude Cowork atau claude.ai) dan user minta ditulis di Google Docs | **B. Google Docs lewat connector** |
| Agen atau script memanggil Google Workspace API sendiri (Hermes agent, n8n, Apps Script, Python) | **C. Google Docs lewat API** |
| User minta file Word atau .docx | **D. File .docx** |
| User secara eksplisit minta teks polos tanpa format | **E. Teks polos** |

Jika tidak ada tool dokumen dan user tidak menyebut tujuan, pakai **A**. Bertanya hanya jika user menyebut dua tujuan yang saling bertentangan.

---

## 2. Prinsip yang Berlaku di Semua Channel

1. **List adalah list asli.** Di Google Docs, HTML, dan .docx, jangan mengetik `•`, `●`, `-`, `*`, atau nomor sebagai teks di awal butir. Simbolnya dibuat oleh format list dokumen. Di Markdown, `- ` adalah sintaks list yang dirender menjadi list asli, jadi itu yang dipakai. Satu-satunya channel yang boleh mengetik `• ` adalah **E**.
2. **Tabel adalah tabel asli.** Ini berlaku untuk tabel meta maupun tabel di badan artikel. Tabel tidak boleh diratakan menjadi baris "Label - Isi".
3. **Jarak berasal dari pengaturan paragraf, bukan dari paragraf kosong.** Dokumen akhir tidak boleh berisi paragraf kosong, `<br>` berderet, atau `&nbsp;` sebagai pengganjal jarak. Di sumber Markdown, baris kosong antarblok justru wajib karena itulah pemisah paragraf. Baris kosong itu tidak menjadi paragraf kosong saat dirender.
4. **Heading memakai style heading asli** (Heading 2 atau Heading 3), bukan teks tebal yang diperbesar. Tidak ada H1 di badan artikel.
5. **Bold, italic, dan link memakai format asli channel.** Simbol `**`, `*`, `##`, atau `|` tidak boleh tampil mentah di Docs atau Word.
6. **Keluarkan artikelnya saja.** Jangan ada kalimat pengantar ("Berikut artikelnya…") atau penutup obrolan di dalam artikel atau dokumen.

---

## 3. Pemetaan Elemen per Channel

| Elemen | A. Markdown (chat) | B/C. Google Docs (impor HTML) | D. .docx |
|---|---|---|---|
| Label meta | `**Meta Information**` | `<p><b>Meta Information</b></p>` | Paragraf Normal, tebal |
| Tabel meta dan tabel isi | Tabel pipa, baris kosong sebelum dan sesudahnya | `<table>` dengan baris header tebal | Tabel asli, style Table Grid |
| H2 / H3 | `##` / `###` | `<h2>` / `<h3>` → HEADING_2 / HEADING_3 | Style Heading 2 / Heading 3 |
| Paragraf | Teks, lalu satu baris kosong | `<p>` | Paragraf Normal |
| List butir | `- Butir` | `<ul><li>Butir</li></ul>` | Style List Bullet atau numbering |
| List bernomor | `1. Langkah` | `<ol><li>Langkah</li></ol>` | Style List Number atau numbering |
| Istilah asing | `*istilah*` | `<i>istilah</i>` | Run italic |
| Link | `[teks](URL)` | `<a href="URL">teks</a>` | Hyperlink |
| Instruksi gambar dan caption | Dua paragraf terpisah | Dua `<p>` rata tengah | Dua paragraf rata tengah |
| Pemisah sebelum Catatan Editor | Baris kosong, `---`, baris kosong | `<hr>` (hapus bila hasil impornya jelek) | Garis atau page break |

---

## 4. Channel A: Chat (Markdown Siap Salin)

Tujuannya: user cukup menyalin jawaban lalu menempelkannya ke Google Docs, Word, atau editor CMS tanpa merapikan apa pun.

Aturan:

- Tulis **Markdown standar** (CommonMark/GFM). Beri tepat **satu baris kosong di antara setiap blok**: paragraf, heading, list, tabel, instruksi gambar, dan caption.
  - Dua baris teks yang hanya dipisah satu Enter dianggap **satu paragraf** dan akan menyatu.
  - Baris teks tepat di bawah tabel tanpa baris kosong ikut **menjadi baris tabel**.
  - Baris teks tepat di atas `---` berubah menjadi **heading besar** (setext heading).
- **Jangan membungkus artikel dalam code block** (```), karena hasil salinannya menjadi teks mentah.
- List memakai `- ` (atau `1. ` untuk langkah berurutan), **bukan** `•`.
- Heading tidak diberi bold tambahan (`## **Judul**` salah).
- Tidak ada teks apa pun sebelum `**Meta Information**` atau sesudah blok terakhir artikel. Catatan untuk editor masuk ke **Catatan Editor**, bukan ditulis di luar artikel.

Cara menempel (jelaskan ke user hanya bila ditanya):

1. Salin tampilan jawaban yang sudah dirender (blok teksnya lalu Ctrl+C, atau tombol salin di aplikasi chat), lalu tempel di Google Docs atau Word. Heading, list, dan tabel ikut menjadi format asli.
2. Jika yang tertempel masih berupa simbol (`##`, `|`, `**`), aktifkan **Tools > Preferences > Enable Markdown** di Google Docs, lalu klik kanan dan pilih **Paste from Markdown**.

---

## 5. Channel B: Google Docs lewat Connector (Claude Cowork / claude.ai)

**Muat skill `google-workspace` dan baca `references/docs.md`-nya sebelum panggilan connector pertama.** Aturan teknis di sana (list asli, heading style, tabel, `requiredRevisionId`, verifikasi) **mengalahkan** aturan format apa pun di skill ini bila bertentangan. Skill ini menentukan isi dan tampilan akhir, sedangkan `google-workspace` menentukan cara mengeksekusinya.

Langkah:

1. **Selesaikan naskah** sesuai house style sebelum menyentuh dokumen.
2. **Buat dokumen** dengan Drive `create_file`, `contentMimeType: "text/html"`, berisi HTML dari template di bagian 7. Nama file mengikuti Title meta.
3. **Baca ulang**: `read_doc`, lalu jalankan `docs_index.py outline` milik skill `google-workspace`.
4. **Perbaiki temuan** pemeriksaan di bagian 8, dalam satu batch per langkah, dimulai dari index tertinggi:
   - Tidak ada tabel: hapus paragraf "Label - Isi" hasil perataan, baca ulang, lalu sisipkan tabel dengan `docs_index.py new-table --at <endIndex-1 paragraf "Meta Information"> --data meta.json --revision <rev> --bold-header`.
   - Teks butir diawali `•`, `-`, atau `*`: hapus penanda teksnya. Bullet aslinya dipertahankan, atau dibuat dengan `createParagraphBullets` bila belum ada.
   - Paragraf kosong: hapus. Biarkan satu paragraf kosong yang ditolak Google untuk dihapus karena menempel pada tabel.
5. **Terapkan gaya** dalam satu batch setelah semua konten masuk:
   - `weightedFontFamily` Arial sekali untuk seluruh body.
   - Setiap paragraf NORMAL_TEXT: `spaceAbove` 0, `spaceBelow` 10 pt, `lineSpacing` 115, `alignment` JUSTIFIED.
   - Setiap HEADING_2: bold, 16 pt, hitam. Setiap HEADING_3: bold, 14 pt, hitam. Semua heading diberi `keepWithNext: true`.
   - Jangan me-reset bold pada heading.
6. **Baca ulang sekali lagi** dan jalankan pemeriksaan di bagian 8. Jika bisa menjalankan kode, ekspor ke PDF dan lihat hasil render halamannya.
7. **Balasan di chat**: satu atau dua kalimat beserta tautan dokumen. Artikel tidak ditempel ulang di chat.

Catatan untuk user (sampaikan sekali bila mereka mengeluhkan jarak heading):

- Jarak di atas heading berasal dari style Heading bawaan Google Docs, dan itu normal.
- Supaya H2/H3 otomatis sesuai house style tanpa langkah gaya, user bisa memformat satu heading, lalu memilih **Format > Paragraph styles > Heading 3 > Update 'Heading 3' to match**, kemudian **Options > Save as my default styles**.

---

## 6. Channel C: Google Docs lewat Google Workspace API (Hermes Agent, Script, Otomasi)

Hasil akhirnya sama dengan channel B. Bedanya hanya pada pemanggilan API langsung tanpa connector.

### Rute 1 (disarankan): impor HTML lewat Drive API, lalu rapikan dengan Docs API

```python
import io
from googleapiclient.http import MediaIoBaseUpload

media = MediaIoBaseUpload(io.BytesIO(html.encode("utf-8")), mimetype="text/html", resumable=False)
doc = drive.files().create(
    body={"name": title_meta, "mimeType": "application/vnd.google-apps.document", "parents": [folder_id]},
    media_body=media,
    fields="id",
).execute()
```

Setelah itu:

1. Panggil `documents.get` (dengan `includeTabsContent=True` bila dokumen memakai tab).
2. Jalankan pemeriksaan di bagian 8.
3. Perbaiki temuan dan terapkan gaya (sama dengan langkah 4–5 channel B) dengan `documents.batchUpdate` plus `writeControl.requiredRevisionId` dari pembacaan terakhir.

Drive juga bisa mengimpor `text/markdown` menjadi Google Docs, tetapi HTML lebih bisa dikendalikan, jadi pakai HTML.

### Rute 2: Docs API murni (bila upload tidak tersedia)

- `insertText` berisi seluruh teks dengan satu `\n` per paragraf. Tanpa penanda list dan tanpa baris kosong.
- `updateParagraphStyle` dengan `namedStyleType: "HEADING_2"` / `"HEADING_3"` dan `fields: "namedStyleType"` untuk setiap rentang heading.
- `createParagraphBullets` dengan `bulletPreset: "BULLET_DISC_CIRCLE_SQUARE"` untuk butir, atau `"NUMBERED_DECIMAL_ALPHA_ROMAN"` untuk langkah. Teks butirnya tanpa penanda.
- `insertTable` (`rows`, `columns`, `location.index = i`). Teks sel (r, c) disisipkan di index `i + 4 + r × (2C + 1) + 2c`. Isi dari sel terakhir ke sel pertama.
- `updateTextStyle` untuk italic istilah asing, bold label, dan link (`textStyle.link.url`).
- Index dihitung dalam satuan UTF-16. Urutkan request dari index tertinggi ke terendah, dan baca ulang dokumen setelah setiap batch.

### Pemeriksaan otomatis (Python)

```python
import re

PENANDA = re.compile(r"^\s*[•●▪◦\-\*–]\s")

def cek_dokumen(doc):
    """doc = hasil documents.get. Mengembalikan daftar masalah format."""
    body = doc["tabs"][0]["documentTab"]["body"] if "tabs" in doc else doc["body"]
    isi = body["content"]
    masalah = []
    if not any("table" in e for e in isi):
        masalah.append("Tidak ada tabel asli (tabel meta hilang atau diratakan)")
    for n, e in enumerate(isi):
        p = e.get("paragraph")
        if not p:
            continue
        teks = "".join(r.get("textRun", {}).get("content", "") for r in p.get("elements", []))
        gaya = p.get("paragraphStyle", {}).get("namedStyleType")
        dekat_tabel = any("table" in isi[k] for k in (n - 1, n + 1) if 0 <= k < len(isi))
        if not teks.strip() and not dekat_tabel and n != len(isi) - 1:
            masalah.append(f"Paragraf kosong di index {e['startIndex']}")
        if PENANDA.match(teks):
            masalah.append(f"Penanda list diketik sebagai teks: {teks[:40]!r}")
        if gaya == "HEADING_1":
            masalah.append(f"Ada H1 di badan: {teks[:40]!r}")
        if re.match(r"^\s*(Title|Description|Slug)\s+[-–]\s", teks):
            masalah.append(f"Baris meta diratakan, bukan tabel: {teks[:40]!r}")
    ada_link = any(
        r.get("textRun", {}).get("textStyle", {}).get("link")
        for e in isi if e.get("paragraph")
        for r in e["paragraph"].get("elements", [])
    )
    if not ada_link:
        masalah.append("Tidak ada link sama sekali: nama sumber di badan artikel belum ditautkan")
    return masalah
```

---

## 7. Template HTML (Channel B dan C)

Satu elemen per baris. Spasi dan baris baru di antara tag diabaikan saat impor. **Dilarang** memakai `<p></p>`, `<p><br></p>`, `<br>`, atau `&nbsp;` di antara blok, dan dilarang mengetik `•` di dalam `<li>`.

```html
<html><body>
<p style="font-family:Arial;font-size:11pt"><b>Meta Information</b></p>
<table style="border-collapse:collapse;width:100%">
<tr><td style="border:1px solid #000;padding:4pt"><b>Element</b></td><td style="border:1px solid #000;padding:4pt"><b>Content</b></td></tr>
<tr><td style="border:1px solid #000;padding:4pt">Title</td><td style="border:1px solid #000;padding:4pt">{Title}</td></tr>
<tr><td style="border:1px solid #000;padding:4pt">Description</td><td style="border:1px solid #000;padding:4pt">{Description}</td></tr>
<tr><td style="border:1px solid #000;padding:4pt">Slug</td><td style="border:1px solid #000;padding:4pt">{slug}</td></tr>
</table>
<p style="font-family:Arial;font-size:11pt;line-height:1.15;margin:0 0 10pt 0;text-align:justify">{Paragraf pendahuluan 1}</p>
<p style="font-family:Arial;font-size:11pt;line-height:1.15;margin:0 0 10pt 0;text-align:justify">{Paragraf pendahuluan 2}</p>
<h2 style="font-family:Arial;font-size:16pt;font-weight:bold;color:#000">{H2 dengan <i>istilah asing</i> bila ada}</h2>
<p style="font-family:Arial;font-size:11pt;line-height:1.15;margin:0 0 10pt 0;text-align:justify">{Jawaban langsung 1–2 kalimat}</p>
<p style="font-family:Arial;font-size:11pt;text-align:center">[Gambar: {instruksi visual}]</p>
<p style="font-family:Arial;font-size:11pt;text-align:center">{Caption} | Sumber: {Nama Situs}</p>
<h3 style="font-family:Arial;font-size:14pt;font-weight:bold;color:#000">{H3}</h3>
<p style="font-family:Arial;font-size:11pt;line-height:1.15;margin:0 0 10pt 0;text-align:justify">{Isi, diakhiri kalimat pengantar list:}</p>
<ul>
<li>{Butir tanpa simbol}</li>
<li>{Butir tanpa simbol}</li>
</ul>
<p style="font-family:Arial;font-size:11pt"><b>Baca Juga:</b> <a href="{URL}">{Judul Artikel}</a></p>
<h2 style="font-family:Arial;font-size:16pt;font-weight:bold;color:#000">Pertanyaan Seputar {Topik}</h2>
<h3 style="font-family:Arial;font-size:14pt;font-weight:bold;color:#000">{Pertanyaan}?</h3>
<p style="font-family:Arial;font-size:11pt;line-height:1.15;margin:0 0 10pt 0;text-align:justify">{Jawaban}</p>
<h2 style="font-family:Arial;font-size:16pt;font-weight:bold;color:#000">{H2 penutup}</h2>
<p style="font-family:Arial;font-size:11pt;line-height:1.15;margin:0 0 10pt 0;text-align:justify">{Isi}</p>
<p style="font-family:Arial;font-size:11pt"><b>Referensi:</b></p>
<ul>
<li><a href="{URL}">{Judul Asli Halaman}</a> | {Nama Situs}</li>
</ul>
<hr>
<p style="font-family:Arial;font-size:11pt"><b>Catatan Editor (tidak untuk dipublikasikan)</b></p>
<ul>
<li>{Hal yang perlu dicek editor}</li>
</ul>
</body></html>
```

---

## 8. Pemeriksaan Setelah Menulis (Channel B, C, D)

Baca ulang dokumen sungguhan. Tool yang menerima panggilan belum berarti hasilnya benar.

- [ ] Ada **tepat satu tabel meta** berukuran 4 baris × 2 kolom dengan header tebal, ditambah tabel isi yang memang direncanakan. Tidak ada baris "Title - …" hasil perataan.
- [ ] Label "Meta Information" dan "Referensi:" tebal.
- [ ] **Tidak ada teks butir yang diawali** `•`, `●`, `-`, `*`, atau `–`, dan setiap butir list punya bullet asli.
- [ ] **Tidak ada paragraf kosong**, kecuali satu yang menempel pada tabel atau di akhir dokumen bila Google menolak menghapusnya. Tidak pernah ada dua paragraf kosong berturut-turut.
- [ ] Tidak ada HEADING_1 di badan. Semua H2 memakai HEADING_2 dan semua H3 memakai HEADING_3, dan tidak ada heading palsu berupa teks tebal.
- [ ] H2/H3 tebal dan hitam, dan body memakai Arial 11 pt.
- [ ] Tidak ada simbol Markdown mentah (`**`, `##`, `|`, `[teks](url)`).
- [ ] Istilah asing tampil miring.
- [ ] Nama sumber di badan artikel (jurnal, media, regulator, dokter) berupa link yang bisa diklik dan menuju halaman spesifik, bukan beranda. Tidak ada nama sumber tanpa link kecuali placeholder `[isi: URL …]`.

---

## 9. Channel D: File .docx

- Di Claude, pakai skill `docx` bila tersedia. Di agen lain, pakai `python-docx` atau `docx` (JavaScript).
- Atur style sekali, jangan per paragraf. Spesifikasinya mengikuti bagian **Spesifikasi Tampilan** di house-style.md.
- List memakai style **List Bullet** atau **List Number**, atau numbering config. **Jangan** menulis `•` sebagai teks.
- Tabel meta memakai tabel asli 4 × 2 dengan style Table Grid dan baris header tebal.
- Tidak ada paragraf kosong untuk jarak, karena jarak datang dari `space_after` 10 pt.

```python
from docx import Document
from docx.shared import Pt

doc = Document()
doc.styles["Normal"].font.name = "Arial"
doc.styles["Normal"].font.size = Pt(11)
doc.styles["Normal"].paragraph_format.space_after = Pt(10)

doc.add_paragraph().add_run("Meta Information").bold = True
tabel = doc.add_table(rows=4, cols=2, style="Table Grid")
for r, (a, b) in enumerate([("Element", "Content"), ("Title", title), ("Description", desc), ("Slug", slug)]):
    tabel.cell(r, 0).text, tabel.cell(r, 1).text = a, b
doc.add_heading("Judul H2", level=2)
doc.add_paragraph("Isi paragraf.")
doc.add_paragraph("Butir list tanpa simbol", style="List Bullet")
doc.save(nama_file)
```

Setelah file disimpan, buka lagi dengan `python-docx`, lalu periksa nama style setiap paragraf dan cocokkan dengan daftar di bagian 8.

---

## 10. Channel E: Teks Polos

Hanya dipakai bila user memintanya secara eksplisit, misalnya untuk kolom CMS yang membuang semua format.

- Satu Enter antarparagraf, tanpa baris kosong.
- List boleh memakai `• ` yang diketik.
- Meta ditulis per baris: `Title: …`, `Description: …`, `Slug: …`.
- Heading ditulis sebagai baris biasa, tanpa simbol Markdown.
- Beri tahu user satu kali bahwa tabel dan heading tidak akan terformat otomatis di channel ini.

---

## 11. Gejala, Penyebab, dan Perbaikan

| Gejala | Penyebab | Perbaikan |
|---|---|---|
| Bullet ganda `● •` | Penanda diketik di dalam list asli | Hapus penanda teks, pertahankan bullet asli |
| Tabel meta tampil sebagai "Title - …" | Tabel diratakan atau impornya gagal | Buat tabel asli (`<table>`, `new-table`, `insertTable`) |
| Jarak raksasa di antara paragraf | Ada paragraf kosong, `<br>`, atau `&nbsp;` | Hapus paragraf kosong |
| H3 abu-abu dan tidak tebal | Style Heading 3 bawaan Google Docs | Jalankan langkah gaya di channel B atau ubah style Heading 3 |
| Simbol `##`, `**`, atau `\|` muncul di Docs | Markdown ditempel sebagai teks | Pakai Paste from Markdown, atau channel B/C |
| Paragraf pendahuluan masuk ke tabel (Markdown) | Tidak ada baris kosong setelah tabel | Tambahkan baris kosong |
| Referensi berubah menjadi heading besar (Markdown) | `---` ditulis tepat di bawah teks | Tambahkan baris kosong sebelum `---` |
| Paragraf menyatu (Markdown) | Blok dipisah satu Enter saja | Pisahkan blok dengan satu baris kosong |

---

## 12. Status Pengujian

- **Terverifikasi:**
  - Perilaku Markdown di bagian 4, dicek dengan spesifikasi GFM dan diuji dengan parser `marked`.
  - Drive mengonversi HTML dan Markdown menjadi Google Docs (developers.google.com/workspace/drive/api/guides/manage-uploads).
  - Tag `h1`, `h2`, `p`, `ul`, `ol`, `b`, `i`, dan `a` dikonversi menjadi format asli (skill `google-workspace`).
  - Google Docs punya fitur Paste from Markdown yang nonaktif secara default (support.google.com/docs/answer/12014036).
- **Belum dites di akun user:**
  - Apakah `<table>` di HTML selalu menjadi tabel asli.
  - CSS inline mana saja yang dipertahankan.
  - Apakah `<hr>` ikut terimpor.
  - Apakah Paste from Markdown ikut mengubah tabel.
  - Karena alur B dan C selalu ditutup dengan pemeriksaan dan perbaikan di bagian 8, artikel tetap rapi walaupun salah satu konversi itu gagal. Catat hasil tes di bagian ini begitu sudah dicoba.
