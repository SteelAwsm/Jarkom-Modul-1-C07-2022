# Jarkom-Modul-1-C07-2022

laporan resmi Praktikum Jaringan Komputer Modul 1 tahun 2022

Anggota Kelompok C07 :
* 5025201274 - Alif Adrian Anzary
* 5025201122 - Marsyavero Charisyah Putra
* 5025201209 - Hemakesha Ramadhani Heriqbaldi

## 1. Sebutkan web server yang digunakan pada "monta.if.its.ac.id"! 
## 2. Ishaq sedang bingung mencari topik ta untuk semester ini , lalu ia datang ke website monta dan menemukan detail topik pada website “monta.if.its.ac.id” , judul TA apa yang dibuka oleh ishaq ?
![image](https://user-images.githubusercontent.com/72655925/192094694-3a2e2a2f-f449-43f2-a9bb-c95b2cb0c1cf.png)
<br>Penjelasan :
<br>Menggunakan display filter : http contains topik
![image](https://user-images.githubusercontent.com/72655925/192094790-4ae8ef76-e436-4cde-9ffc-74f57222f294.png)
<br>Meng-export file 194 karena memiliki path /topik/detailTopik/194
![image](https://user-images.githubusercontent.com/72655925/192094987-61c34bb8-585b-4e4a-888c-396637ce61af.png)
<br>Menjalankan file 194.html dan akan menampilkan page Detail Topik yang dibuka Ishaq
![image](https://user-images.githubusercontent.com/72655925/192095040-bbaf9641-ebef-4317-8987-0e6e457d4572.png)


## 3. Filter sehingga wireshark hanya menampilkan paket yang menuju port 80! 
## 4. Filter sehingga wireshark hanya mengambil paket yang berasal dari port 21!
## 5. Filter sehingga wireshark hanya mengambil paket yang berasal dari port 443!
<img src="img/5-1.png">
Penjelasan :
<br>
Menggunakan display filter : tcp.srcport == 443


## 6. Filter sehingga wireshark hanya menampilkan paket yang menuju ke lipi.go.id !

<img src="img/6-1.png">
Penjelasan :
<br>
Mengambil ip dari website lipi.go.id menggunakan ping di dalam cmd
<img src="img/6-2.png">
Lalu menggunakan ip address website lipi.go.id (203.160.128.158) untuk display filter : ip.dst == 203.160.128.158

## 7. Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!
<img src="img/7-1.png">
<img src="img/7-2.png">
<img src="img/7-3.png">
<img src="img/7-4.png">
Penjelasan :
<br>
Penjelasan:
Mendapatkan Ip address pribadi dengan :
Membuka Settings -> Network & Internet -> WIFI -> pilih network WIFI yang telah terkoneksi -> properties -> Ip address tertulis di sebelah IPv4 Address. Setelah mendapatkan IP Address, IP address digunakan sebagai capture filter dengan syntax : Src host [IP Address pribadi]



## 8. Telusuri aliran paket dalam file .pcap yang diberikan, cari informasi berguna berupa percakapan antara dua mahasiswa terkait tindakan kecurangan pada kegiatan praktikum. Percakapan tersebut dilaporkan menggunakan protokol jaringan dengan tingkat keandalan yang tinggi dalam pertukaran datanya sehingga kalian perlu menerapkan filter dengan protokol yang tersebut.
Jawaban:
![image](https://user-images.githubusercontent.com/72655925/192096550-49c63410-7b90-4d7a-ba8f-db54481f4ebd.png)
Penjelasan:
<br>Cari dulu file dengan ip.addr == 127.0.0.1, lalu di TCP Stream salah satu paket. Untuk total chattingan yang dilakukan terdapat 3 chattingan yang ditemukan untuk tiap stream pada beberapa paket yang berbeda.
## 9. Terdapat laporan adanya pertukaran file yang dilakukan oleh kedua mahasiswa dalam percakapan yang diperoleh, carilah file yang dimaksud! Untuk memudahkan laporan kepada atasan, beri nama file yang ditemukan dengan format [nama_kelompok].des3 dan simpan output file dengan nama “flag.txt”.
## 10. Temukan password rahasia (flag) dari organisasi bawah tanah yang disebutkan di atas!
