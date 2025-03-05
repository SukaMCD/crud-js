# CRUD JS (Node.js, React, Express)

## 📌 Deskripsi
Proyek ini adalah aplikasi **CRUD (Create, Read, Update, Delete)** yang dibangun menggunakan **Node.js, Express, dan React**. Backend menggunakan **Express.js** sebagai REST API, sedangkan frontend menggunakan **React** untuk antarmuka pengguna.

## 🛠 Teknologi yang Digunakan
- **Frontend:** React, React Router, Axios
- **Backend:** Node.js, Express, MySQL

## 🚀 Instalasi

### 1. Clone Repository
```sh
git clone https://github.com/SukaMCD/crud-js.git
cd crud-js
```

### 2. Install Dependencies
#### Backend
```sh
cd backend
npm install
```

#### Frontend
```sh
cd frontend
npm install
```

## ▶️ Menjalankan Aplikasi

### 1. Jalankan Backend
```sh
cd backend
npm start
```

### 2. Jalankan Frontend
```sh
cd frontend
npm start
```
Aplikasi akan berjalan di `http://localhost:3000/` (default React).

## 📂 Struktur Proyek
```
crud-js/
│── backend/
│   ├── config/          # Konfigurasi aplikasi
│   ├── controllers/     # Logika bisnis aplikasi
│   ├── models/         # Schema database
│   ├── routes/         # API routes
│   ├── node_modules/    # Dependensi backend
│   ├── package.json     # File konfigurasi npm
│   ├── package-lock.json
│   ├── request.rest     # File untuk testing API
│   ├── index.js         # File utama backend
│── frontend/
│   ├── public/         # Folder untuk aset statis
│   ├── src/
│   │   ├── components/  # Komponen React
│   │   ├── pages/       # Halaman aplikasi
│   │   ├── App.js       # Root component
│   ├── node_modules/    # Dependensi frontend
│   ├── package.json     # File konfigurasi npm
│   ├── package-lock.json
│   ├── .gitignore
│   ├── README.md
```

## 🗄 Database
Aplikasi ini menggunakan **MySQL** sebagai database.

### 📌 Struktur Tabel `users`
```sql
CREATE TABLE users (
    id INT(11) AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255) NOT NULL,
    email VARCHAR(255) NOT NULL,
    gender VARCHAR(255) NOT NULL,
    createdAt DATETIME NOT NULL,
    updatedAt DATETIME NOT NULL
);
```

### 🔧 Konfigurasi Koneksi Database
Buat file `.env` di dalam folder **backend** dan tambahkan konfigurasi berikut:
```env
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=
DB_NAME=crud_db
DB_PORT=3306
```

## 📡 API Endpoint
**Base URL:** `http://localhost:5000/api`

### 📍 Endpoint CRUD
| Method  | Endpoint       | Deskripsi             |
|---------|--------------|-----------------------|
| GET     | /users       | Mendapatkan semua data pengguna |
| GET     | /users/:id   | Mendapatkan data pengguna berdasarkan ID |
| POST    | /users       | Menambahkan pengguna baru |
| PUT     | /users/:id   | Mengupdate pengguna berdasarkan ID |
| DELETE  | /users/:id   | Menghapus pengguna berdasarkan ID |

## 💡 Kontribusi
1. Fork repository ini
2. Buat branch fitur baru (`git checkout -b fitur-baru`)
3. Commit perubahan (`git commit -m 'Menambahkan fitur baru'`)
4. Push ke branch (`git push origin fitur-baru`)
5. Buat pull request

## 📜 Lisensi
Proyek ini dilisensikan di bawah **MIT License**.

