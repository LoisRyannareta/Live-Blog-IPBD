# 📌 Live Blog API (FastAPI + WebSocket)

## 📖 Deskripsi Singkat

Project ini adalah aplikasi **Live Blog sederhana** menggunakan **FastAPI** dengan fitur:

* Register user (mahasiswa)
* CRUD blog (Create, Read, Update, Delete)
* Autentikasi menggunakan token (Bearer)
* Realtime update menggunakan **WebSocket**

Setiap perubahan blog (create, update, delete) akan langsung dikirim ke client tanpa refresh halaman.

---

## 📁 Struktur Project

```
PRAKTIKUM2_IPBD/
│
├── main.py              # Backend FastAPI (API + WebSocket)
├── frontend/
│   └── index.html      # Tampilan frontend
├── __pycache__/        # Cache Python (auto generate)
```

### Penjelasan:

* **main.py** → Berisi seluruh logic backend:

  * API endpoint
  * Authentication
  * WebSocket (realtime)
* **frontend/index.html** → UI sederhana untuk:

  * Menampilkan blog
  * Connect ke WebSocket
* ****pycache**** → Folder otomatis Python (tidak perlu diubah)

---

## 🚀 Cara Menjalankan Project

### 1. Install Dependency

Pastikan Python sudah terinstall, lalu install FastAPI & Uvicorn:

```bash
pip install fastapi uvicorn
```

---

### 2. Jalankan Server Backend

Masuk ke folder project, lalu jalankan:

```bash
uvicorn main:app --reload
```

Jika berhasil, akan muncul:

```
Uvicorn running on http://127.0.0.1:8000
```

---

### 3. Akses API Docs (Opsional)

Buka di browser:

```
http://127.0.0.1:8000/docs
```

Di sini kamu bisa test API langsung.

---

### 4. Jalankan Frontend

Buka file:

```
frontend/index.html
```

Langsung di browser (double click / open with browser)

---


## 🎯 Kesimpulan

Project ini menunjukkan:

* Implementasi REST API dengan FastAPI
* Authentication sederhana (Bearer Token)
* Realtime system dengan WebSocket
* Integrasi backend & frontend


