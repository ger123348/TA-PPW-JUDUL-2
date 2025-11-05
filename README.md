Website Portofolio – Gerhana Malik Ibrahim

Repository ini dibuat untuk memenuhi Tugas Akhir Percobaan 2: Git & Version Control
pada mata kuliah Praktikum Pemrograman Web, Teknik Informatika, Fakultas Teknik, Universitas Lampung.

Gerhana Malik Ibrahim (2315061032)

---

Cara Pembuatan

```bash
# Inisialisasi Git dan Konfigurasi Pengguna
git config --global user.name "Gerhana Malik Ibrahim"
git config --global user.email "gerhanamalikibrahim@gmail.com"

# Membuat folder proyek
mkdir TA-JUDUL-2
cd TA-JUDUL-2

# Inisialisasi repository Git
git init

# Commit awal (menambahkan file index.html)
git add index.html
git commit -m "Tambah index.html"

# Commit kedua (menambahkan style.css dan file pendukung)
git add .
git commit -m "Tambah style.css"

# Buat branch baru untuk menambahkan NPM
git branch feature-nim
git checkout feature-nim

# Lakukan perubahan pada index.html
git add .
git commit -m "Menambahkan NPM pada index.html"

# Kembali ke branch utama
git checkout master

# Gabungkan hasil perubahan dari branch feature-nim ke master
git merge feature-nim

# Hapus branch setelah merge
git branch -d feature-nim

# Hubungkan repository lokal dengan repository GitHub
git remote add origin https://github.com/ger123348/TA-PPW-JUDUL-2.git

# Push ke GitHub
git push -u origin master
```

---

Cara Penggunaan

1. Clone repository ini:

   ```bash
   git clone https://github.com/ger123348/TA-PPW-JUDUL-2.git
   ```

2. **Masuk ke direktori proyek:**

   ```bash
   cd TA-PPW-JUDUL-2
   ```

3. Buka file `index.html`:
   Klik dua kali file `index.html` di folder untuk membukanya di browser.

---

Branching dan Merging

Pengembangan fitur baru dilakukan melalui branch eksperimen (feature branch) agar tidak mengganggu versi utama.

- master → berisi versi stabil dari website portofolio.
- feature-nim → digunakan untuk menambahkan informasi NPM ke file index.html.

Setelah proses pengujian dan revisi selesai, branch `styling-nim` di-merge kembali ke `master` agar hasil akhirnya menjadi bagian dari versi utama proyek.
