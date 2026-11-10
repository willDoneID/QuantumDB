# QuantumDB 🚀

QuantumDB adalah proyek database engine *in-memory* sederhana yang dibuat menggunakan bahasa pemrograman **Rust** untuk mencapai performa *read* dan *write* yang tinggi, dengan keunikan menggunakan **Query Language berbasis Bahasa Indonesia**. 

Proyek ini dibangun sebagai sarana pembelajaran untuk memahami arsitektur penyimpanan data, manajemen memori, dan pembuatan parser dari dasar.

---

## ⚡ Perkiraan Performa (Benchmarks)
Karena menggunakan struktur data *in-memory* (`HashMap` di Rust) tanpa overhead jaringan yang kompleks, QuantumDB dirancang untuk memiliki performa yang sangat cepat:
* **Write (SIMPAN):** ~1.5 - 2 juta operasi per detik (tergantung spesifikasi hardware).
* **Read (AMBIL):** ~3 - 5 juta operasi per detik (pencarian berbasis *hash O(1)*).

---

## 🛠️ Cara Instalasi & Menjalankan

Pastikan kamu sudah menginstal **Rust** dan **Cargo** di komputer kamu. Jika belum, instal melalui https://rustup.rs/

1. **Clone repository ini:**
   git clone https://github.com/willDoneID/QuantumDB.git
   cd quantumdb

2. **Jalankan program dalam mode release (untuk performa optimal):**
   cargo run --release

---

## 📖 Cara Penggunaan (Syntax)

Setelah program berjalan, kamu akan masuk ke antarmuka terminal `quantumdb>`. Berikut adalah perintah dasar yang didukung saat ini:

### 1. Menyimpan Data (`SIMPAN`)
Digunakan untuk memasukkan atau memperbarui data.

quantumdb> SIMPAN nama Budi
Sukses: Data berhasil disimpan.

### 2. Mengambil Data (`AMBIL`)
Digunakan untuk membaca data berdasarkan kunci (*key*).

quantumdb> AMBIL nama
Hasil: Budi

### 3. Keluar Aplikasi (`KELUAR`)
Digunakan untuk menutup sesi database.

quantumdb> KELUAR
Sampai jumpa!

---

## 🤝 Kontribusi
Kontribusi, kritik, dan saran sangat terbuka! Silakan buat *Pull Request* atau buka *Issues* jika kamu memiliki ide menarik untuk pengembangan QuantumDB.

## 📝 Lisensi
Proyek ini dilisensikan di bawah MIT License (LICENSE).
