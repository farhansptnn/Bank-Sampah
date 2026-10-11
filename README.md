# ♻️ Bank Sampah BPI Lestari

<div align="center">

![React](https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-7.x-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3.x-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-8.x-777BB4?style=for-the-badge&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

**Aplikasi web modern untuk manajemen bank sampah BPI Lestari — dari setoran sampah hingga laporan transaksi.**

> Platform fullstack yang membantu pengelolaan bank sampah secara digital: pencatatan setoran, konversi nilai sampah ke poin/uang, riwayat transaksi, dan pelaporan. Dibangun dengan React + TypeScript (frontend) dan PHP API + MySQL (backend).

</div>

---

## 📌 Tentang Proyek

**Bank Sampah BPI Lestari** adalah aplikasi manajemen bank sampah berbasis web yang mengdigitalisasi proses pencatatan sampah, konversi nilai, dan pengelolaan akun nasabah. Proyek ini menjawab kebutuhan nyata pengelolaan bank sampah komunitas yang sebelumnya masih dilakukan secara manual/berbasis kertas.

---

## ✨ Fitur Utama

| Fitur | Deskripsi |
|---|---|
| 📦 **Setoran Sampah** | Pencatatan jenis dan berat sampah yang disetorkan nasabah |
| 💰 **Konversi Nilai** | Kalkulasi otomatis nilai sampah ke poin atau saldo uang |
| 👤 **Manajemen Nasabah** | Pendaftaran, profil, dan riwayat transaksi nasabah |
| 📊 **Dashboard & Laporan** | Ringkasan statistik setoran dan penarikan |
| 📰 **Berita & Edukasi** | Konten edukasi tentang pengelolaan sampah |
| 🪜 **Panduan Langkah** | Step-by-step cara berpartisipasi di bank sampah |
| 🌄 **Landing Page** | Halaman publik informatif tentang BPI Lestari |

---

## 🛠️ Tech Stack

### Frontend
- **React 19** — UI library dengan hooks modern
- **TypeScript 5** — Type-safe development untuk mencegah bug runtime
- **Vite 7** — Build tool super cepat dengan Hot Module Replacement
- **Tailwind CSS 3** — Utility-first CSS framework
- **ShadCN/UI** — 40+ komponen UI siap pakai (Radix UI based)
- **React Hook Form** + **Zod** — Form handling & validasi schema

### Backend
- **PHP 8** — REST API server-side
- **MySQL 8** — Relational database
- **PDO** — Database abstraction layer

### Arsitektur Frontend
```
src/
├── components/     # Reusable UI components (ShadCN + custom)
├── sections/       # Page sections (Hero, Features, Steps, News, dll)
├── context/        # React Context untuk state management global
├── hooks/          # Custom hooks
├── types/          # TypeScript type definitions
├── lib/            # Utility functions
├── App.tsx         # Root component & routing
└── main.tsx        # Entry point
```

---

## 📁 Struktur Proyek

```
Bank-Sampah/
├── src/                    # Source code React + TypeScript
│   ├── components/         # Komponen UI reusable
│   ├── sections/           # Section halaman (Hero, Steps, News, dll)
│   ├── context/            # Global state management
│   ├── hooks/              # Custom React hooks
│   └── types/              # Type definitions TypeScript
├── api/                    # Backend PHP REST API
├── assets/                 # Asset statis
├── public/                 # File publik
├── database.sql            # Schema & seed database MySQL
├── tailwind.config.js      # Konfigurasi Tailwind CSS + ShadCN theme
├── vite.config.ts          # Konfigurasi Vite bundler
├── tsconfig.json           # Konfigurasi TypeScript
└── package.json            # Dependencies & scripts
```

---

## 🚀 Cara Menjalankan Proyek

### Prasyarat
- **Node.js 20+**
- **PHP 8+** & **MySQL 8** (XAMPP/LAMP)
- **Git**

### Instalasi

```bash
# 1. Clone repositori
git clone https://github.com/farhansptnn/Bank-Sampah.git
cd Bank-Sampah

# 2. Install dependencies frontend
npm install

# 3. Jalankan development server
npm run dev
```

```bash
# 4. Setup backend (PHP API)
# Pastikan XAMPP/server PHP sudah berjalan
# Import database
mysql -u root -p < database.sql
```

```bash
# 5. Build untuk production
npm run build

# 6. Preview hasil build
npm run preview
```

### Scripts Tersedia

| Command | Deskripsi |
|---|---|
| `npm run dev` | Jalankan dev server dengan HMR |
| `npm run build` | Build untuk production (TypeScript check + Vite build) |
| `npm run lint` | Cek kualitas kode dengan ESLint |
| `npm run preview` | Preview hasil production build |

---

## 🧩 Komponen ShadCN/UI yang Digunakan

Proyek ini menggunakan **40+ komponen** dari ShadCN/UI:

`Accordion` `Alert Dialog` `Avatar` `Badge` `Button` `Calendar` `Card` `Carousel` `Chart` `Checkbox` `Dialog` `Drawer` `Dropdown Menu` `Form` `Input` `Navigation Menu` `Pagination` `Popover` `Progress` `Select` `Sheet` `Sidebar` `Skeleton` `Slider` `Table` `Tabs` `Toast (Sonner)` `Tooltip` dan lainnya.

---

## 💡 Highlight Teknis untuk Reviewer

- **TypeScript strict mode** — Seluruh codebase menggunakan type-safe TypeScript
- **Component-based architecture** — Pemisahan section, komponen, dan logic yang bersih
- **ShadCN/UI** — Penggunaan design system modern berbasis Radix UI (accessible by default)
- **React Context** — State management tanpa library eksternal (ringan & efisien)
- **Custom Hooks** — Abstraksi logic yang reusable
- **Vite bundler** — Build time yang sangat cepat dibanding CRA/Webpack
- **Fullstack integration** — Frontend React berkomunikasi dengan backend PHP via REST API
- **Type-safe API calls** — Interface TypeScript untuk setiap response API

---

## 👤 Developer

**Farhan Septian**  
📧 [farhansptnn@github](https://github.com/farhansptnn)

---

## 📄 Lisensi

Proyek ini dikembangkan untuk keperluan digitalisasi bank sampah komunitas BPI Lestari.  
© 2025 Bank Sampah BPI Lestari
