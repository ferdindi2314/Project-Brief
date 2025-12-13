# Cloud Customer Support & Ticketing System

Sistem Layanan Pelanggan dan Tiketing Berbasis Cloud untuk Tugas Akhir

## 📋 Deskripsi Proyek

Cloud Customer Support & Ticketing System adalah aplikasi web berbasis cloud untuk mencatat keluhan pelanggan, permintaan layanan, perbaikan produk, dan manajemen tiket pelanggan secara online. Sistem ini dibangun menggunakan Laravel sebagai frontend dan backend, dengan Firebase sebagai database real-time untuk memastikan respons yang cepat dan sinkronisasi data yang efisien.

## 🎯 Tujuan Proyek

- ✓ Membangun sistem ticketing terpusat untuk menangani keluhan dan permintaan pelanggan
- ✓ Meningkatkan efisiensi proses dukungan pelanggan dengan automasi dan pelacakan
- ✓ Memberikan akses real-time terhadap status tiket untuk pelanggan dan staf support
- ✓ Mengintegrasikan multiple channel komunikasi (email, chat, formulir web)
- ✓ Menyediakan dashboard analitik untuk monitoring kinerja support team
- ✓ Menerapkan sistem notifikasi otomatis untuk update tiket

## 🛠️ Teknologi yang Digunakan

- **Laravel 10** - Backend & Frontend Framework
- **Firebase Firestore** - Real-time Database
- **Firebase Authentication** - Sistem Login dan Keamanan
- **Bootstrap 5** - UI Framework
- **HTML5, CSS3, JavaScript** - Frontend Technologies
- **Cloud Functions** - Backend Logic dan Automasi
- **Firebase Hosting** - Deployment Platform

## ✨ Fitur Utama

### 1. Manajemen Pengguna

- Registrasi dan login multi-role (Admin, Agent, Customer)
- Profil pengguna dengan avatar dan preferensi
- Manajemen hak akses berbasis peran
- Autentikasi dengan email/password dan Google

### 2. Sistem Ticketing

- Pembuatan tiket baru oleh pelanggan
- Kategori tiket dan prioritas (Low, Medium, High, Critical)
- Pelacakan status tiket (Open, In Progress, Resolved, Closed)
- Lampiran file pada tiket (gambar, dokumen)

### 3. Komunikasi

- Thread percakapan dalam setiap tiket
- Notifikasi real-time untuk update tiket
- Email otomatis untuk konfirmasi dan update
- Internal notes untuk agent dan admin

### 4. Pelaporan & Analitik

- Dashboard dengan metrik kinerja
- Laporan tiket per periode
- Analisis waktu respon dan resolusi
- Export data ke format CSV/PDF

## 👥 Pembagian Role Tim

### **Project Manager / Team Lead**

**Tanggung Jawab:**

- Koordinasi tim dan pengaturan timeline
- Review dan approval semua deliverables
- Manajemen repository dan version control
- Dokumentasi proyek lengkap
- Setup dan konfigurasi Firebase

**Deliverables:**

- Project planning dan timeline
- Repository setup dengan Git workflow
- Konfigurasi Firebase Project
- Dokumentasi teknis lengkap

---

### **Backend Developer**

**Tanggung Jawab:**

- Implementasi Laravel REST API
- Integrasi Firebase Firestore
- Sistem autentikasi multi-role
- Business logic dan validation
- Email service integration

**Deliverables:**

- Laravel Controllers dan Models
- API Endpoints untuk CRUD operations
- Middleware untuk authorization
- Service classes untuk Firebase operations
- Mail templates dan notification system

**File yang dikerjakan:**

```
app/
├── Http/Controllers/
│   ├── AuthController.php
│   ├── TicketController.php
│   ├── UserController.php
│   └── DashboardController.php
├── Models/
│   ├── User.php
│   └── Ticket.php
├── Services/
│   ├── FirebaseService.php
│   └── NotificationService.php
└── Middleware/
    └── RoleMiddleware.php
```

---

### **Frontend Developer**

**Tanggung Jawab:**

- Implementasi UI/UX dengan Bootstrap 5
- Laravel Blade templates
- JavaScript interaktif dan real-time features
- Responsive design untuk semua devices
- Integrasi dengan backend API

**Deliverables:**

- Landing page dan authentication pages
- Dashboard untuk setiap role (Admin, Agent, Customer)
- Ticket management interface
- Real-time notification system
- Form validations dan user feedback

**File yang dikerjakan:**

```
resources/
├── views/
│   ├── auth/
│   │   ├── login.blade.php
│   │   └── register.blade.php
│   ├── dashboard/
│   │   ├── admin.blade.php
│   │   ├── agent.blade.php
│   │   └── customer.blade.php
│   ├── tickets/
│   │   ├── index.blade.php
│   │   ├── create.blade.php
│   │   ├── show.blade.php
│   │   └── edit.blade.php
│   └── layouts/
│       ├── app.blade.php
│       └── guest.blade.php
├── css/
│   └── app.css
└── js/
    ├── app.js
    └── firebase-realtime.js
```

