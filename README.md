📦 Sistem Manajemen Gudang

<div align="center">

![Gudang Management System](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

*Sistem manajemen gudang modern dengan antarmuka yang intuitif dan fitur lengkap*

[![GitHub stars](https://img.shields.io/github/stars/FahmiSaddam/gudang.svg?style=social&label=Star)](https://github.com/FahmiSaddam/gudang)
[![GitHub forks](https://img.shields.io/github/forks/FahmiSaddam/gudang.svg?style=social&label=Fork)](https://github.com/FahmiSaddam/gudang/fork)

</div>

---

## 🌟 Fitur Utama

<table>
<tr>
<td width="50%">

### 📊 **Dashboard Interaktif**
- Statistik real-time stok barang
- Grafik aktivitas harian/mingguan/bulanan
- Informasi pengguna dan role-based access

### 📦 **Manajemen Stok**
- Penerimaan barang dengan validasi lengkap
- Pengeluaran barang dengan kontrol stok
- Koreksi stok untuk supervisor & manajer
- Laporan stok komprehensif

</td>
<td width="50%">

### 👥 **Manajemen Pengguna**
- 3 Level akses: Operator, Supervisor, Manajer
- Profil pengguna dengan foto profil
- Audit trail untuk semua aktivitas
- Keamanan berlapis dan validasi data

### 📈 **Laporan & Analytics**
- Histori transaksi lengkap
- Dashboard grafik interaktif
- Export data dan pencarian advanced
- Real-time monitoring stok

</td>
</tr>
</table>

---

## 🚀 Quick Start

### Prerequisites

Pastikan sistem Anda memiliki:

```bash
PHP >= 7.4
MySQL >= 5.7
Apache/Nginx Web Server
```

### 🔧 Instalasi

1. **Clone repository**
   ```bash
   git clone https://github.com/FahmiSaddam/gudang.git
   cd gudang
   ```

2. **Setup Database**
   ```sql
   CREATE DATABASE gudang_db;
   ```
   
3. **Import struktur database** (jika ada file SQL)
   ```bash
   mysql -u root -p gudang_db < gudang_db.sql
   ```

4. **Konfigurasi Database**
   
   Edit file database.php:
   ```php
   $host = 'localhost';
   $dbname = 'gudang_db';
   $user = 'root';        // Username database Anda
   $pass = '';            // Password database Anda
   ```

5. **Setup Web Server**
   
   Pastikan document root mengarah ke folder project atau akses melalui:
   ```
   http://localhost/gudang/
   ```

---

## 👤 User Roles & Permissions

<div align="center">

| Role | Dashboard | Operasional | Administrasi | Sistem |
|------|-----------|-------------|--------------|---------|
| **🔧 Operator** | ✅ | ✅ Penerimaan & Pengeluaran | ❌ | ❌ |
| **👨‍💼 Supervisor** | ✅ | ✅ Semua Operasional | ✅ Koreksi & Laporan | ❌ |
| **👑 Manajer** | ✅ | ✅ Semua Operasional | ✅ Semua Administrasi | ✅ Manajemen User |

</div>

---

## 📁 Struktur Project

```
gudang/
├── 📄 index.php                 # Halaman login
├── 📄 dashboard.php             # Dashboard utama
├── 📄 dashboard_grafik.php      # Dashboard dengan grafik
├── 📂 config/
│   └── 📄 database.php          # Konfigurasi database
├── 📂 includes/
│   ├── 📄 header.php            # Header template
│   ├── 📄 footer.php            # Footer template
│   ├── 📄 sidebar.php           # Sidebar navigation
│   └── 📄 auth_check.php        # Validasi autentikasi
├── 📄 penerimaan_barang.php     # Form penerimaan barang
├── 📄 pengeluaran_barang.php    # Form pengeluaran barang
├── 📄 koreksi_stok.php          # Koreksi stok (Supervisor+)
├── 📄 laporan_stok.php          # Laporan stok (Supervisor+)
├── 📄 histori_transaksi.php     # Histori semua transaksi
├── 📄 manajemen_pengguna.php    # Manajemen user (Manajer)
├── 📄 pengguna_form.php         # Form tambah/edit user
├── 📄 pengguna_aksi.php         # Handler aksi user
├── 📄 profil.php               # Profil pengguna & foto
├── 📄 get_profile_pic.php      # Handler foto profil
└── 📄 logout.php               # Logout handler
```

---

## 🛠️ Teknologi yang Digunakan

<div align="center">

### Backend
[![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)](https://php.net)
[![MySQL](https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white)](https://mysql.com)

### Frontend
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://javascript.com)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white)](https://getbootstrap.com)

### Libraries & Frameworks
- **SB Admin 2** - Admin template
- **Chart.js** - Grafik interaktif
- **Font Awesome** - Icons
- **jQuery** - JavaScript library

</div>

---

## 🔒 Fitur Keamanan

- ✅ **Prepared Statements** - Mencegah SQL Injection
- ✅ **Session Management** - Kontrol akses pengguna
- ✅ **Role-based Access Control** - Pembatasan akses berdasarkan role
- ✅ **Input Validation** - Validasi semua input pengguna
- ✅ **CSRF Protection** - Perlindungan dari serangan CSRF
- ✅ **File Upload Security** - Validasi file upload
- ✅ **Audit Trail** - Pencatatan semua aktivitas

---

## 📈 Database Schema

<details>
<summary><strong>📋 Klik untuk melihat struktur database</strong></summary>

### Tables:
- **users** - Data pengguna dan autentikasi
- **produk** - Master data produk
- **lokasi_penyimpanan** - Master lokasi penyimpanan
- **stok** - Data stok barang per lokasi
- **transaksi_penerimaan** - Transaksi penerimaan barang
- **transaksi_pengeluaran** - Transaksi pengeluaran barang
- **transaksi_koreksi** - Transaksi koreksi stok
- **audit_trail** - Log aktivitas pengguna

</details>

---

## 🤝 Contributing

Kontribusi sangat diterima! Silakan:

1. **Fork** repository ini
2. Buat **feature branch** (`git checkout -b feature/AmazingFeature`)
3. **Commit** perubahan (`git commit -m 'Add some AmazingFeature'`)
4. **Push** ke branch (`git push origin feature/AmazingFeature`)
5. Buat **Pull Request**

---

## 📞 Support & Contact

<div align="center">

[![GitHub Issues](https://img.shields.io/badge/Issues-GitHub-red?style=for-the-badge&logo=github)](https://github.com/FahmiSaddam/gudang/issues)
[![GitHub Discussions](https://img.shields.io/badge/Discussions-GitHub-blue?style=for-the-badge&logo=github)](https://github.com/FahmiSaddam/gudang/discussions)

**Butuh bantuan?** Jangan ragu untuk membuat issue atau diskusi!

</div>

---

## 📄 License

Project ini dilisensikan di bawah MIT License - lihat file LICENSE untuk detail.

---

<div align="center">

### ⭐ Jika project ini membantu, berikan star!

**Dibuat dengan ❤️ oleh [FahmiSaddam](https://github.com/FahmiSaddam)**

[![GitHub followers](https://img.shields.io/github/followers/FahmiSaddam.svg?style=social&label=Follow)](https://github.com/FahmiSaddam)

---

*© 2025 Sistem Manajemen Gudang. All rights reserved.*

</div>
