# Distribusi Off-Page — Nalar Digital

Panduan cross-posting dan daftar komunitas untuk distribusi konten. Terakhir diperbarui: 14 September 2026.

## Cross-Posting ke Dev.to

File siap-pakai ada di `crosspost/devto/` (5 artikel pilar). Setiap file sudah punya front matter `canonical_url` yang menunjuk balik ke Nalar Digital — ini **wajib** diisi supaya Google tahu versi asli ada di blog Anda (menghindari masalah duplicate content, dan link balik itu sendiri berfungsi sebagai backlink).

**Langkah posting ke Dev.to:**
1. Login/daftar di https://dev.to (bisa pakai akun GitHub `nalardigital` atau akun personal Anda)
2. Klik **"Create Post"**
3. Klik ikon **"..."** di editor → **"Import from Markdown"** (atau paste manual)
4. Buka salah satu file di `crosspost/devto/`, copy seluruh isinya, paste ke editor Dev.to
5. Dev.to otomatis membaca front matter (title, tags, canonical_url, cover_image) — cek preview untuk memastikan ter-parse benar
6. Ubah `published: false` jadi `published: true` di editor sebelum publish, atau langsung klik **Publish** di UI
7. Ulangi untuk 4 file lainnya (beri jeda beberapa hari antar-posting, jangan sekaligus — terlihat lebih natural dan tidak seperti spam)

## Cross-Posting ke Hashnode

Hashnode tidak pakai front matter dalam artikel — canonical URL diisi lewat UI:
1. Login/daftar di https://hashnode.com
2. Buat blog personal (gratis, dapat subdomain `namaanda.hashnode.dev`)
3. Klik **"Write"**, paste isi artikel (tanpa bagian front matter `---...---`, cukup bagian body)
4. Klik **"Post settings"** di sidebar editor → isi field **"Canonical URL"** dengan link asli, contoh: `https://nalardigital.github.io/posts/panduan-memilih-ai-coding-assistant/`
5. Upload cover image yang sama (dari `assets/images/covers/`)
6. Publish

## Kenapa Canonical URL Penting

Tanpa canonical URL yang benar, Google bisa menganggap Dev.to/Hashnode sebagai "sumber asli" karena domain mereka lebih besar — artikel Anda sendiri malah kalah bersaing dengan salinannya sendiri. Dengan canonical URL terisi benar, SEO value tetap mengalir ke Nalar Digital, sementara Anda tetap dapat exposure ke pembaca baru di platform tersebut.

## Daftar Komunitas untuk Share Manual

Catatan jujur: saya tidak bisa memverifikasi status real-time komunitas di bawah (grup bisa berubah/nonaktif), jadi cek dulu keaktifannya sebelum posting. Selalu ikuti aturan masing-masing komunitas (banyak yang melarang self-promotion berlebihan — baca rules dulu, dan ikut diskusi organik, jangan cuma drop link).

**Platform global (bahasa Inggris, tapi audiens developer relevan):**
- Dev.to — tag `#discuss`, `#ai`, `#programming`
- Hashnode — komunitas developer, domain authority tinggi
- Reddit: r/artificial, r/MachineLearning, r/LocalLLaMA, r/programming (cek rules tiap subreddit soal self-promotion, biasanya dibatasi rasio konten sendiri vs partisipasi)
- Hacker News (Show HN) — untuk konten yang punya sudut pandang teknis kuat, kompetitif tapi traffic besar jika masuk depan

**Komunitas Indonesia (cek keaktifan sebelum join/posting):**
- Grup Facebook seputar "AI Indonesia", "Data Science Indonesia", "Developer Indonesia" — cari dengan kata kunci tersebut, pilih grup dengan member aktif tinggi
- Komunitas Telegram/Discord developer Indonesia (banyak bermunculan/berganti — cari lewat rekomendasi komunitas developer lokal seperti GDG/DevC chapter kota Anda)
- LinkedIn — posting dengan hashtag `#TeknologiIndonesia`, `#AIIndonesia`, `#DeveloperIndonesia`, dan ikut grup LinkedIn seputar tech Indonesia
- Kaskus — forum lama tapi subforum teknologi/programming masih ada aktivitas

**Strategi realistis:**
1. Mulai dari platform yang paling sesuai audiens (Dev.to untuk artikel teknis, LinkedIn untuk karier/bisnis)
2. Jangan posting ke semua sekaligus — sebar dalam beberapa minggu, sambil pantau mana yang menghasilkan traffic nyata (cek Google Analytics/Search Console)
3. Fokus ke komunitas yang benar-benar relevan dengan topik artikel spesifik, bukan broadcast ke semua tempat
