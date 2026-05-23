## 🖥️ NetMap Pro — Inventaris Aset TI & Penemuan Jaringan

**NetMap Pro** adalah aplikasi web lengkap untuk melacak perangkat, perangkat lunak, pengguna, kredensial, dan topologi jaringan secara real-time. Dibangun murni dengan HTML, CSS, dan JavaScript tanpa backend atau dependensi eksternal, menggunakan IndexedDB sebagai database lokal dan SubtleCrypto untuk autentikasi aman.

---

## 🚀 Fitur

- 📊 **Dasbor Waktu Nyata** — Statistik ringkasan perangkat, status online/offline, garansi, OS, dan lainnya.
- 🖥️ **Manajemen Perangkat** — Tabel yang dapat diurutkan, dicari, dan difilter. CRUD lengkap (tambah, edit, hapus).
- 💿 **Inventaris Perangkat Lunak** — Pelacakan setiap aplikasi terpasang di seluruh armada dengan versi.
- 👤 **Akun Pengguna** — Deteksi akun lokal dan domain, status admin, dan login terakhir.
- 🌐 **Jaringan & VLAN** — Inventaris subnet, VLAN, gateway, dan alokasi perangkat.
- 🔐 **Brankas Kredensial** — Simpan kredensial SSH/WMI/SNMP/API untuk pemindaian.
- 🔎 **Pemindaian Penemuan Simulasi** — Pemindaian jaringan dengan progress bar dan output realistis, perangkat baru otomatis masuk database.
- 📋 **8 Laporan Bawaan** — Perangkat offline, garansi berakhir, OS EOL, perangkat usang, workstation belum ditugaskan, dll.
- 📝 **Catatan Audit** — Setiap aksi tercatat dengan timestamp dan atribusi pengguna.
- 📥 **Ekspor CSV** — Ekspor data perangkat, software, pengguna, dan laporan.
- 📌 **Panel Detail Geser** — Lihat detail perangkat dalam 4 tab: Ikhtisar, Software, Pengguna, Jaringan.
- 🔒 **Autentikasi Aman** — Hashing kata sandi SHA-256 + salt acak 16-byte menggunakan SubtleCrypto.
- 🧪 **Akun Demo** — Satu klik langsung masuk ke organisasi "Acme Corp" yang telah terisi puluhan data realistis.

---

## 🧰 Teknologi

| Teknologi        | Keterangan                                                                 |
|------------------|----------------------------------------------------------------------------|
| **HTML/CSS/JS**  | Vanilla, tanpa framework atau build tools.                                 |
| **IndexedDB**    | Database asli browser dengan 9 object store, indeks, dan cascade delete.   |
| **SubtleCrypto** | Web Crypto API untuk hashing kata sandi SHA-256 dengan salt.               |
| **GitHub Pages** | Hosting statis langsung dari repository.                                   |

---

## 🖥️ Menjalankan

1. **Clone repository** ini atau download file `index.html`.
2. Buka file `index.html` di browser modern (Chrome, Firefox, Edge).
3. **Tidak perlu server**, tidak perlu `npm install`, tidak perlu build. Semua berjalan di sisi klien.

Atau langsung akses melalui **GitHub Pages** jika sudah di-deploy.

---

## 🔑 Kredensial

### Akun Admin Bawaan
- **Username:** `admin`
- **Password:** `admin`

### Akun Demo
Klik tombol **"Jelajahi dengan Akun Demo"** di layar login untuk langsung masuk ke organisasi demo "Acme Corp" yang sudah terisi:
- 87 perangkat dari 13 jenis OS
- Ratusan instalasi software
- Akun pengguna lokal & domain
- 5 subnet, 4 kredensial, 3 pemindaian contoh
- Catatan audit lengkap

Akun demo **direset setiap kali login** sehingga Anda bebas bereksperimen.

---

## 🧪 Teknis

- **Database IndexedDB** — 9 penyimpanan objek: `orgs`, `devices`, `software`, `users`, `networks`, `credentials`, `scans`, `auditLogs`, `settings`. Dilengkapi indeks untuk pencarian cepat dan penghapusan berjenjang (cascade delete).
- **Keamanan** — Password tidak pernah disimpan dalam bentuk plaintext. Kombinasi SHA-256 + salt 16-byte membuat brute-force tidak praktis.
- **Ketahanan Data** — Semua data (perangkat, software, pengguna, pemindaian) tetap ada setelah refresh tab, restart browser, atau bahkan reboot sistem.
- **UI Responsif** — Didesain untuk desktop dan tablet, dengan panel geser yang berfungsi baik di layar kecil.

---

## 🌟 Dukungan

Jika proyek ini bermanfaat, beri ⭐ di GitHub dan bagikan ke rekan tim TI Anda!
