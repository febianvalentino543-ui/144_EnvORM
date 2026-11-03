# 📚 Komik CRUD API
 
REST API sederhana untuk operasi **CRUD** (Create, Read, Update, Delete) data komik menggunakan **Express.js**, **Sequelize ORM**, dan **PostgreSQL**.
 
## 🛠️ Teknologi
- Node.js & Express.js
- PostgreSQL
- Sequelize (ORM)
- dotenv
- Postman (pengujian API)
## 🗄️ Struktur Tabel `komik`
 
| Kolom       | Tipe Data | Keterangan                  |
|-------------|-----------|-----------------------------|
| id          | INTEGER   | Primary Key, Auto Increment |
| title       | STRING    | Judul komik (wajib)         |
| description | TEXT      | Deskripsi komik             |
| author      | STRING    | Pengarang (wajib)           |

## 🔗 Endpoint API
 
| Method | Endpoint     | Fungsi                  |
|--------|--------------|-------------------------|
| GET    | `/komik`     | Mengambil semua komik   |
| GET    | `/komik/:id` | Mengambil komik per ID  |
| POST   | `/komik`     | Menambah komik baru     |
| PUT    | `/komik/:id` | Mengubah data komik     |
| DELETE | `/komik/:id` | Menghapus komik         |
 
Contoh body (JSON) untuk **POST** / **PUT**:
```json
{
  "title": "One Piece",
  "description": "Petualangan Monkey D. Luffy mencari harta karun One Piece",
  "author": "Eiichiro Oda"
}
```
 
## 📸 Hasil Pengujian di Postman
 
### 1. POST - Menambah Data
<img width="3000" height="1876" alt="GET" src="https://github.com/user-attachments/assets/bd3bc9f7-020c-4e99-851e-c834e707f141" />

### 2. DELETE - Menghapus Data
<img width="3000" height="1874" alt="POST" src="https://github.com/user-attachments/assets/a4052cf3-4690-4c50-b9f0-49279e9e7188" />

### 3. GET - Mengambil Data
<img width="3000" height="1876" alt="PUT" src="https://github.com/user-attachments/assets/75b26096-582c-4d3f-b68c-d26d9b13214e" />

### 4. PUT - Mengubah Data
<img width="3000" height="1876" alt="DELETE" src="https://github.com/user-attachments/assets/42d55ac6-016e-4af3-ab6c-2fc443fa5649" />
