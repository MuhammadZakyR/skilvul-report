# **Rangkuman Minggu Ke-2**

## 1. JavaScript
![image](https://skilvul-prod-01.s3.ap-southeast-1.amazonaws.com/course/Skilvul%20asset%20volume%202-02.jpg)

### A. JS Scope
Scope merupakan konsep dalam flow data variabel yang mana dengan scope dapat menentukan suatu variabel bisa diakses pada scope tertentu atau tidak.

#### **Jenis Scope**
#### - Block Scope
Block scope adalah cakupan kode yang hanya terbatas pada block code saja. Block code adalah area yang ada di antara kurung kurawal `{` dan `}`.

Contoh :
```js
var printConsole = function(){
  if(true){
    let greeting = "Good Morning"
    console.log(greeting)
  }
  console.log(greeting)
}
printConsole()
```

Hasil :

![image](https://cdn.discordapp.com/attachments/773086561696612372/1026378529337786408/unknown.png)

Error terjadi karena `console.log` kedua tidak bisa mengakses variabel greeting. Variabel yang dibuat dengan menggunakan `let` atau `const` akan tidak bisa diakses apabila dipanggil di luar block kode.

#### - Global Scope
Global scope adalah kode yang cakupannya di seluruh file javascript sehingga bisa diakses oleh semua fungsi yang ada di dalam file javascript. Agar bisa menjadi Global scope, maka kode perlu di tulis di dasar atau root dari file javascript.

Contoh :
```js
var greeting = "Halo! ini adalah Global Scope"

function printConsole() {
  console.log(greeting)
}
printConsole()

function printMessage(param) {
  console.log(param)
}
printMessage(greeting)
```

Hasil :

![image](https://cdn.discordapp.com/attachments/773086561696612372/1026380962164117525/unknown.png)

Dari kode diatas variabel `greeting` bisa dipanggil di dalam fungsi `printAlert` dan juga bisa menjadikan variabel `greeting` sebagai argument untuk memanggil fungsi `printConsole`. Ini adalah salah satu contoh kemampuan variabel pada global scope untuk diakses oleh kode lain di dalam satu file Javascript.

#### - Local Scope
Local Scope atau function scope adalah cakupan kode yang hanya dapat diakses dari dalam fungsi itu saja dan tidak bisa diakses oleh kode di luar fungsi tersebut.

Contoh 1 :
```js
function printConsole() {
  var greeting = "Halo! ini adalah Local Scope"
  console.log(greeting)
}
printConsole()

function printMessage(param) {
  console.log(param)
}
printMessage(greeting)
```

Hasil :

![image](https://cdn.discordapp.com/attachments/773086561696612372/1026383355152965692/unknown.png)

Output dari kode di atas adalah adanya alert berisi nilai variabel `greeting` namun output pada console hanya berisi `undefined`, hal ini terjadi karena variabel `greeting` hanya dapat diakses oleh kode yang ada di dalam fungsi `printAlert`.

Contoh 2 :
```js
var printConsole = function () {
  if (true) {
    var greeting = "Halo! ini adalah Local Scope"
  }
  console.log(greeting)
}
printConsole()
```

Hasil :

![image](https://cdn.discordapp.com/attachments/773086561696612372/1026383645193273354/unknown.png)

Variabel yang dibuat menggunakan keyword `var` akan menjadi local variabel di dalam fungsi.

### B. JS Function
Function adalah sebuah blok kode dalam sebuah grup untuk menyelesaikan 1 task / fitur yang mana penggunaannya dapat digunakan berkali-kali dengan cara memanggil function tersebut untuk dijalankan.

#### 1. Pembuatan Function
```js
function greeting(){
  return "Halo! ini dari function greeting";
}
```

#### 2. Pemanggilan Function
```js
greeting(); //Memanggil function greeting
console.log(greeting())
```

Hasil :

![image](https://cdn.discordapp.com/attachments/773086561696612372/1026387548681027615/unknown.png)

#### 4. Parameter dan Argumen
Dengan parameter, function dapat menerima sebuah inputan data dan menggunakannya untuk melakukan task/tugas. Saat membuat function/fitur, kita harus tahu data-data yang dibutuhkan. Misalnya saat membuat function penambahan 2 buah nilai. Maka data yang dibutuhkan adalah 2 buah nilai tersebut. Kemudian, Argumen adalah nilai yang digunakan saat memanggil function. Jumlah argumen harus sama dengan jumlah parameternya. Maka jika di function penambahan ada 2 parameter nilai saat membuat function. Saat memanggil function kita gunakan 2 buah nilai argumen.

Contoh :
```js
function perkalian(a, b){
  return a*b;
}
console.log(perkalian(8, 6))

//a dan b merupakan parameter dari function perkalian
//8 dan 6 merupakan argument dari function perkalian
```

### C. Error dan Debugging
#### **1. Error Message**
#### a. Reference Errors (Kesalahan Referensi)
Ketika mencoba menggunakan variabel yang belum dideklarasikan, maka akan mendapatkan pesan kesalahan seperti berikut pada console log.
```js
Uncaught ReferenceError: foo is not defined
```

Untuk mengatasi permasalahan ini kita hanya perlu melakukan deklarasi terlebih dahulu variabel tersebut sebelum variabel dipanggil atau digunakan.

#### b. Syntax Errors (Kesalahan Syntaks)
Syntax error adalah kesalahan penulisan kode dalam sebuah program. Biasanya salah memasukkan angka, kata, atau tanda baca sehingga format atau informasi tersebut tidak bisa dikenali oleh sistem komputer. Seperti ketika mencoba mengurai objek yang tidak valid menggunakan JSON.parse. Hal ini akan memunculkan pesan error pada console log seperti berikut.
```js
Uncaught SyntaxError: "[object Object]" is not valid JSON
```

Untuk mengatasi permasalahan ini kita dapat memperbaiki sintaks dimana objek JSON tersebut ingin dijalankan.

#### c. Range Errors
Range error adalah kesalahan yang terjadi ketika objek dengan panjang tertentu tidak valid. Hal ini akan memunculkan pesan error pada console log seperti berikut.
```js
Uncaught RangeError: Invalid array length
```

Untuk mengatasi permasalahan ini kita dapat menyesuaikan panjang dari objek yang diinginkan sesuai dengan panjang yang akan diberikan.

#### d. Type Errors
Kesalahan ini muncul ketika jenis (angka, string dll) yang kita coba gunakan atau akses tidak kompatibel seperti mengakses properti dalam jenis variabel yang tidak ditentukan. Untuk mengatasi permasalahan ini kita dapat menyesuaikan jenis data yang kita inginkan dengan jenis data yang sesuai atau yang sudah dideklarasikan.

#### **2. Debugging**
Untuk mendebug kode JavaScript adalah dengan cara menggunakan console.log() variabel yang ingin kita periksa. Untuk melihat hasilnya kita bisa menggunakan Inspect pada browser yang kita miliki.

### D. Tipe dan Struktur Data
JavaScript adalah bahasa dinamis dengan tipe dinamis. Variabel dalam JS tidak secara langsung terkait dengan jenis nilai tertentu dan variabel apapun dapat diberi nilai dari semua jenis.

#### **1. Jenis Tipe Data JavaScript**
#### a. Nilai primitif
Nilai primitif adalah tipe data yang tidak dapat diubah diwakili pada tingkat bahasa terendah.
Contoh :
- Boolean
- Null
- Undefined
- Number
- Bigint
- String
- Types of Symbol

#### b. Object (Kumpulan Properti)
Dalam ilmu komputer, object adalah nilai dalam memori yang mungkin dirujuk oleh pengidentifikasi.
Ada dua jenis properti objek:
- properti data
- properti pengakses

Setiap properti memiliki atribut yang sesuai. Setiap atribut diakses secara internal oleh mesin JavaScript, tetapi kita juga dapat mengaturnya melalui Object.defineProperty(), atau membacanya melalui Object.getOwnPropertyDescriptor().

## 2. DOM (Document Object Model)
![image](https://skilvul.com/static/nav-path.svg)

Model Objek Dokumen W3C (DOM) adalah platform dan antarmuka netral bahasa yang memungkinkan program dan skrip untuk mengakses dan memperbarui konten, struktur, dan gaya dokumen secara dinamis. Dengan DOM, JavaScript mendapatkan semua kebutuhan untuk membuat HTML dinamis.

### A. DOM HTML
_HTML DOM_ adalah model objek standar dan antarmuka pemrograman untuk HTML.
- Elemen HTML sebagai objek
- Properti dari semua elemen HTML
- Metode untuk mengakses semua elemen HTML
- Acara untuk semua elemen HTML
> DOM HTML adalah standar untuk mendapatkan, mengubah, menambah, atau menghapus elemen HTML.

### B. Interface DOM
_HTML DOM_ dapat diakses dengan _JavaScript_ (dan dengan bahasan pemograman lainnya). Semua element HTML pada DOM didefinisikan sebagai objek. Antarmuka pemrograman adalah properti dan metode dari setiap objek. Properti adalah nilai yang bisa Anda dapatkan atau atur (seperti mengubah konten elemen HTML). Metode adalah tindakan yang dapat Anda lakukan (seperti menambah atau menghapus elemen HTML).

### C. Elemen DOM HTML JavaScript
#### **1. Mengambil Element HTML**
#### a. Mengambil Element HTML dengan Id
```js
document.getElementById("id-name")
```

#### b. Mengambil Element HTML dengan Tag
```js
document.getElementByTagName("tage-name")
```

#### c. Mengambil Element HTML dengan Class
```js
document.getElementByClassName("class-name")
```

#### d. Mengambil Element HTML dengan CSS Selector
```js
document.querySelectorAll("tag-name.id-name")
```

#### e. Mengambil Element HTML dengan Object HTML
```js
document.getElementById("id-name").innerHTML
```
Macam-macam Object HTML
- document.anchors
- document.body
- document.documentElement
- document.embeds
- document.forms
- document.head
- document.images
- document.links
- document.scripts

#### **2. Mengedit HTML**
#### a. Mengedit Konten HTML
```js
document.getElementById(id).innerHTML = new HTML();
```

#### b. Mengedit Nilai Attribute
```js
document.getElementById(id).attribute = new value;
```
#### c. Membuat Konten HTML yang Dinamis
```html
<!DOCTYPE html>
<html>
  <body>
    <p id="demo"></p>
    <script>
      document.getElementById("demo").innerHTML = "Date : " + Date();
    </script>
  </body>
</html>
```

Hasil : 

![image](https://cdn.discordapp.com/attachments/773086561696612372/1026417693148074065/unknown.png)
