Array
Array dapat menyimpan data lebih dari satu tipe data, tipe data apapun bisa.
memangginya dengan nama-array[indeks-array]
Properti array :
.length untuk mengcek panjang indeks array.

Method array :
push untuk memasukan/menambahkan data/item pada indeks paling belakang pada array.
unshift untuk memasukan/menambahkan data/item pada indeks paling depan pada array.
pop untuk menghapus element terakhir.
shift untuk menghapus element paling awal(data pertama).
splice untuk mengubah konten didalam array dengan menghapus atau mengganti atau menambahkan data baru.
slice untuk memotong data.

Loop pada Array
menggunakan for basic.
contoh :
for(let i = buah.length - 1 ; i > 0 ; i--){
     console.log(buah[i])
 }

menggunakan for of.
for ( let bh of buah){
    console.log(bh)
}

menggunakan forEach, tanpa return.
menggunakan map, bisa dengan return.

Array multidimensi
array didalam array
contoh :
let arrMulti = [
    ["nama","alpha"], 	r1 0
    ["umur",17],	r2 1
    ["kelas","js"],	r3 2
]	c1	c2
	0	1
console.log(arrMulti[0][1])

Object

create object
Membuat objek
menambah objek dengan string bila ada spasi

create key
Menambahkan isi objek:
dengan dot operation
dengan bracket

Akses Objek
dengan cara dot notation, bracket, menampung dengan variabel

assign
mengganti properti objek
dengan dot
dengan bracket

delete objek

Method objek

nestedObjek
membuat Objek didalam Objek

loopObject

arrayOfObject

JavaScript modules
JSmodules adalah cara untuk memisahkan kode ke file yang berbeda 
keuntungan :
agar lebih mudah dikelola.
kode tidak menumpuk didalam 1 file.

Import JS,Export JS
pada html scrpit diberi type module

kurung kurawal digunakan untuk variabel yang menggunakan hanya keyword export saja
alternatif untuk melakukan export 
export {motor , smartPhone}
export default untuk melakukan eksport pada produk utama
export default di import tanpa kurung kurawal

pada export default karena hanya bisa satu jadi dapat diganti namanya saaat dipanggil(import)
script js yang dipasang (utama) tidak dapat melakukan export kedalam js yang lain
script js ke dua dapat melakukan import dari js ke-3 dan export ke js utama dan ke-3
script js ke-3 dapat melakukan export ke js utama dan ke-2 namun tidak bisa import sama sekali

recursive
fungsi yang memanggil dirinya sendiri
base case (titik paling kecil)

recursion case(titik dimana memanggil dirinya sendiri

Asynchronous

asinkron (asynchronous) adalah pemebelajaran yang dilakukan secara tunda

Singlethread dan multithread

bloking :thread yang lama tetap berjalanan dan non bloking : thread yang mempunyai durasi yang lama akan dijadikan prioritas terakhir
asinkron dapat me-non-bloking atau proses yang berjalan tidak berututan
sinkron dapat memblok atau proses yang berjalan sacara berurutan

proses settimeout : digunakan untuk menjeda waktu proses.
callback : fungsi yang dijadikan argumen

promise
resolve ke then
reject ke catch

Web Storage

web storage muncul pada di html5
html web storage lebih baik dari cookies

WEB API menjdai perantara yang memungkinkan orang luar dapat berkomunikasi dengan data kita.
js menjadi jembatan untuk web api

web storage disimpan untuk :
-preferensi user
-setting
-score pada game
-posisi video

Web storage Object:
-local : tidak ada tanggal kadaluarsa
-session : ada tanggal kadaluarsa

jangan digunakan untuk simpan data sensitif
