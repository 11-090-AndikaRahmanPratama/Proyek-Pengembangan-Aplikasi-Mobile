# 📱 [Aplikasi] - Tugas Besar Pengembangan Aplikasi Mobile
**Program Studi Teknik Informatika - Institut Teknologi Sumatera (ITERA)**

Aplikasi ini dikembangkan sebagai Proyek Akhir mata kuliah Pengembangan Aplikasi Mobile menggunakan framework **Kotlin Multiplatform (KMP)**.

---

## 👥 Profil Kelompok
| Nama | NIM |
| :--- | :--- |
| **Andika Rahman Pratama** | 123140090
| **Muhammad Farhan Muzakhi** | 123140075

---

## 🚀 Deskripsi Proyek
....

### ✨ Fitur Utama
- 🔒 **Secure Data:** Penyimpanan data lokal terenkripsi menggunakan SQLDelight.
- 🤖 **AI-Powered:** Integrasi Google Gemini API untuk [Sebutkan fitur AI-nya].
- 🌓 **Adaptive Theme:** Mendukung Dark Mode dan Light Mode sesuai preferensi sistem.
- 📱 **Cross-Platform:** Tersedia untuk perangkat Android dan iOS (Single Codebase).

---

## 🏗️ Arsitektur & Teknologi
Aplikasi ini mengimplementasikan **Clean Architecture** dengan pola **MVVM** untuk memastikan kode yang modular dan mudah diuji.

### Tech Stack
- **UI:** Compose Multiplatform (Material 3)
- **Dependency Injection:** Koin
- **Database:** SQLDelight (Local Persistence)
- **Networking:** Ktor Client
- **Reactive State:** Kotlin Flow & StateFlow
- **AI Integration:** Google Gemini SDK

### Diagram Arsitektur
```mermaid
graph TD
    subgraph Presentation_Layer
        A[Compose Screens] <--> B[ViewModels]
    end
    
    subgraph Domain_Layer
        C[Use Cases] --> D[Repository Interfaces]
        B --> C
    end
    
    subgraph Data_Layer
        D --> E[Repository Impl]
        E --> F[SQLDelight / Local]
        E --> G[Ktor / Remote API]
        E --> H[Gemini API]
    end
