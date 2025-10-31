---
layout: post
title: "API Testing"
date: 2025-10-15
categories: [Software Testing and Quality Assurance]
tags: [Article]
image:
  path: /assets/img/sample.jpg
  alt: "Sample image"
---
# API Testing

API Testing adalah jenis pengujian yang berfokus pada **Application Programming Interface (API)**, yaitu seperangkat aturan dan protokol yang memungkinkan aplikasi atau layanan perangkat lunak berkomunikasi dan bertukar data. Pengujian ini dilakukan pada *layer* logika bisnis (bukan UI) untuk memastikan fungsionalitas, kinerja, keamanan, dan keandalan API.

## Keunggulan Utama Pengujian API

API Testing jauh lebih unggul dan efisien daripada pengujian UI tradisional karena:

1.  **Dukungan Otomatisasi Tinggi:** Lebih mudah dan lebih cepat untuk diotomatisasi. Perubahan pada UI tidak memengaruhi skrip pengujian API, menjadikannya stabil.
2.  **Deteksi Bug Lebih Awal:** Dilakukan di tahap awal SDLC (*Software Development Life Cycle*), memungkinkan *developer* menemukan dan memperbaiki *bug* jauh sebelum mencapai *layer* UI.
3.  **Memastikan Keamanan:** Fokus pada pengujian otentikasi (misalnya, token), otorisasi (akses data), dan validasi *input* untuk mencegah serangan.
4.  **Verifikasi Logika Bisnis:** Menguji logika inti dan alur data secara langsung, tanpa intervensi visual.

## Fokus Utama Dalam API Testing

Pengujian API harus mencakup verifikasi pada beberapa aspek kritis:

| Aspek Pengujian | Tujuan |
| :--- | :--- |
| **Functional Testing** | Memastikan API melakukan fungsi yang dijanjikan, menghasilkan data yang benar, dan menangani parameter *input* yang valid/tidak valid dengan tepat. |
| **Reliability Testing** | Memastikan API dapat terhubung ke sistem lain secara konsisten (misalnya, *database* atau layanan eksternal). |
| **Performance Testing** | Menguji kecepatan respons dan stabilitas API ketika menerima sejumlah besar *request* secara bersamaan (uji *load* dan *stress*). |
| **Security Testing** | Memverifikasi kontrol akses, enkripsi, dan mencegah serangan *injection* pada API *endpoint*. |

## Anatomi Request & Response API

Pengujian API melibatkan pengiriman *request* dan analisis *response* yang diterima:

### 1. Request (Permintaan)

* **HTTP Method (Verb):** Menentukan aksi yang ingin dilakukan server: **GET** (Ambil/Baca), **POST** (Buat/Tulis), **PUT** (Perbarui Penuh), **PATCH** (Perbarui Sebagian), **DELETE** (Hapus).
* **Endpoint (URL):** Alamat spesifik dari sumber daya (*resource*).
* **Header:** Metadata seperti *Content-Type* atau token otentikasi.
* **Body (Payload):** Data yang dikirimkan ke server (terutama pada POST/PUT/PATCH), biasanya dalam format JSON.

### 2. Response (Balasan)

* **Status Code:** Kode numerik yang mengindikasikan hasil pemrosesan:
    * **2xx (Success):** **200 OK** (berhasil), **201 Created** (sumber daya baru dibuat).
    * **4xx (Client Error):** **404 Not Found**, **401 Unauthorized** (tanpa otentikasi), **400 Bad Request** (input salah).
    * **5xx (Server Error):** **500 Internal Server Error** (kesalahan internal server).
* **Body:** Data yang dikembalikan server (misalnya, data yang diminta atau pesan error).

## Tools Populer untuk API Testing

| Tool | Keunggulan Kunci |
| :--- | :--- |
| **Postman** | *API Client* paling populer. Mudah digunakan untuk eksplorasi, *functional testing*, otomatisasi dengan *collections*, dan manajemen *environment*. |
| **SOAPUI** | Kuat untuk API berbasis **SOAP** (XML) dan **REST** (JSON). Ideal untuk pengujian tingkat lanjut: *load testing* dan *security testing*. |