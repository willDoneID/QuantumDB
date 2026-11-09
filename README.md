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

Pastikan kamu sudah menginstal **Rust** dan **Cargo** di komputer kamu. Jika belum, instal melalui [rustup.rs](https://rustup.rs/).

1. **Clone repository ini:**
   ```bash
   git clone https://github.com/willDoneID/QuantumDB.git
   cd QuantumDB
