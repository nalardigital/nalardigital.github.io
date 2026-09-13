# Checklist SEO On-Page — Nalar Digital

Dipakai setiap kali menulis/mempublikasikan artikel baru di blog ini (manual maupun oleh Claude). Terakhir diperbarui: 14 September 2026.

## 1. Front Matter (Wajib Diisi Lengkap)

- [ ] `title` — mengandung keyword utama, idealnya di bawah 60 karakter (supaya tidak terpotong di hasil pencarian Google)
- [ ] `date` — **cek waktu saat ini dulu sebelum menulis tanggal** (jangan future-dated, Hugo akan menyembunyikannya — pernah terjadi di blog ini)
- [ ] `categories` — sesuai salah satu dari 5 pilar (AI Tools & Engineering, Tutorial & Implementasi Teknis, Tren & Analisis Industri AI, Karier & Bisnis di Era AI, Etika/Regulasi & Masa Depan AI)
- [ ] `tags` — 3-6 tag spesifik, termasuk keyword long-tail yang relevan
- [ ] `summary` — 150-160 karakter, ini yang jadi meta description di hasil pencarian Google. Harus menarik untuk diklik, bukan sekadar ringkasan generik
- [ ] `cover.image` + `cover.alt` — gambar sampul dengan alt text deskriptif (bukan cuma "gambar artikel")

## 2. Judul & Slug

- [ ] Keyword utama muncul di judul, idealnya mendekati awal kalimat
- [ ] Slug URL (nama file) pendek, huruf kecil, pisah dengan tanda hubung, mengandung keyword (contoh: `panduan-membangun-rag-langchain.md`, bukan `artikel-baru-2.md`)

## 3. Struktur Konten

- [ ] Ada **satu** H1 (otomatis dari title, jangan tambah H1 manual di body)
- [ ] Body pakai H2 untuk seksi utama, H3 untuk sub-seksi — hierarki tidak boleh loncat (H2 langsung ke H4)
- [ ] Paragraf pembuka (100 kata pertama) sudah menyebutkan keyword utama dan inti topik — jangan bertele-tele sebelum masuk substansi
- [ ] Panjang konten proporsional dengan kedalaman topik: cluster ringan 800-1200 kata, tutorial/pilar 1500-3000 kata (jangan dipanjang-panjangkan tanpa isi, jangan dipendekkan sampai dangkal)

## 4. Internal Linking (Wajib untuk Setiap Artikel Baru)

- [ ] Link ke minimal 1 artikel pilar terkait (model pillar-cluster)
- [ ] Kalau artikel baru adalah pilar, sebutkan bahwa akan ada cluster artikel terkait (tanpa link mati ke artikel yang belum ada)
- [ ] Kalau relevan, link ke artikel cluster lain yang sudah ada (bukan cuma satu arah ke pilar)
- [ ] Gunakan anchor text deskriptif, bukan "klik di sini"

## 5. E-E-A-T (Kualitas & Kepercayaan)

- [ ] Ada contoh konkret, kode nyata, atau kasus spesifik — bukan generalisasi kosong
- [ ] Klaim data/statistik disertai konteks sumber, atau dihindari kalau tidak bisa diverifikasi (jangan mengarang angka spesifik demi terlihat meyakinkan)
- [ ] Kalau membahas isu yang masih diperdebatkan (etika, regulasi, prediksi masa depan), akui ketidakpastiannya secara eksplisit
- [ ] Tulisan menunjukkan pemahaman nyata terhadap topik, bukan sekadar rewrite permukaan

## 6. Search Intent

- [ ] Sebelum menulis, tentukan intent: informational (jelaskan konsep), transactional (bandingkan/rekomendasi), atau navigational
- [ ] Format artikel cocok dengan intent (tabel perbandingan untuk transactional, penjelasan bertahap untuk informational)

## 7. Sebelum Publish — Verifikasi Teknis

- [ ] Build lokal dulu (`hugo --gc --minify`) untuk memastikan tidak ada error dan artikel benar-benar muncul di halaman list
- [ ] Cek tidak ada broken internal link
- [ ] Setelah live, submit URL ke Google Search Console via "Request Indexing" (mempercepat crawl)

## Yang TIDAK Perlu Dikhawatirkan Berlebihan

- Keyword density/pengulangan kata kunci paksa — Google sudah lama tidak pakai metrik ini, fokus ke bahasa natural
- Panjang artikel demi angka kata tertentu — kualitas dan kelengkapan lebih penting dari jumlah kata
- Menjamin "halaman 1" — tidak ada yang bisa menjamin ini; fokus ke konsistensi dan kualitas jangka panjang, terutama karena domain masih baru (masa Google Sandbox beberapa bulan pertama adalah wajar)
