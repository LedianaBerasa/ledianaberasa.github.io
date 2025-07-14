---
layout: post
title: "Belajar Menambahkan ke Folder Student"
categories: student
---

Pendahuluan

Dalam proyek Jekyll, kita bisa mengelompokkan postingan berdasarkan kategori, seperti `student`, agar lebih terstruktur dan mudah diatur. Pada artikel ini, kita akan mempelajari cara **menambahkan postingan ke folder `student`** dengan benar.

---

Langkah-langkah Menambahkan Postingan ke Folder `student`

1. Buat Folder `student` di Dalam `_posts`

Pastikan kamu memiliki folder bernama `student` di dalam folder `_posts`. Jika belum, buat secara manual atau dengan perintah terminal berikut:

```bash
mkdir -p _posts/student

2. Buat File Postingan Markdown
Gunakan format nama file: YYYY-MM-DD-nama-post.md. Contoh:

bash
Copy
Edit
_posts/student/2025-07-14-belajar-menambahkan-javascript-pada-website.md

3. Isi File dengan Front Matter dan Konten
Berikut adalah contoh isi file:

markdown
Copy
Edit
---
layout: post
title: "Belajar Menambahkan JavaScript pada Website"
categories: student
---

## Apa Itu JavaScript?

(JavaScript adalah bahasa pemrograman untuk membuat website interaktif...)

## Cara Menambahkan

(Contoh: internal, inline, external...)

4. Jalankan Server Jekyll
Gunakan perintah berikut di terminal untuk melihat hasilnya:

bash
Copy
Edit
bundle exec jekyll serve
Kemudian buka di browser:

arduino
Copy
Edit
http://localhost:4000
Bonus: Tampilkan Semua Postingan student
Jika ingin membuat halaman khusus yang menampilkan semua artikel dalam kategori student, buat file student.html:

html
Copy
Edit
---
layout: default
title: Kategori Student
---

<h1>Postingan Kategori Student</h1>
<ul>
  {% for post in site.categories.student %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
Kesimpulan
Dengan menggunakan folder student, kamu dapat mengelompokkan postingan dan membuat struktur blog yang rapi. Ini sangat berguna untuk situs edukasi, tugas kuliah, atau proyek kelompok.

Selamat mencoba!
