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

Perintah cat sendiri digunakan  untuk membuat, menggabungkan, atau menampilkan file di layar output standar atau ke file lain, dan banyak lagi. Menjawab pertanyaan dari uji coba pertama adalah sebagai berikut: Menggunakan cat dengan file teks besar memiliki beberapa kelemahan, di antaranya:
a. Memakan banyak memori
b.Tidak efisien untuk file besar
c. Tidak dapat mengedit isi file
d. Output terlalu banyak
e. Tidak fleksibel

2. Membaca file log more

![8](https://user-images.githubusercontent.com/99699435/224777435-be706e36-e474-4a67-ae88-5918c9c74934.png)

Dilihat dari fungsinya more digunakan untuk melihat isi suatu file dengan fasilitas melihat isi file dari atas. Dalam menjalankan perintah ini saya berhasil menjalankan pada terminal. Terdapat pertanyaan pada uji coba kedua ini, berikut pembahasan dari pertanyaannya: Meskipun more sangat berguna untuk membaca dan menampilkan isi file teks yang panjang, tetapi ada beberapa kelemahan penggunaan more, di antaranya:
a. Tidak efisien untuk navigasi mundur
b. idak fleksibel
c. Output terlalu banyak
d. Tidak dapat mengedit isi file

3. Membaca file log less

![9](https://user-images.githubusercontent.com/99699435/224777454-f4892996-4429-4284-bc36-bfa18612f6ff.png)

file sesuai dengan teori less adalah utilitas baris perintah yang menampilkan konten file atau output dari suatu perintah dalam satu halaman. Ini mirip dengan perintah more, tetapi memiliki fitur yang lebih maju dan memungkinkan Anda menavigasi maju dan mundur melalui file. Ketika dihubungkan dengan pertanyaan perintah cat tadi, perintah less yang banyak digunakan untuk membuka file yang lebih besar. 

4. Membaca file log tail dan tail -f

![10](https://user-images.githubusercontent.com/99699435/224777477-a1ac83db-0493-4b29-bdb0-4b33eb65fc42.png)

![11](https://user-images.githubusercontent.com/99699435/224777532-cf3e7c60-76a0-4dc6-9c8a-3da23ffdbdb0.png)

Pada analisis perbedaan output dari tal dan tail -f sebagai berikut: 
1.	Output tail: digunakan untuk menampilkan beberapa baris terakhir dari sebuah file teks. Ketika Anda menjalankan perintah tail, kita akan melihat isi file yang terakhir dibaca pada saat itu. Hal ini sesuai dengan data yang saya ambil pada terminal. 
2.	Output tail -f: Perintah tail -f memiliki arti yaitu: "follow" atau "mengikuti" digunakan utuk menampilkan isi file teks secara real-time. Ketika saya menjalankan perintah tail -f, saya akan melihat isi file yang sedang terus bertambah seiring dengan penambahan isi file tersebut. Perintah tail -f sangat berguna dalam memantau file log atau file yang terus diperbarui oleh aplikasi.
Dalam output tail -f, ketika ada perubahan pada file, maka perintah akan terus berjalan secara real-time dan akan menambahkan baris baru ke layar. Sedangkan pada output tail, saya harus menjalankan perintah kembali setiap kali ingin melihat isi file yang terbaru.

5. Membaca file log dan syslog

![12](https://user-images.githubusercontent.com/99699435/224777593-8854032e-61fc-4f29-ac7c-a8dbd3510133.png)

Analisis mengenai mengapa perintah cat harus dijalankan sebagai root, hal ini dikarenakan: Perintah cat tidak harus dijalankan sebagai root, karena perintah ini biasanya hanya digunakan untuk membaca isi file teks dan tidak memerlukan akses ke hak istimewa root. Namun, dalam beberapa kasus, cat harus dijalankan sebagai root, seperti:
a. Membaca file dengan hak akses terbatas
b. Mengakses file yang terletak di direktori sistem 
Namun, dalam kondisi umum, sebaiknya perintah cat dijalankan dengan hak akses pengguna biasa, kecuali jika ada kebutuhan tertentu untuk menggunakan hak akses root. Hal ini untuk menjaga keamanan sistem dan mencegah penggunaan hak akses root yang tidak perlu.

6. Membuat daftar file syslog yang lebih lama 

![13](https://user-images.githubusercontent.com/99699435/224777632-2add423d-43bb-4c2f-a720-f889200d2c84.png)

Percobaan ini hampir sama dengan sebelumnya perbedaannya hanya pada penggunakan perintah cat dalam membuat daftar file syslog yang lebih lama. Disini saya berhasil menjalankan perintah pada terminal dan mendapatkan output sesuai intruksi kerja. Analisis dari pertanyaan mengapa kita harus mengsinkronisasikan waktu dan tanggal komputer dengan benar adalah sebagai berikut: 
a.	Menjaga akurasi waktu
b.	Memudahkan manajemen jaringan
c.	Mencegah kegagalan sertifikat
d.	Mencegah kerentanan keamanan dapat mencegah serangan semacam ini.
Dengan demikian, mensinkronkan waktu dan tanggal pada komputer dengan benar sangat penting untuk memastikan akurasi waktu, kelancaran jaringan, keamanan, dan fungsi aplikasi.

7. Pemahaman file log dan journalctl

![14](https://user-images.githubusercontent.com/99699435/224777641-c8aea5ce-6902-4c39-97dc-4268b94fd7a8.png)

Perintah journalctl adalah utilitas yang digunakan untuk membaca log sistem di sistem operasi Linux yang menggunakan sistem logging journald. Dengan perintah ini, kita dapat membaca, menampilkan, dan menganalisis log sistem yang disimpan oleh journald. Beberapa penggunaan dari perintah journalctl adalah sebagai berikut:
a.Melihat log sistem secara keseluruhan
b.	Mencari log berdasarkan kriteria tertentu
c.	Menampilkan log dengan format yang berbeda
d.	Melihat log pada unit service tertentu
e.	Membaca log pada waktu tertentu
Perintah journalctl sangat berguna untuk menganalisis masalah sistem dan mencari tahu penyebab terjadinya masalah. Dengan perintah ini, kita dapat melihat log sistem dengan cara yang lebih terstruktur dan mudah dibaca. Namun, perintah ini hanya dapat digunakan pada sistem operasi Linux yang menggunakan journald sebagai sistem logging.

8. Menjalankan perintah journal --uct 

![15](https://user-images.githubusercontent.com/99699435/224777800-9bdc4b21-2a99-4393-903d-370e8e9db4d0.png)

Penggunaan perintah jorunalctl –utc adalah untuk menampilkan log sistem dalam waktu UTC (Coordinated Universal Time). UTC adalah standar waktu internasional yang digunakan sebagai referensi untuk mengukur waktu di seluruh dunia. Dengan menggunakan perintah journalctl --utc, waktu yang ditampilkan dalam log sistem akan disesuaikan dengan waktu UTC, sehingga memudahkan analisis log sistem dalam konteks waktu global.

9. Menjalankan perintah journal -b

![16](https://user-images.githubusercontent.com/99699435/224777804-11199a5e-d330-45b0-a4e2-44638558849f.png)

Perintah journalctl -b digunakan untuk menampilkan entri log dari sesi boot terakhir pada sistem Linux. Argumen -b menunjukkan bahwa kita ingin menampilkan log sesi boot terakhir, dan jika argumen tersebut tidak ditentukan, secara default akan menampilkan log untuk sesi saat ini. Ketika sistem Linux boot, jurnal sistem menyimpan semua entri log dalam sesi boot tersebut. Dengan menggunakan perintah journalctl -b, kita dapat menampilkan semua entri log yang dihasilkan selama sesi boot terakhir.

10. Penggunaan journalactl untuk menentukan layanan dan kerangkan waktu entri log

![17](https://user-images.githubusercontent.com/99699435/224777807-d504fa1c-8d49-417b-a446-9002f8ced92b.png)

Analisis dari uji coba ini adalah Perintah journalctl dapat digunakan untuk menentukan layanan dan kerangka waktu entri log dengan menggunakan beberapa argumen atau opsi. Dengan menggunakan argumen atau opsi ini, pengguna dapat menentukan layanan (dengan argumen -u) dan kerangka waktu (dengan opsi --since, --until, --since today, --since yesterday, atau --since "x time ago") untuk menampilkan entri log yang dibutuhkan. Disini saya menggunakan perintah analis@secOps ~$ sudo journalctl -u nginx.service –since today, yang berarti saya ingin menampilkan entri log untuk layanan tertentu dan menampilkan entri log yang terjadi hari ini.  

11. Menjalankan perintah journal -k 

![18](https://user-images.githubusercontent.com/99699435/224777810-8f1e1302-05a7-45ab-b15c-492b86d7b34b.png)

Perintah journalctl -k digunakan untuk menampilkan entri log dari kernel. Argumen -k menunjukkan bahwa kita ingin menampilkan log kernel, dan jika argumen tersebut tidak ditentukan, secara default akan menampilkan log untuk jurnal sistem. Ketika sistem Linux berjalan, kernel menghasilkan entri log yang sangat penting untuk memantau kinerja dan keamanan sistem. Dengan menggunakan perintah journalctl -k, kita dapat menampilkan semua entri log yang dihasilkan oleh kernel sejak sistem dimulai. 

12. Menjalankan perintah journal -f

![19](https://user-images.githubusercontent.com/99699435/224777812-3d407368-bfb2-47cd-93d1-a7e490d03f5b.png)

Perintah journalctl -f digunakan untuk memantau secara langsung entri log yang baru dibuat pada sistem Linux. Argumen -f menunjukkan bahwa kita ingin memantau entri log secara langsung (real-time), dan jika argumen tersebut tidak ditentukan, secara default akan menampilkan seluruh entri log dalam jurnal sistem.

Ketika kita menjalankan perintah journalctl -f, terminal akan menampilkan entri log baru yang muncul pada jurnal sistem secara langsung. Ini dapat sangat berguna untuk memantau aktivitas sistem secara real-time. 
