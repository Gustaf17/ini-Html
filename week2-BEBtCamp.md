Backend Development

Backend adalah teknologi yang berjalan di sisi server dari sebuah perangkat lunak.

Server
Server adalah sebuah wadah atau jaringan komputer yang berguna untuk pelayanan tertentu untuk perangkat komputer lain.

databases 
Database dapat diartikan sebagai kumpulan data yang disimpan didalam wadah.

API
API adalah intruksi - intruksi yang digunakan untuk membuat software

REST API bertugas sebagai perantara antara frontend dan backend (jembatan), dimana terdapat request dan response.

DBMS
software yang digunakan untuk mengoprasikan data yang ada didalam database

Table
kumpulan data berupa baris dan kolom.

Field
Adalah sebuah kolom dari sebuah tabel.

Record
Adalah sebuah value dari suatu kolom biasanya dijabarkan dalam bentuk baris.

SQL adalah bahasa query yang digunakan untuk melakukan interaksi di Database.

DDL		DML		DCL
Alter		select		Grant
DROP		INsert		Revoke
		Update
		Delete

Primary Key : Kunci primer atau kunci utama sebagai identifikasi yang membedakan suatu baris pada tabel.
Foreign Key : Primary key dari tabel luar yang berada di tabel yang lain.

Inner join menampilkan data yang memunyai relasi saja(irisan).

right join melakukan irisan dan menampilkan semua data dari tabel kanan. 
left join melakukan irisan dan menampilkan semua data dari tabel kiri.

fungsi agregat
avg untuk average atau rata-rata
sum untuk penjumlahan
max untuk nilai maximum

Authorization & Authentication

Author.... kepemilikan akses
Authen.... Pengecekan atau verifikasi identitas atas kepemilikan hak akses

Enkripsi
Enkripsi adalah proses teknis yang mengonversikan informasi menjadi kode rahasia, sehingga mengaburkan data yang dikirim, diterima, atau disimpan. Pada dasarnya, sebuah algoritma digunakan untuk mengacak data, sebelum pihak penerima memulihkan kembali data yang diacak tersebut menggunakan kunci dekripsi.

Sequelize
merupakan ORM nodejs berbasis promise.

ORM merupakan metode yang memudahkan kita dalam bermain dengan database kita, seperti mengoprasikannya hanya dengan method saja tidak dengan query.


cek globally installed packages
npm list -g --depth 0

install sequelize cli globally
npm i -g sequelize-cli

install in local project
npm install sequelize

init sequelize in local project
npx sequelize-cli init
