# QuantumDB 🚀

[![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](LICENSE)
[![Language: Rust](https://img.shields.io/badge/Language-Rust-orange.svg?logo=rust)](https://www.rust-lang.org/)
[![Owner: Wildan Erly](https://img.shields.io/badge/Owner-Wildan_Erly-emerald.svg)](https://github.com/willDoneID)

**QuantumDB** adalah *in-memory database engine* berperforma tinggi yang dibangun menggunakan **Rust**. Uniknya, database ini menggunakan **Query Language berbasis Bahasa Indonesia** untuk interaksi dan manipulasi data.

Proyek ini merupakan bagian dari ekosistem **Will Done Project (`willDoneID`)** — diarsitekturi oleh **Wildan Erly** sebagai sarana eksplorasi mendalam terkait arsitektur penyimpanan data, efisiensi manajemen memori, dan pembuatan parser dari dasar.

---

## ⚡ Estimasi Performa (Benchmarks)

Mengoptimalkan keunggulan zero-cost abstraction dan keamanan memori dari Rust (`std::collections::HashMap`), QuantumDB dirancang untuk kecepatan eksekusi ultra-rendah:

- ✍️ **Write (`SIMPAN`):** `~1.5 - 2.0 Juta OPS` (tergantung spesifikasi perangkat keras)
- 📖 **Read (`AMBIL`):** `~3.0 - 5.0 Juta OPS` (pencarian berbasis *Hash Table* $O(1)$)

---

## 🛠️ Cara Instalasi & Menjalankan

Pastikan kamu sudah memasang **Rust** dan **Cargo**. Jika belum, unduh melalui [rustup.rs](https://rustup.rs/).

1. **Clone repositori ini:**
   ```bash
   git clone https://github.com/willDoneID/QuantumDB.git
   cd QuantumDB
   ```

2. **Jalankan dalam mode *release* (untuk performa optimal):**
   ```bash
   cargo run --release
   ```

---

## 📖 Sintaks Query (Bahasa Indonesia)

Setelah masuk ke antarmuka terminal `quantumdb>`, kamu bisa menggunakan perintah berikut:

### 1. Menyimpan Data (`SIMPAN`)
Digunakan untuk memasukkan atau memperbarui nilai berdasarkan kunci (*key*).
```text
quantumdb> SIMPAN nama Budi
[SUKSES] Data berhasil disimpan.
```

### 2. Mengambil Data (`AMBIL`)
Digunakan untuk membaca nilai data berdasarkan kunci (*key*).
```text
quantumdb> AMBIL nama
[HASIL] Budi
```

### 3. Keluar Aplikasi (`KELUAR`)
Digunakan untuk mengakhiri sesi interaktif database.
```text
quantumdb> KELUAR
Sampai jumpa!
```

---

## 🤝 Kontribusi

Kontribusi, kritik, dan gagasan baru sangat terbuka! Silakan buat *Pull Request* atau buka *Issue* di repositori ini.

---

## 📝 Lisensi

Proyek ini dirilis di bawah lisensi [GNU Affero General Public License v3.0 (AGPL-3.0)](LICENSE).  
Copyright (c) 2026 **Wildan Erly** (Will Done Project).
