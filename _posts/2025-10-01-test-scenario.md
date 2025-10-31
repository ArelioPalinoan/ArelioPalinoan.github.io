---
layout: post
title: "Test Scenario, Test Case, dan Bug Report"
date: 2025-10-01
categories: [Software Testing and Quality Assurance]
tags: [Article]
---
# Test Scenario, Test Case, dan Bug Report

Test scenario, test case, dan bug report adalah tiga elemen fundamental dan saling terkait dalam proses pengujian perangkat lunak (*Software Testing*). Ketiganya memastikan fungsionalitas aplikasi diuji secara komprehensif dan setiap kekurangan didokumentasikan dengan jelas.

## 1. Test Scenario (Skenario Pengujian)

Test Scenario adalah gambaran tingkat tinggi (umum) yang menjelaskan apa yang akan diuji untuk memverifikasi fungsionalitas aplikasi. Ini adalah ide atau tujuan pengujian, bukan detail langkah-langkah.

* **Fokus:** Apa yang harus diverifikasi.
* **Tujuan:** Memastikan keseluruhan fitur utama aplikasi diuji.
* **Contoh:** "Verifikasi fungsionalitas *login* pengguna," atau "Uji proses pembayaran dengan kartu kredit."

## 2. Test Case (Kasus Pengujian)

Test Case adalah serangkaian langkah detail dan terstruktur yang diikuti oleh *tester* untuk memverifikasi fungsi atau *scenario* tertentu. Test Case harus spesifik dan menghasilkan hasil yang dapat diukur.

| Komponen Kunci | Deskripsi |
| :--- | :--- |
| **Test Case ID** | Nomor unik untuk identifikasi (misalnya, TC-LOGIN-001). |
| **Precondition** | Kondisi yang harus dipenuhi sebelum pengujian dimulai (misalnya, pengguna sudah terdaftar). |
| **Test Steps** | Langkah-langkah detail yang harus dilakukan (*input*). |
| **Expected Result** | Hasil yang diharapkan dari langkah-langkah yang dilakukan. |
| **Actual Result** | Hasil yang benar-benar terjadi saat pengujian. |
| **Status** | Status pengujian (*Pass* atau *Fail*). |

## 3. Bug Report (Laporan Bug)

Bug Report adalah dokumen formal yang dibuat ketika *tester* menemukan perbedaan antara **Actual Result** (Hasil Aktual) dan **Expected Result** (Hasil yang Diharapkan) dari suatu Test Case.

Laporan ini memastikan *developer* dapat mereproduksi masalah dan memperbaikinya.

### Komponen Utama Bug Report

| Komponen | Tujuan |
| :--- | :--- |
| **Bug Title** | Judul singkat, jelas, dan spesifik tentang masalah (misalnya, "Perhitungan diskon salah pada produk X"). |
| **Bug ID** | Penanda unik untuk melacak *bug* (misalnya, BUG-PAY-005). |
| **Steps to Reproduce** | Langkah detail yang diperlukan agar *developer* dapat melihat masalah yang sama. |
| **Actual vs. Expected Result** | Menjelaskan apa yang terjadi dan apa yang seharusnya terjadi. |
| **Severity** | Tingkat keparahan dampak *bug* terhadap sistem (Critical, Major, Minor). |
| **Priority** | Urutan kapan *bug* harus diperbaiki (P1-Urgent, P4-Low). |
| **Environment/Build** | Informasi tentang *browser*, OS, atau versi *build* aplikasi saat *bug* ditemukan. |

### Klasifikasi Bug: Severity vs. Priority

* **Severity (Tingkat Keparahan):** Mengukur seberapa parah dampak *bug* terhadap fungsi sistem.
    * *Contoh:* **Critical** (Aplikasi *crash* total) atau **Minor** (Kesalahan ketik).
* **Priority (Prioritas):** Mengukur seberapa mendesak *bug* harus diperbaiki.
    * *Contoh:* **P1-Urgent** (*Bug* menghentikan bisnis inti, harus diperbaiki segera).

## Cara Menghindari Bug

Meskipun *bug* tak terhindarkan, ada praktik yang dapat meminimalkannya:

1.  **Pahami Persyaratan:** Pastikan semua persyaratan dipahami dengan jelas oleh seluruh tim.
2.  **Unit Testing:** Lakukan pengujian unit di tahap awal untuk mendeteksi *bug* di kode terkecil.
3.  **Code Review:** Minta pengembang lain meninjau kode untuk menemukan kesalahan logika.
4.  **Rencana Pengujian:** Ikuti *Testing Plan* yang terstruktur.