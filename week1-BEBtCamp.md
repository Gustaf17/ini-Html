Web Server & REsTful API
======================================================================================================================
Web server adalah tempat untuk menaruh file website.

Dynamic site/server side render full dilakukan didalam server, terdapat 2 opsi ada html atau json

RESTAPI
=========================================================
Representational State Transfer salah satu arsitektur design untuk membuat web services

rules :
1.Uniform interface
2.Client-server
3.stateless
4.cacheable
5.Layered System
6.Code on demand(optional)
API yg menerapkan rules diatas disebut RESTful API

HTTP method			sTATUS code :
-GET				    -2xx - success
-POST				    -3xx - redirect
-DELETE				  -4xx - client error
-PUT/PATCH			-5xx - server error

thunder client / postman untuk mengetes API

Node.js
Node.js itu secara sederhananya, merupakan platform JavaScript yang dapat berjalan di backend atau server-side, di komputer kita secara langsung.
Runtime adalah tempat untuk menjalankan atau mengesekusi kode ktia.
Yang menyebabkan js bisa berjalan dibrowser salah satuya v8 engine.

main feature
1. file system
2. http & https
3. REPS (Read, Eval, Print, Loop)
4. Console

node.js membuat web service yang bisa menerima data request dan response.

build in module Node JS
console 
proses 
util 
fs

node -v untuk mengecek versi node js
node (nama file) untuk menjalankan log di terminal
npm install
npm init
npm run "test"

process
console
os
fs
event
util

Node JS web server
Node.js memiliki built-in modul yang disebut HTTP
Untuk menggunakan modul HTTP, gunakan require()


Gunakan method createServer() untuk membuat server HTTP


Callback function yang digunakan pada method http.createServer(), akan dijalankan ketika seseorang mencoba mengakses komputer pada port 8080.

https://en.wikipedia.org/wiki/List_of_TCP_and_UDP_port_numbers  mengecek status code


Express JS
middleware merupakan jembatan yang menjadi penengah antara request dengan express

Express.js, atau hanya Express, adalah kerangka aplikasi web back end untuk Node.js, dirilis sebagai open-source software dan gratis di bawah Lisensi MIT. Ini dirancang untuk membangun aplikasi web dan API. Express telah disebut sebagai kerangka kerja server standar de facto untuk Node.js.

Back end app adalah aplikasi yang berjalan di server-side yang bekerja untuk memberikan informasi berupa data sesuai request dari client / browser / front end app. Umumnya server-side app membuat REST API

REST (Representional State Transfer) adalah sebuah arsitektur metode komunikasi yang menggunakan protokol HTTP untuk pertukaran data dimana metode ini sering diterapkan dalam pengembangan aplikasi.

RESTFUL API memiliki 4 komponen penting yaitu:

URL Design
HTTP Verbs
HTTP Response Code
Format Response

Routes adalah sebuah end point yang diapat kita akses menggunakan URL di website. Didalam routes kita perlu menentukan method API, alamat dan response apa saja yang akan dikeluarkan

Method
Kita dapat menggunakan method yang dalam REST API seperti POST, PUT, PATCH dan DELETE

Di dalam route kita dapat mengirim response menggunakan parameter dari route express.js yaitu “res.Send()” untuk mengirim plain text ketika kita mengakses route tersebut.

Dalam pengaplikasian back end application, kita sangat perlu memberikan status code sebagai informasi apakah route yang kita akses berjalan sebagaimana mestinya dan tidak terjadi error.

Nested route digunakan ketika terdapat banyak route yang memiliki nama yang sama atau ingin membuat route yang lebih mendalam


Middleware
Middleware function adalah sebuah fungsi yang memiliki akses ke object request (req), object response (res), dan sebuah fungsi next didalam request-response cycle.
Fungsi next biasanya di berikan nama variable next.


Review Materi Express JS
routing
controller

Desain databse dengan MySQL

ERD
Entity Relation Diagram
contoh :

user dapat megikuti mata kuliah
   1			m
[User] <mengikuti> [matakuliah]

matakuliah diikuti user
	1		m
[matakuliah] <diikuti> [User]
	m		m
[matakuliah] <diikuti> [User]

Class Diagram
  
 Normalisasi Database

Normalisasi database adalah proses pengelompokan atribut data yang membentuk entitas sederhana, nonredundant, fleksibel, dan mudah beradaptasi. Sehingga dapat dipastikan bahwa database yang dibuat berkualitas baik.

Tujuan utama dari normalisasi database adalah:

Menghilangkan dan mengurangi redudansi data.
Memastikan dependensi data (data berada pada tabel yang tepat).
Jika sebuah database belum dinormalisasi, kemungkinan terburuk yang akan merugikan sistem adalah:

INSERT Anomali
Situasi dimana tidak memungkinkan untuk memasukkan beberapa jenis data secara langsung di database.
UPDATE Anomali
Situasi dimana nilai yang diubah mengakibatkan ketidakkonsistenan database, artinya data yang diubah tidak sesuai dengan yang diinginkan.
DELETE Anomali
Penghapusan data tidak sesuai yang diharapkan, artinya data yang seharusnya tidak terhapus malah terhapus.

Database Seperti Apa Yang Bisa Dinormalisasi?
Tidak semua database bisa dinormalisasi, hanya tipe “relational database” yang bisa dinormalisasi. Banyak vendor DBMS (Database Management System) diantaranya Oracle, MySQL, SQL Server, PostgreSQL, dll.

Bagaimana Cara Melakukan Normalisasi Database?

1NF
Inti dari normalisasi 1NF adalah tidak boleh ada grouping data ataupun duplikasi data. Sekarang lanjut pada tahap normalisasi 2NF.

2NF
Syarat 2NF adalah tidak diperkenankan adanya partial “functional dependency” kepada primary key dalam sebuah tabel.

Apa itu “functional dependency”?

Functional dependency adalah setiap atribut yang bukan kunci (non key) bergantung secara fungsional terhadap primary key.

Intinya adalah pada tahap normalisasi 2NF ini tabel tersebut harus dipecah berdasarkan primary key.

3NF
Pada 3NF tidak diperkenankan adanya partial “transitive dependency” dalam sebuah tabel.

Apa itu “transitive dependency”? Transitive dependency biasanya terjadi pada tabel hasil relasi, atau kondisi dimana terdapat tiga atribut A, B, C. Kondisinya adalah A ⇒ B dan B ⇒ C. Maka C dikatakan sebagai transitive dependency terhadap A melalui B.

Intinya pada 3NF ini, jika terdapat suatu atribut yang tidak bergantung pada primary key tapi bergantung pada field yang lain maka atribut-atribut tersebut perlu dipisah ke tabel baru.
