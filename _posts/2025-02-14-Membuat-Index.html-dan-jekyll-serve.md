---
layout: post
title: "Membuat Index.html dan jekyll serve"

---
1. Buat Proyek Jekyll Baru
bash
Salin
Edit
jekyll new myblog
cd myblog
Folder myblog akan berisi struktur proyek Jekyll dengan file dan folder default.

2. Ganti index.markdown Menjadi index.html (Opsional)
Secara default, jekyll new membuat index.markdown. Jika kamu ingin memakai index.html, lakukan:

Hapus index.markdown:

bash
Salin
Edit
rm index.markdown
Buat file baru:

html
Salin
Edit
<!-- index.html -->
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>Halaman Utama</title>
</head>
<body>
  <h1>Selamat datang di situs Jekyll saya!</h1>
  <p>Ini adalah halaman index.html custom.</p>
</body>
</html>
Simpan file ini di direktori root proyek (myblog/index.html).

3. Jalankan jekyll serve
Pastikan kamu ada di folder proyek, lalu jalankan:

bash
Salin
Edit
bundle exec jekyll serve
Atau jika tidak menggunakan bundler:

bash
Salin
Edit
jekyll serve
4. Akses Website
Buka browser dan kunjungi:

arduino
Salin
Edit
http://localhost:4000
Kamu akan melihat konten dari index.html.

📝 Tips Tambahan
Jika kamu ingin memakai layout Jekyll, pastikan index.html punya front matter:

html
Salin
Edit
---
layout: default
title: Beranda
---

<h1>Halo dunia!</h1>
File layout default ada di _layouts/default.html.

