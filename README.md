# PRAKTIKUM JARKOM 1
```
Anggota :

	Muhammad Daffa Aldriantama (5025201177)
	Burhanudin Rifa (5025201191)
	Maisan Auliya (5025201137)

```
## 1.  Sebutkan web server yang digunakan pada "monta.if.its.ac.id"! 
* buka monta.if.its.ac.id
* lalu filter http
* pilih salah satu
* lalu cek servernya
* servernya nginx/1.10.3
![Alt text](/image/Jarkom1-1.png)
## 2. Ishaq sedang bingung mencari topik ta untuk semester ini , lalu ia datang ke website monta dan menemukan detail topik pada website “monta.if.its.ac.id” , judul TA apa yang dibuka oleh ishaq ?
* export object (http)
* pilih yang file name nya 194
* lalu buka di file
* terlihat topik TA nya
![Alt text](/image/Jarkom1-2.png)
![Alt text](/image/Jarkom1-2a.png)
![Alt text](/image/Jarkom1-2b.png)
![Alt text](/image/Jarkom1-2c.png)
## 3. Filter sehingga wireshark hanya menampilkan paket yang menuju port 80! 
* menggunakan tcp.dstport == 80
![Alt text](/image/Jarkom1-3.png)
## 4. Filter sehingga wireshark hanya mengambil paket yang berasal dari port 21!
* Untuk mengambil paket yang berasal dari port 21, kita dapat menggunakan sintaks berikut di dalam display filters
![Alt text](/image/Jarkom1-4.png)
## 5. Filter sehingga wireshark hanya mengambil paket yang berasal dari port 443!
* Tidak jauh berbeda dengan nomor sebelumnya, Untuk mengambil paket yang berasal dari port 443, kita dapat menggunakan sintaks berikut di dalam display filters.
![Alt text](/image/Jarkom1-5.png)
## 6. Filter sehingga wireshark hanya menampilkan paket yang menuju ke lipi.go.id!
* Hal yang pertama kali dilakukan adalah menulis sintaks berikut di dalam display filter.
![Alt text](/image/Jarkom1-6.png)
* Hasil dari display filters adalah sebagai berikut:
![Alt text](/image/Jarkom1-6a.png)
* Kemudian, ditemukan bahwa IP dari lipi.go.id adalah 203.160.128.158. 
<br></br>
* Kita dapat menampilkan paket yang menuju ke lipi.go.id dengan menggunakan IP yang ditemukan dan sintaks berikut di display filters. 
![Alt text](/image/Jarkom1-6b.png)
* Hasil dari filter adalah sebagai berikut:
![Alt text](/image/Jarkom1-6c.png)
## 7. Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!
* Dapatkan alamat ip kita sendiri, karena saya memakai mac jadi alamat ipnya otomatis tersedia pada System Preferences -> Networks
![Alt text](/image/Jarkom1-7.png)
* Lalu filter wireshark src host dan masukkan alamat ip
![Alt text](/image/Jarkom1-7a.png)
## 8. Telusuri aliran paket dalam file .pcap yang diberikan, cari informasi berguna berupa percakapan antara dua mahasiswa terkait tindakan kecurangan pada kegiatan praktikum. Percakapan tersebut dilaporkan menggunakan protokol jaringan dengan tingkat keandalan yang tinggi dalam pertukaran datanya sehingga kalian perlu menerapkan filter dengan protokol yang tersebut.
* karena dalam teka teki nya membicarakan tentang kecurangan tentang jawaban, maka keyword yang didapat yaitu “jawaban”
* menggunakan tcp contains berdasarkan keyword
* follow salah satu paket
* kemudian TCP stream
![Alt text](/image/Jarkom1-8.png)
![Alt text](/image/Jarkom1-8a.png)
![Alt text](/image/Jarkom1-8b.png)
## 9. Terdapat laporan adanya pertukaran file yang dilakukan oleh kedua mahasiswa dalam percakapan yang diperoleh, carilah file yang dimaksud! Untuk memudahkan laporan kepada atasan, beri nama file yang ditemukan dengan format [nama_kelompok].des3 dan simpan output file dengan nama “flag.txt”.
* dari percakapan pada no.8, didapatkan kode 9002
* gunakan tcp.srcport == 9002
* follow salah satu paket
* save as
* lalu rename sesuai ketentuan soal
* gunakan openssl dengan output flag.txt
![Alt text](/image/Jarkom1-9.png)
![Alt text](/image/Jarkom1-9a.png)
![Alt text](/image/Jarkom1-9b.png)
![Alt text](/image/Jarkom1-9c.png)
![Alt text](/image/Jarkom1-9d.png)
![Alt text](/image/Jarkom1-9e.png)
## 10. Temukan password rahasia (flag) dari organisasi bawah tanah yang disebutkan di atas!
* berdasarkan teka teki, didapatkan password : “nakano”
* buka file flag.txt
![Alt text](/image/Jarkom1-10.png)