---

### **Database Designer / Firebase Specialist**

**Tanggung Jawab:**

- Desain struktur Firestore database
- Implementasi Firebase Cloud Functions
- Security rules untuk Firestore
- Data migration dan seeding
- Performance optimization

**Deliverables:**

- Database schema documentation
- Firestore collections dan indexes
- Cloud Functions untuk automation
- Security rules configuration
- Database seeder dengan sample data

**File yang dikerjakan:**

```
database/
├── migrations/
├── seeders/
└── firestore-schema.json

firebase/
├── functions/
│   ├── index.js
│   ├── ticket-automation.js
│   └── email-triggers.js
├── firestore.rules
└── firestore.indexes.json
```

---

### **QA/Tester & DevOps**

**Tanggung Jawab:**

- Testing semua fitur aplikasi
- Bug tracking dan reporting
- Deployment ke production
- Setup CI/CD pipeline
- Documentation untuk user dan developer

**Deliverables:**

- Test cases documentation
- Bug reports dan fixes verification
- Deployment configuration
- User manual dan technical documentation
- Performance testing report

**File yang dikerjakan:**

```
tests/
├── Feature/
│   ├── AuthenticationTest.php
│   ├── TicketManagementTest.php
│   └── DashboardTest.php
└── Unit/
    ├── UserModelTest.php
    └── FirebaseServiceTest.php

docs/
├── USER_MANUAL.md
├── API_DOCUMENTATION.md
├── DEPLOYMENT_GUIDE.md
└── TESTING_REPORT.md
```

---

## 📁 Struktur Proyek

```
Cloud-Customer-Support/
├── app/
│   ├── Http/
│   │   ├── Controllers/
│   │   └── Middleware/
│   ├── Models/
│   └── Services/
├── bootstrap/
├── config/
│   └── firebase.php
├── database/
│   ├── migrations/
│   └── seeders/
├── firebase/
│   ├── functions/
│   ├── firestore.rules
│   └── firestore.indexes.json
├── public/
│   ├── css/
│   ├── js/
│   └── images/
├── resources/
│   ├── views/
│   ├── css/
│   └── js/
├── routes/
│   ├── web.php
│   └── api.php
├── storage/
├── tests/
├── .env.example
├── .gitignore
├── composer.json
├── package.json
└── README.md
```

## 📅 Timeline Pengembangan

### Fase 1: Analisis dan Perancangan (2 Minggu)

- Analisis kebutuhan
- Desain database
- Perancangan UI/UX
- Setup environment

### Fase 2: Setup dan Autentikasi (1.5 Minggu)

- Setup Laravel
- Konfigurasi Firebase
- Implementasi sistem autentikasi
- Manajemen pengguna

### Fase 3: Sistem Ticketing Inti (2.5 Minggu)

- Modul ticketing
- Pembuatan tiket
- Pelacakan status
- Manajemen kategori

### Fase 4: Komunikasi & Notifikasi (1.5 Minggu)

- Sistem komentar
- Notifikasi real-time
- Integrasi email

### Fase 5: Dashboard & Pelaporan (1.5 Minggu)

- Dashboard analitik
- Sistem pelaporan
- Fitur ekspor data

### Fase 6: Testing & Deployment (1 Minggu)

- Testing sistem
- Bug fixing
- Deployment
- Dokumentasi

## 🚀 Instalasi

### Prerequisites

- PHP >= 8.1
- Composer
- Node.js & NPM
- Firebase Account

### Langkah Instalasi

1. Clone repository

```bash
git clone https://github.com/your-repo/cloud-customer-support.git
cd cloud-customer-support
```

2. Install dependencies

```bash
composer install
npm install
```

3. Setup environment

```bash
cp .env.example .env
php artisan key:generate
```

4. Konfigurasi Firebase

- Buat project di Firebase Console
- Download service account key
- Tambahkan credentials ke `.env`

5. Setup database

```bash
php artisan migrate
php artisan db:seed
```

6. Build assets

```bash
npm run build
```

7. Jalankan development server

```bash
php artisan serve
```

## 🔐 Default Credentials

### Admin

- Email: admin@ticketing.com
- Password: admin123

### Agent

- Email: agent@ticketing.com
- Password: agent123

### Customer

- Email: customer@ticketing.com
- Password: customer123

## 📝 API Documentation

API documentation tersedia di `/docs/API_DOCUMENTATION.md`

## 🧪 Testing

```bash
# Run all tests
php artisan test

# Run specific test
php artisan test --filter=TicketManagementTest
```

## 📧 Contact & Support

- Email: support@ticketing.com
- Documentation: [Link to docs]

## 📄 License

© 2025 - Tugas Akhir UAS - All rights reserved

---

**Catatan untuk Tim:**

- Setiap anggota bertanggung jawab atas bagian masing-masing
- Gunakan Git branch untuk setiap feature (feature/nama-fitur)
- Pull request harus direview sebelum merge ke main
- Dokumentasi harus diupdate seiring development
- Daily standup untuk sync progress
"# Cloud-Customer-Support" 
