---
title: "5 Prompt Berguna untuk Debugging Kode dengan AI"
date: 2026-09-13T06:00:00+07:00
draft: false
categories: ["AI Tools & Engineering"]
tags: ["debugging", "prompt engineering", "quick tips", "produktivitas developer"]
summary: "Lima pola prompt siap pakai untuk mempercepat proses debugging dengan AI assistant, lebih efektif daripada sekadar menempelkan pesan error dan bertanya 'kenapa ini error'."
---

Menempelkan pesan error lalu bertanya "kenapa ini error?" sering menghasilkan jawaban generik. Lima pola prompt berikut terbukti lebih efektif untuk debugging.

## 1. Minta Analisis Hipotesis, Bukan Langsung Solusi

```
Berikut error dan kode terkait: [tempel]. Sebelum memberi solusi, sebutkan 
3 kemungkinan penyebab paling mungkin, urutkan dari yang paling mungkin.
```

Ini memaksa AI (dan Anda) berpikir sistematis, serta membantu Anda mengevaluasi apakah penyebab yang disebutkan benar-benar masuk akal untuk konteks kode Anda sebelum menerapkan fix.

## 2. Sertakan Apa yang Sudah Dicoba

```
Saya sudah mencoba [X] dan [Y], keduanya tidak menyelesaikan masalah. 
Error tetap muncul: [pesan error]. Jangan sarankan solusi yang sama.
```

Tanpa ini, AI cenderung mengulang saran generik yang sama meski Anda sudah mencobanya — konteks "sudah dicoba" mempersempit ruang solusi secara signifikan.

## 3. Minta Penjelasan Assumption yang Mendasari Kode

```
Jelaskan asumsi apa saja yang harus benar agar kode ini bekerja sesuai 
harapan. Untuk masing-masing asumsi, bagaimana cara memverifikasinya?
```

Berguna untuk bug yang tidak menghasilkan error eksplisit tapi perilakunya tidak sesuai harapan (silent bug) — sering kali akar masalahnya adalah asumsi yang ternyata salah.

## 4. Minta Reproduksi Minimal

```
Bantu saya buat contoh kode paling minimal yang bisa mereproduksi masalah 
ini, dengan menghilangkan bagian yang tidak relevan.
```

Proses menyusun reproduksi minimal sering kali membantu menemukan akar masalah bahkan sebelum AI selesai memberi jawaban — teknik debugging klasik ("rubber duck debugging") yang tetap ampuh dikombinasikan dengan AI.

## 5. Minta Review dari Sudut Pandang Edge Case

```
Kode ini bekerja untuk kasus normal. Sebutkan edge case yang mungkin belum 
tertangani (input kosong, nilai negatif, concurrency, dll) yang bisa 
menjadi penyebab masalah ini.
```

Berguna khususnya untuk bug yang muncul secara intermiten atau hanya di kondisi tertentu yang sulit direproduksi secara konsisten.

## Prinsip di Baliknya

Kelima pola ini punya benang merah yang sama: memberi AI **konteks terstruktur** dan **memaksa proses berpikir bertahap**, alih-alih meminta jawaban instan dari informasi minim. Prinsip yang sama dibahas lebih dalam soal decomposition dan structured output di [Prompt Engineering Tingkat Lanjut](/posts/prompt-engineering-tingkat-lanjut/).
