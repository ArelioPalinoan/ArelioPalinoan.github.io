---
layout: post
title: "Unit Testing"
date: 2025-10-08
categories: [Software Testing and Quality Assurance]
tags: [Article]
---
# Unit Testing

Unit Testing adalah jenis pengujian perangkat lunak yang paling dasar. Pengujian ini berfokus pada pengujian unit-unit terkecil dalam sebuah sistem, seperti *function*, *method*, atau *class*, secara terpisah tanpa bergantung pada komponen lain.

## Apa dan Mengapa Unit Testing?

| Aspek | Deskripsi |
| :--- | :--- |
| **Fokus Utama** | Unit kode terkecil yang dapat diuji secara independen. |
| **Posisi** | Berada di dasar *Testing Pyramid*, menjadikannya pengujian **paling cepat** dan **paling murah** untuk dieksekusi. |
| **Tujuan Kualitas** | Memastikan setiap bagian kode berfungsi dengan benar sebelum diintegrasikan dengan sistem yang lebih besar. |

### Manfaat Utama Unit Testing:

1.  **Deteksi Bug Dini:** Menemukan dan memperbaiki *bug* di tahap pengembangan paling awal, sehingga menghemat biaya perbaikan besar di akhir.
2.  **Memudahkan Refactoring:** Berfungsi sebagai "jaring pengaman" yang menjamin fungsionalitas yang ada tidak rusak saat kode dimodifikasi atau distruktur ulang.
3.  **Meningkatkan Kualitas Kode:** Mendorong penulisan kode yang lebih modular, terstruktur, dan mudah dipelihara.

## Pola Dasar Unit Test: Arrange, Act, Assert (AAA)

Setiap *unit test* yang baik harus mengikuti pola tiga langkah ini agar terstruktur dan mudah dipahami:

1.  **Arrange (Persiapan):** Menyiapkan data awal, objek, dan kondisi yang dibutuhkan untuk memulai tes.
2.  **Act (Tindakan):** Menjalankan fungsi atau metode yang akan diuji.
3.  **Assert (Verifikasi Hasil):** Membandingkan Hasil Aktual dengan Hasil yang Diharapkan.

### Memverifikasi Hasil (Tahap Assert)

Tahap `Assert` adalah tahap inti untuk memastikan kode bekerja sesuai logika. Verifikasi dapat berupa:
* **Verifikasi Nilai:** Memastikan fungsi mengembalikan nilai yang benar.
* **Verifikasi State:** Memastikan status objek internal berubah sesuai yang diharapkan (misalnya, jumlah item di keranjang bertambah).
* **Verifikasi Pengecualian (*Exceptions*):** Memastikan kode mengeluarkan *error* yang tepat (misalnya, `ValueError` atau `OverflowError`) ketika diberikan *input* yang salah.

## Prinsip Isolasi: Kunci Pengujian Unit Sejati

Agar *unit test* benar-benar independen dan cepat, kita harus mengisolasi ketergantungan eksternal.

* **Kebutuhan Isolasi:** Unit kode sering kali bergantung pada komponen lain seperti database, API eksternal, atau sistem file.
* **Solusi (Mocking/Stubbing):** Mengganti ketergantungan nyata dengan objek tiruan (*Mock* atau *Stub*) yang hanya meniru perilaku objek aslinya. Hal ini memastikan bahwa kegagalan tes disebabkan oleh kode unit yang diuji, bukan oleh kegagalan sistem eksternal.

## Pengenalan Framework Unit Testing Populer

| Framework | Ekosistem Kode | Keunggulan Kunci |
| :--- | :--- | :--- |
| **JUNIT 5** | Java (dan bahasa berbasis JVM) | Framework standar dan matang untuk Java, berbasis Anotasi. |
| **JEST** | JavaScript (React, Node.js) | Minimal konfigurasi (*Zero-Config*), cepat, dengan fitur *Snapshot Testing*. |
| **PYTEST** | Python | Sintaks yang sederhana dan mudah dibaca, serta sistem *fixtures* yang kuat. |