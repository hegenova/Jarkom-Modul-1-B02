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
