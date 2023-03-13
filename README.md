# Unit4.1_KeamananInformasi 

## 1. Analisis STEGO 
Praktikum dilakukan dengan analisis 2 gambar yang berbeda yaitu kuda dan pemandangan gunung berdasarkan referensi dari Elok. 
## Penyelesaian dan Analisis STEGO:
1. mahasiswa melakukan download file stego 

![1](https://user-images.githubusercontent.com/99699435/224770471-cbe2b51a-bcde-4e38-b0f1-971eb3a48cb4.png)

2. melakukan download file  MD5SUMS
 
![2](https://user-images.githubusercontent.com/99699435/224771219-e876fced-2ac7-4f77-9af0-4eaeb4bc1f2d.png) 

3. membuat folder STEGO 

![3](https://user-images.githubusercontent.com/99699435/224771815-b40310c8-dbff-4b21-8035-23490bdc9968.png)
 
4. menjalankan kedua gambar 
5. hasil command prompt 

![4](https://user-images.githubusercontent.com/99699435/224772254-d520ddb2-a8d1-4b06-b0ac-2e16d4acd3cd.png)
6. analisis tabel kompresi gambar: 


![5](https://user-images.githubusercontent.com/99699435/224772847-e76d3b74-f45f-44bd-8f3d-84318a4abb17.png) 

Pada kedua gambar terlihat size mengalami perubahan, ketika di download dari elok dan se sudah di embed melalui STEGO. Terjadi perubahan yang signifikan pada ukuran hasil keluaran JPG, hal ini dapat terjadi setelah melalui proses steganografi yang disebabkan adanya penyususan bit dan struktur JPG yang tinggi pada tingkat error nya. Besarnya file JPG dikarenakan memanfaatkan metode kompresi dalam menjaga kualitas gambar dengan teknik redundansi data yang lebih sedikit. Dari data hasil Analisa diatas terlihat nilai faktor kompresi horses dan Everest memiliki nilai faktor kompresi yang tinggi, karena nilai horses dan Everest yang kecil berubah jauh lebih besar ketika terjadinya penyisipan pesan atau text. ukuran file stego (file yang berisi pesan tersembunyi) biasanya akan lebih besar daripada ukuran file cover (file yang digunakan untuk menyembunyikan pesan) karena pesan yang tersembunyi akan menambah ukuran file tersebut.  Dalam konteks steganografi, pesan tersembunyi dalam file stego mungkin memiliki pola atau struktur tertentu yang dapat dieksploitasi oleh algoritma kompresi untuk mengurangi ukuran file.
