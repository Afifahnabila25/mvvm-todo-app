# To-Do List App (Android Room Practice) 📝

Aplikasi To-Do List sederhana berbasis Android yang dibangun untuk mempraktikkan pengelolaan data lokal (Local Database). Proyek ini dibuat sebagai pemenuhan Tugas Praktikum **Pengembangan Aplikasi Perangkat Bergerak (PAPB)** materi Room Database.

Aplikasi ini menerapkan arsitektur **MVVM (Model-View-ViewModel)** dan menggunakan **Jetpack Compose** untuk antarmuka pengguna (UI).

## 🚀 Fitur Utama
Aplikasi ini mendukung operasi CRUD (Create, Read, Update, Delete) secara asinkron:

* **Create**: Menambahkan tugas baru ke dalam daftar.
* **Read**: Menampilkan daftar tugas secara *real-time* (Reactive) menggunakan Kotlin Flow.
* **Update Status**: Menandai tugas sebagai selesai (Check/Uncheck).
* **Update Title**: Mengedit/mengubah nama tugas yang sudah ada (Fitur Refleksi).
* **Delete**: Menghapus tugas dari database.
* **Data Persistence**: Data tersimpan permanen di SQLite dan tidak hilang saat aplikasi ditutup.

## 🛠️ Tech Stack & Library
* **Bahasa**: Kotlin
* **UI Framework**: Jetpack Compose (Material Design 3)
* **Database**: Room Persistence Library (SQLite Abstraction)
* **Arsitektur**: MVVM (Model-View-ViewModel) + Repository Pattern
* **Concurrency**: Kotlin Coroutines & Flow (untuk operasi background)
* **Minimum SDK**: Android 7.0 (API 24)

## 📂 Struktur Project
Struktur kode mengikuti pola MVVM yang direkomendasikan Google:
1.  **Entity**: `Task` (Representasi tabel database).
2.  **DAO**: `TaskDao` (Interface akses data untuk Insert, Update, Delete, Query).
3.  **Repository**: `TaskRepository` (Penghubung antara ViewModel dan Database).
4.  **ViewModel**: `TaskViewModel` (Pengelola State UI dan Logika Bisnis).
5.  **UI**: `MainActivity` & Composable Functions (`TaskScreen`, `TaskItem`).

## 📸 Cara Menjalankan
1.  **Clone** repositori ini ke komputer lokalmu.
2.  Buka project menggunakan **Android Studio** (Versi terbaru disarankan).
3.  Biarkan Gradle mengunduh semua *dependency* yang dibutuhkan.
4.  Jalankan aplikasi (Run) pada Emulator atau Device fisik.

## 👤 Author
Dibuat oleh Afifah Nabila Devi
---
*Project ini dikembangkan berdasarkan Modul Praktikum 7: Mengelola Data Dengan Room.*
