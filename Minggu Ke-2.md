# **Rangkuman Minggu Ke-2**

## 1. JavaScript
![image](https://skilvul-prod-01.s3.ap-southeast-1.amazonaws.com/course/Skilvul%20asset%20volume%202-02.jpg)

### A. JS Scope
Scope merupakan konsep dalam flow data variabel yang mana dengan scope dapat menentukan suatu variabel bisa diakses pada scope tertentu atau tidak.

#### 1. Jenis Scope
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
