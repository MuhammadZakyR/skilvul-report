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
#### **1. Jenis Error Message**
#### a. Reference Errors (Kesalahan Referensi)
Ketika mencoba menggunakan variabel yang belum dideklarasikan, maka akan mendapatkan pesan kesalahan seperti berikut pada console log.
```js
Uncaught ReferenceError: foo is not defined
```
Untuk mengatasi permasalahan ini kita hanya perlu melakukan deklarasi terlebih dahulu variabel tersebut sebelum variabel dipanggil atau digunakan.

#### b. Syntax Errors (Kesalahan Syntaks)
