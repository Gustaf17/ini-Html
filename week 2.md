Javascript Scope
Scope adalah konsep dalam flow data variabel. 
Menentukan suatu variabel bisa diakses pada scope tertentu atau tidak.

Blocks
Blocks adalah code yang berada didalam curly braces {}.

Global Scope
Global scope berarti variabel yang kita buat dapat diakses dimanapun dalam suatu file.

Local Scope
Local scope berarti kita mendeklarasikan variabel didalam blocks seperti function, conditional, dan looping.


JAVASCRIPT - FUNCTION
Function adalah sebuah blok kode dalam sebuah grup untuk menyelesaikan 1 task/1 fitur.
Manfaatnya adalah kita dapat menggunakan ulang code yang telah dibuat.

Membuat - memanggil fungsi

Parameter dan Argumen
Dengan parameter, function dapat menerima sebuah inputan data dan menggunakannya untuk melakukan task/tugas.

Argumen adalah nilai yang digunakan saat memanggil function.
Jumlah argumen harus sama dengan jumlah parameternya

Default Parameters
Default paramaters digunakan untuk memberikan nilai awal/default pada parameter function.

Data Type Built in Prototype & Method

JavaScript types

Primitive values
-Boolean type
Boolean mewakili entitas logis dan dapat memiliki dua nilai: benar dan salah

-Null type
Tipe Null memiliki tepat satu nilai: null

-Undefined type
Variabel yang belum diberi nilai memiliki nilai yang tidak terdefinisi(undefined)

-Number type

-BigInt type
BigInt adalah tipe data primitif numeric dalam JavaScript yang dapat mewakili bilangan bulat dengan presisi arbitrer(penengah).

-String type
Jenis JavaScript String digunakan untuk mewakili data tekstual.

-Objects
Dalam JavaScript, objek dapat dilihat sebagai kumpulan properti.

typeof untuk mengecek tipe data sebuah value.

properti lenght digunakan untuk mengecek panjang karakter/array.

method string toUpperCase untuk membuat value string menjadi kapital.
method string toLowerCase untuk membuat value string menjadi kecil.

charAt metode mengembalikan karakter pada indeks tertentu dalam sebuah string.

includes metode untuk mencari karakter atau string di dalam string.

method isNaN untuk mengecek itu adalah number atau bukan.
method toString untuk mengubah number menjadi string.
toFixed method yang mirip dengan toString.

parseInt dan parseFloat digunakan untuk mengubah string menjadi number.

DOM HTML
DOM (Document Object Model) adalah sebuah API yang menyediakan fungsi-fungsi untuk memanipulasi dokumen.
Objek dari dokumen ini menyediakan sekumpulan fungsi dan atribut/data yang bisa kita manfaatkan dalam membuat program Javascript. Inilah yang disebut API (Application Programming Interface).

salah satu cara mengakses elemen HTML adalah dengan DOM document.getElementByID untuk mengambil isi dokumen dengan id.
document.getElementsByClass untuk mengambil isi dokumen dengan kelas.
Mengakses elemennya dengan indeks untuk getElementsByClass. contoh memanggil : console.log(item[2])
getElementByTag mengakses isi dokumen dengan tag name, cara aksesnya mirip seperti array. Dan 
querySelector 

DOM manipulasi
innerHTML
innerHTML adalah sebuah atribut di dalam (objek) elemen HTML yang berisi string HTML. Dengan innerHTML , kita dapat menampilkan output ke elemen yang lebih spesifik.

innerText
innerText fungsinya adalah untuk menentukan dan mengembalikan nilai konten dari suatu element dalam bentuk text atau string

createElement
append dan appendchild (hanya bisa menyisipkan sebuah node)
remove

DOM event  
html atribute
event property
addEventListener
