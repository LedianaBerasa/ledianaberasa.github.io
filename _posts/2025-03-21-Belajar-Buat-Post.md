---
layout: post
title: "Belajar Buat Post"

---
 Kamu sudah membuat post Jekyll dengan format yang benar secara dasar, tapi masih sangat minimalis. Supaya post kamu tampil rapi di halaman blog Jekyll, berikut adalah penjelasan dan contoh template post yang bisa kamu gunakan.

✅ 1. Struktur File Post Jekyll
File post harus disimpan di folder:

Salin
Edit
_posts/
Dan nama file harus mengikuti format:

css
Salin
Edit
YYYY-MM-DD-nama-post.md
Contoh nama file:

yaml
Salin
Edit
2025-07-03-belajar-buat-post.md
✅ 2. Isi File Markdown Post
Berikut contoh konten post yang baik:

markdown
Salin
Edit
---
layout: post
title: "Belajar Buat Post di Jekyll"
date: 2025-07-03 12:00:00 +0700
author: Lediana Berasa
categories: [tutorial, jekyll]
tags: [jekyll, blog, markdown]
---

Halo! 👋

Ini adalah post pertama saya menggunakan **Jekyll**.

Di post ini saya belajar:
- Cara membuat file markdown untuk blog
- Struktur front matter
- Menyimpan file di folder `_posts`

Semoga postingan ini bermanfaat bagi yang ingin belajar Jekyll!
✅ 3. Pastikan File Tersimpan di Folder _posts
Letakkan file markdown (.md) tersebut di:

bash
Salin
Edit
/_posts/2025-07-03-belajar-buat-post.md
✅ 4. Jalankan Website
Kalau kamu ingin melihat hasilnya di browser:

bash
Salin
Edit
bundle exec jekyll serve
Lalu buka:
📍 http://localhost:4000/blog/
(jika blog kamu sudah diatur di blog.html, atau langsung dari halaman utama)

🔧 Kalau Belum Ada Halaman Blog:
Buat file blog.html di root folder (satu folder dengan index.html) dengan isi:

html
Salin
Edit
---
layout: default
title: Blog
---

<h1>Blog</h1>
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span>{{ post.date | date: "%d %B %Y" }}</span>
    </li>
  {% endfor %}
</ul>