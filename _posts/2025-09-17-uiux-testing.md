---
layout: post
title: "UI/UX Testing"
date: 2025-09-17
categories: [Software Testing and Quality Assurance]
tags: [Article]
image:
  path: /assets/img/sample.jpg
  alt: "Sample image"
---
# UI/UX Testing

Pengujian UI (User Interface) dan UX (User Experience) adalah dua proses penting yang memastikan interaksi pengguna dengan perangkat lunak berjalan optimal.

## Perbedaan Mendasar

| Aspek | UI Testing | UX Testing |
| :--- | :--- | :--- |
| **Fokus** | Tampilan antarmuka: warna, ikon, tata letak (*layout*), dan responsivitas. | Pengalaman pengguna: efektivitas, efisiensi, dan kepuasan secara keseluruhan. |
| **Tujuan** | Memastikan elemen visual ditampilkan dengan benar dan konsisten di semua platform. | Memastikan pengguna dapat menyelesaikan tugas dan mencapai tujuan mereka dengan mudah. |
| **Contoh** | Memeriksa apakah ukuran *font* dan tombol terbaca jelas di HP dan desktop. | Menguji apakah alur pendaftaran atau pembelian berjalan mulus dan intuitif. |

## Fokus Utama UI Testing

UI Testing berfokus pada elemen visual dan teknis antarmuka:

1.  **Konsistensi Visual:** Memastikan *style* (warna, *font*, ukuran tombol, ikon) seragam di semua halaman.
    * *Tools:* *Checklist* manual, *Automated Visual Regression Testing*.
2.  **Responsivitas:** Memastikan desain tetap nyaman dan berfungsi baik di berbagai ukuran layar (*desktop*, tablet, *mobile*).
    * *Tools:* *Automated testing* (misalnya BrowserStack).
3.  **Kompatibilitas (*Cross-Browser*):** Memastikan UI bekerja dengan baik di berbagai *browser* (Chrome, Firefox, Safari) dan sistem operasi.

## Fokus Utama UX Testing

UX Testing berfokus pada kegunaan, alur, dan aksesibilitas:

1.  **Alur Kerja (*Workflow*):** Proses terintegrasi yang melibatkan perencanaan, rekrutmen pengguna, pelaksanaan sesi uji (observasi), dan analisis data untuk mengoptimalkan *user journey*.
2.  **Kegunaan (*Usability*):** Mengacu pada seberapa mudah dan efektif pengguna dapat menggunakan aplikasi.
    * **Tujuan:** Mengidentifikasi cacat desain yang menghambat pengguna.
3.  **Aksesibilitas (*Accessibility*):** Memastikan aplikasi dapat digunakan oleh semua orang, termasuk penyandang disabilitas, dengan mengacu pada standar global seperti **WCAG** (Web Content Accessibility Guidelines).

## Metode dan Tools Kunci

* **Manual/Step-by-Step:** Dilakukan oleh QA atau pengguna untuk mengecek tampilan dan alur secara langsung.
* **Heuristic Evaluation:** Mengevaluasi desain berdasarkan 10 prinsip kegunaan yang diakui secara umum (misalnya, Konsistensi, Pencegahan Kesalahan).
* **Heatmaps:** Alat visualisasi yang menunjukkan area yang paling sering di-*klik* atau diperhatikan pengguna, membantu memahami perilaku pengguna terhadap UI.
* **A/B Testing:** Membandingkan dua versi desain (A dan B) untuk mengukur performa mana yang menghasilkan konversi atau klik yang lebih baik.