---
title: "Bias Algoritma dalam Praktik: Pelajaran dari Dua Kasus yang Terdokumentasi"
date: 2026-09-13T05:00:00+07:00
draft: false
categories: ["Etika, Regulasi & Masa Depan AI"]
tags: ["bias algoritma", "etika AI", "studi kasus", "tata kelola data"]
summary: "Dua kasus bias algoritma yang paling banyak dikutip dan terdokumentasi publik — apa yang sebenarnya terjadi, dan pelajaran konkret untuk tim yang membangun sistem berbasis AI."
cover:
  image: "images/covers/bias-algoritma-studi-kasus.png"
  alt: "Ilustrasi sampul: Bias Algoritma dalam Praktik: Pelajaran dari Dua Kasus yang Terdokumentasi"
  relative: false
---
Diskusi soal bias algoritma sering berhenti di level konsep abstrak. Artikel ini membahas dua kasus yang benar-benar terdokumentasi secara publik, untuk melengkapi pembahasan di [Etika dan Regulasi AI: Panduan Praktis](/posts/etika-regulasi-ai-panduan-praktis/), dengan fokus pada pelajaran konkret yang bisa diterapkan tim engineering.

## Kasus 1: Sistem Rekrutmen Otomatis yang Bias Gender

Sekitar tahun 2018, dilaporkan bahwa sebuah perusahaan teknologi besar menghentikan penggunaan internal sebuah sistem AI eksperimental untuk menyaring resume kandidat setelah ditemukan sistem tersebut secara sistematis memberi skor lebih rendah pada resume yang mengandung kata-kata terkait perempuan (misalnya nama organisasi seperti "women's chess club").

**Apa yang menyebabkannya:** sistem dilatih menggunakan data resume yang diterima perusahaan selama sekitar satu dekade sebelumnya, di mana mayoritas pelamar (terutama untuk posisi teknis) adalah laki-laki. Model belajar pola historis tersebut sebagai "sinyal kandidat yang baik" — bukan karena ada instruksi eksplisit untuk diskriminasi, tapi karena data training merefleksikan bias historis dalam proses rekrutmen industri secara luas.

**Pelajaran untuk tim engineering:**
- Data historis bukan "ground truth netral" — data merefleksikan keputusan manusia di masa lalu, termasuk bias yang ada di dalamnya.
- Menghapus atribut sensitif (seperti gender) dari data training tidak cukup — model bisa belajar proxy tidak langsung (nama organisasi, kata tertentu) yang berkorelasi dengan atribut tersebut.
- Audit performa model secara terpisah untuk subkelompok yang relevan adalah langkah wajib, bukan opsional, sebelum sistem dipakai untuk keputusan yang berdampak signifikan pada seseorang.

## Kasus 2: Algoritma Penilaian Risiko dalam Sistem Peradilan

Sebuah investigasi jurnalistik yang banyak dikutip menganalisis sebuah algoritma penilaian risiko residivisme (kemungkinan seseorang mengulangi tindak kriminal) yang dipakai di beberapa wilayah yurisdiksi Amerika Serikat. Investigasi tersebut menemukan disparitas: kelompok terdakwa dari ras tertentu lebih sering salah diklasifikasikan sebagai "berisiko tinggi" dibanding kelompok lain, meski pada akhirnya tidak mengulangi tindak kriminal.

Penting dicatat: temuan ini memicu perdebatan metodologis yang masih berlangsung di kalangan akademisi soal definisi "keadilan" (fairness) mana yang seharusnya dipakai — karena secara matematis, beberapa definisi fairness yang berbeda bisa saling bertentangan satu sama lain (tidak mungkin memenuhi semua definisi sekaligus). Namun konsensus umum yang bertahan dari kasus ini: sistem pengambilan keputusan berdampak tinggi butuh transparansi metodologi dan audit independen, bukan sekadar klaim akurasi dari pembuat sistem.

**Pelajaran untuk tim engineering:**
- Untuk sistem yang berdampak signifikan pada kehidupan seseorang, "akurat secara agregat" tidak cukup — disparitas antar kelompok harus diukur dan dilaporkan secara eksplisit.
- Definisi "adil" bukan pilihan teknis semata — melibatkan pilihan nilai yang idealnya melibatkan pemangku kepentingan di luar tim teknis.
- Transparansi metodologi ke pihak eksternal (bukan hanya klaim internal) penting untuk sistem yang berdampak signifikan pada publik.

## Pola yang Berulang di Kedua Kasus

Baik kasus rekrutmen maupun penilaian risiko menunjukkan pola yang sama: **bias tidak muncul karena niat jahat, tapi karena data historis dan definisi metrik yang tidak dipertanyakan secara kritis sejak awal.** Ini yang membuat bias algoritma sering lebih sulit dideteksi dibanding bias yang disengaja — sistemnya "bekerja sesuai desain", masalahnya ada di asumsi yang mendasari desain tersebut.

## Menerapkan Kerangka Audit dari Pilar Etika & Regulasi

Sesuai kerangka lima pertanyaan yang dibahas di artikel pilar, kedua kasus di atas menunjukkan pentingnya menjawab secara eksplisit di tahap desain: *siapa yang bisa dirugikan, kelompok mana yang kurang terwakili dalam data, dan siapa yang bertanggung jawab jika sistem salah* — bukan menunggu insiden publik untuk menyadarinya.

*Artikel ini melengkapi [Etika dan Regulasi AI: Panduan Praktis untuk Developer dan Perusahaan Teknologi](/posts/etika-regulasi-ai-panduan-praktis/) di seri Etika, Regulasi & Masa Depan AI.*
