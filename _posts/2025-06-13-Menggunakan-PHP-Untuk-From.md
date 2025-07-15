---
layout: post
title: "Langkah-Langkah Menggunakan PHP Untuk Form"
---

Langkah-Langkah Membuat Form dengan PHP
Berikut adalah panduan dasar membuat form HTML dan memprosesnya menggunakan PHP:

1.  Buat File HTML Form
Untuk Memproses Data
Misalnya proses.php:
php
Copy
Edit
<?php
  $nama = $_POST['nama'];
  $email = $_POST['email'];

  echo "Halo, $nama! Email kamu adalah $email.";
?>
3. Simpan Kedua File di Folder yang Sama
Pastikan kamu menyimpan form.html dan proses.php di direktori yang bisa dijalankan oleh server lokal seperti XAMPP, Laragon, atau MAMP.

4. Jalankan di Web Server Lokal
Jalankan http://localhost/foldermu/form.html di browser untuk melihat form.

Tips:

Gunakan isset() di PHP untuk validasi agar menghindari error saat data kosong.

Kamu juga bisa menggunakan file .php tunggal untuk form dan proses, jika ingin lebih praktis.
