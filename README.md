# Unit4.1_KeamananInformasi 

## 1. Analisis STEGO 
Praktikum dilakukan dengan analisis 2 gambar yang berbeda yaitu kuda dan pemandangan gunung berdasarkan referensi dari Elok. 
Steganografi merupakan teknik dalam menyembunyika suatu pesan rahasia (hiding message) agar keberadaan atau makna pesan tidak dapat terdeteksi oleh orang lain kecuali oleh pengirim dan penerima pesan. Terdapat tujuh teknik steganografi yaitu : 1) Injection 2) Substitution 3) Tranformasi Domain 4) Spread Spectrum 5) Statistical Method 6) Distortion 7) Cover Generation (Ariyus, 2009). Tujuan dari steganografi adalah merahasiakan atau menyembunyikan keberadaan dari sebuah pesan yang tersembunyi atau sebuah informasi. Steganografi dapat digunakan untuk berbagai alasan, seperti alasan baik ataupun sebaliknya “alasan tidak baik”.
## Penyelesaian analisis STEGO:
1. Mahasiswa melakukan download file stego 

![1](https://user-images.githubusercontent.com/99699435/224770471-cbe2b51a-bcde-4e38-b0f1-971eb3a48cb4.png)

2. Melakukan download file  MD5SUMS
 
![2](https://user-images.githubusercontent.com/99699435/224771219-e876fced-2ac7-4f77-9af0-4eaeb4bc1f2d.png) 

3. Membuat folder STEGO 

![3](https://user-images.githubusercontent.com/99699435/224771815-b40310c8-dbff-4b21-8035-23490bdc9968.png)
 
4. Menjalankan kedua gambar 
5. hasil command prompt 

![4](https://user-images.githubusercontent.com/99699435/224772254-d520ddb2-a8d1-4b06-b0ac-2e16d4acd3cd.png)
6. Analisis tabel kompresi gambar: 


![5](https://user-images.githubusercontent.com/99699435/224772847-e76d3b74-f45f-44bd-8f3d-84318a4abb17.png) 

Pada kedua gambar terlihat size mengalami perubahan, ketika di download dari elok dan se sudah di embed melalui STEGO. Terjadi perubahan yang signifikan pada ukuran hasil keluaran JPG, hal ini dapat terjadi setelah melalui proses steganografi yang disebabkan adanya penyususan bit dan struktur JPG yang tinggi pada tingkat error nya. Besarnya file JPG dikarenakan memanfaatkan metode kompresi dalam menjaga kualitas gambar dengan teknik redundansi data yang lebih sedikit. Dari data hasil Analisa diatas terlihat nilai faktor kompresi horses dan Everest memiliki nilai faktor kompresi yang tinggi, karena nilai horses dan Everest yang kecil berubah jauh lebih besar ketika terjadinya penyisipan pesan atau text. ukuran file stego (file yang berisi pesan tersembunyi) biasanya akan lebih besar daripada ukuran file cover (file yang digunakan untuk menyembunyikan pesan) karena pesan yang tersembunyi akan menambah ukuran file tersebut.  Dalam konteks steganografi, pesan tersembunyi dalam file stego mungkin memiliki pola atau struktur tertentu yang dapat dieksploitasi oleh algoritma kompresi untuk mengurangi ukuran file.

## 2. Analisis Log Server 
Log Server adalah file log yang dibuat dan dipelihara oleh server secara otomatis. Peringatan yang berisi daftar aktivitas yang dilakukan oleh server, seperti jumlah permintaan halaman, alamat IP klien, jenis permintaan dan lainnya.  File Log merupakan alat penting dalam memecahkan masalah dan pemantauan. Aplikasi yang berbeda menghasilkan file log yang berbeda, masing – masing berisi kumpulan bidang dan informasi sendiri. Secara struktur bidang dapat berubah di antara file log, alat yang digunakan untuk membacanya Sebagian besar sama. File Log merupakan file digunakan untuk merekam peristiwa tertentu untuk dihasilkan oleh aplikasi, layanan, atau sistem operasi itu sendiri

## Penyelesaian analisis Log Server
1. Membaca file log cat

![6](https://user-images.githubusercontent.com/99699435/224777296-01e54525-a9ab-4174-bfac-3baccb89ccec.png)


3. Membaca file log more
4. Membaca file log less
5. Membaca file log tail dan tail -f
6. Membaca file log dan syslog
7. Membuat daftar file syslog yang lebih lama 
8. Pemahaman file log dan journalctl
9. Menjalankan perintah journal --uct 
10. Menjalankan perintah journal -b
11. Penggunaan journalactl untuk menentukan layanan dan kerangkan waktu entri log
12. Menjalankan perintah journal -k 
13. Menjalankan perintah journal -f
