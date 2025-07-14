---
layout: post
title: "Belajar Menambahkan JavaScript pada Website"
---

Apa Itu JavaScript?

JavaScript adalah bahasa pemrograman yang digunakan untuk membuat website menjadi interaktif. Dengan JavaScript, kita bisa menambahkan berbagai fitur dinamis seperti validasi form, animasi, tombol interaktif, popup, dan lain-lain.

HTML dan CSS digunakan untuk struktur dan tampilan, sedangkan JavaScript digunakan untuk mengatur perilaku.

---

## Cara Menambahkan JavaScript ke Website

Ada tiga cara umum untuk menambahkan JavaScript ke dalam halaman HTML:

### 1. **Internal JavaScript**

Menulis kode JavaScript langsung di dalam file HTML, menggunakan tag `<script>` di bagian `<head>` atau sebelum penutup `</body>`:

```html
<!DOCTYPE html>
<html>
<head>
  <title>Contoh Internal JavaScript</title>
  <script>
   function sapaPengunjung() {
      alert("Selamat datang di websitemu!");
    }
  </script>
</head>
<body onload="sapaPengunjung()">
  <h1>Halo, Dunia!</h1>
</body>
</html>

2.Inline JavaScript
Menambahkan JavaScript langsung ke dalam atribut HTML, seperti contoh ini:

html
Copy
Edit
<button onclick="alert('Tombol diklik!')">Klik Saya</button>
3. External JavaScript
Menulis kode JavaScript di file terpisah (misalnya script.js) lalu dihubungkan ke HTML dengan tag <script>:

script.js

javascript
Copy
Edit
function halo() {
  alert("Hello dari file eksternal!");
}
index.html

html
Copy
Edit
<!DOCTYPE html>
<html>
<head>
  <title>Contoh External JS</title>
  <script src="script.js"></script>
</head>
<body>
  <button onclick="halo()">Klik Saya</button>
</body>
</html>
Tips Penggunaan JavaScript
Letakkan tag <script> sebelum </body> agar konten HTML termuat terlebih dahulu.

Gunakan file eksternal untuk menjaga kode lebih rapi dan terorganisir.

Untuk proyek besar, gunakan framework/library seperti React, Vue, atau jQuery jika dibutuhkan.

Kesimpulan
JavaScript adalah bagian penting dari pengembangan website modern. Dengan menambahkan JavaScript, kamu bisa mengubah website statis menjadi lebih hidup dan interaktif. Cobalah berbagai metode di atas untuk memahami cara kerja JavaScript pada website!