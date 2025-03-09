# Praktikum TCC

## Tugas 4

Silakan deploy repository ini melalui Compute Engine. Repository ini merupakan sebuah implementasi Front-end sederhana dari praktik Back-end yang telah kita lakukan pada pertemuan 2 dan 3. Untuk Back-end **TIDAK PERLU** ikut di-deploy ke VM, cukup dijalankan secara local.

File Back-end dapat di-download melalui link ini:
https://github.com/plirapli/asisten-tcc-2-api-be

Sebelum mengikuti langkah-langkah di bawah, **pastikan teman-teman telah menjalankan server Back-End secara lokal terlebih dahulu**. Untuk caranya silakan ikuti instruksi yg terdapat pada README link di atas.

## How to deploy to VM:

- Lakukan update package pada instance VM dengan perintah `sudo apt update`
- Install web server apache dengan perintah `sudo apt install apache2`
- Clone/download repository ini pada instance VM dengan perintah `git clone https://github.com/plirapli/asisten-tcc-2-api-fe`
- Agar dapat men-download repository di atas, pastikan instance VM telah terinstall git terlebih dahulu. Jika belum, ketik `sudo apt install git`
- Jika repository telah di-download, copy seluruh isi file dari repository tersebut ke `/var/www/html/` dengan perintah `sudo cp -r asisten-tcc-2-api-fe/. /var/www/html/`
- Jalankan web dengan mengetikkan http://[EXTERNAL IP]
- Jika data sudah muncul, maka Front-End dan Back-End telah terhubung
