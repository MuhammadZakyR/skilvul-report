# **Rangkuman Minggu Ke-1**

## 1. Unix Command Line
![image](https://skilvul-prod-01.s3.ap-southeast-1.amazonaws.com/course/unix-command-line-dasar-1631260071148.jpeg)

### A. Shell
Shell merupakan salah satu jenis program yang ada pada komputer untuk pengguna dapat berkomunikasi atau memerintahkan sistem operasi. Shell menurut jenis tampilannya dibagi menjadi dua yaitu `Graphical User Interface (GPU)` dan `Command Line Interface (CLI)`

### B. CLI (Command Line Interface)
CLI merupakan salah satu jenis aplikasi yang interaksinya hanya berbasis tulisan atau command untuk memerintahkan perangkat komputer dalam menjalankan suatu tugas tertentu.

Berikut adalah beberapa contoh aplikasi yang berbasis CLI :
- sh
- bash
- zsh
- cmd.exe

### C. Terminal Emulator
![image](https://cdn.discordapp.com/attachments/773086561696612372/1024603958293037136/unknown.png)

Terminal Emulator merupakan sebuah program atau media yang menghubungkan antara pengguna dan komputer. Di terminal emulator inilah pengguna dapat mengetikan atau memberikan perintah pada komputer.

### D. File System Structure
![image](https://raw.githubusercontent.com/Jirjatss/week-1/main/gambar/tree.JPG)

Sebuah sistem file yang mengatur bagaimana data dapat disimpan dalam sistem operasi.

### E. Command / Perintah CLI
#### 1. Melihat lokasi folder atau file yang sedang dibuka
```
pwd
```
#### 2. Melihat isi folder
```
ls
```
#### 3. Melihat isi file
```
nano <nama file>
```
#### 4. Berpindah folder
```
cd <nama folder>
```
Berpindah ke folder sebelumnya :
```
cd ..
```
#### 5. Membuat folder
```
mkdir <nama folder>
```
#### 6. Membuat file
```
touch <nama file>
```
#### 7. Menyalin folder atau file
```
cp <asal> <tujuan>
```
#### 8. Memindahkan folder atau file
```
mv <asal> <tujuan>
```
#### 9. Menghapus folder atau file
```
rm <nama folder atau file>
```

## 2. Git dan Github
![image](https://skilvul-prod-01.s3.ap-southeast-1.amazonaws.com/course/git-dan-github-dasar-1631259937188.png)

### A. Definisi
- Git
Merupakan sebuah aplikasi yang digunakan oleh seorang developer sebagai alat yang dapat membantu developer untuk membuat sebuah `Version Control System` pada aplikasi yang akan dibuat.

- Github
Merupakan sebuah vendor penyedia layanan git atau layanan hosting berbasis web sebagai repository git.

### B. Tujuan
Dengan bantuan Git, Developer dapat melacak perubahan dalam aplikasi yang sedang dibuat. Selain itu, developer juga dapat memanfaatkan Github sebagai media untuk berkolaborasi dengan developer yang lain dalam menyelesaikan suatu project atau aplikasi.

### C. Command / Perintah Git

#### 1. Untuk pengguna baru, diwajibkan untuk membuat atau mendaftarkan `username` dan `email` terlebih dahulu dengan menjalankan perintah berikut pada Terminal Emulator.

- Membuat username
```
git config --global user.name "username"
```
- Membuat email
```
git config --global user.email contoh@email.com
```
Untuk mengecek apakah `username` dan `email` sudah berhasil dibuat, silahkan jalankan perintah berikut.
```
git config --list
```
Apabila sudah terdaftar maka akan muncul list `user.name` dan `user.email` seperti pada gambar dibawah ini.

![image](https://cdn.discordapp.com/attachments/773086561696612372/1024617529198514227/unknown.png)

#### 2. Memulai untuk membuat repositori git baru
```
git init <nama project>
```
#### 3. Menghubungkan repository dengan project yang sedang dibuat
```
git remote add origin <URL remote>
```
#### 4. Melihat histori perubahan pada git
```
git status
```
#### 5. Memilih folder atau file untuk ditambahkan kedalam remote repositori
- Memilih semua folder dan file
```
git add .
```
- Memilih folder atau file tertentu
```
git add <nama file>
```
#### 6. Menyimpan perubahan yang dilakukan, tetapi tiak ada perubahan pada remote repositori
```
git commit -m "Pesan Commit"
```
#### 7. Mengupload dan menggabungkan folder atau file yang sudah di commit kedalam remote repositori
```
git push -u origin master
```
#### 8. Menyalin Repository
- Fork
![image](https://cdn.discordapp.com/attachments/773086561696612372/1024626081938034739/unknown.png)

Fork merupakan salah satu cara untuk menyalin repositori developer lain yang mana repositori tersebut dapat langsung masuk kedalam repositori pribadi secara automatis.

- Terminal Emulator
![image](https://cdn.discordapp.com/attachments/773086561696612372/1024626599263490048/unknown.png)

Untuk menyalin dengan menggunakan terminal emulator, pengguna harus menentukan terlebih dahulu lokasi dimana repositori tersebut ingin disimpan dengan mengarahkan posisi atau letak dari terminal emulator tersebut. Kemudian jalankan perintah berikut pada terminal emulator.
```
git clone <URL repositori>
```

- ZIP / RAR
![image](https://cdn.discordapp.com/attachments/773086561696612372/1024627787480444948/unknown.png)

Untuk yang merasa terlalu rumit dengan cara sebelumnya, kita juga dapat secara langsung mendownload repositori tersebut dengan cara mendownload langsung melalui ZIP dan ekstrak folder sesuai dengan lokasi yang diinginkan.

## 3. HTML (_HyperText Markup Language_)
![image](https://skilvul-prod-01.s3.ap-southeast-1.amazonaws.com/course/Skilvul%20asset%20volume%202-03.jpg)

### A. Definisi
HTML (_HyperText Markup Language_) merupakan bahasa markup standar yang digunakan untuk membuat dan menyusun halaman dan aplikasi web. Pada halaman website, HTML sendiri berperan sebagai kerangka atau struktur. Dengan HTML, developer dapat menampilkan beberapa konten seperti gambar, video, audio, teks, dan banyak lagi.

### B. Tools
Dalam pembuatan website, diperlukan dua tools penting yaitu :
- Browser
`Google Chrome`, `Mozila Firefox`, `Microsoft Edge`, dll.
- Text Editor
`Visual Studio Code`, `Notepad`, `Adobe Dreamweafer`, dll.

### C. Struktur Dokumen HTML
```html
<!DOCTYPE html>
<html lang="en">
<head>
    ...
</head>
<body>
    ...
</body>
</html>
```
> `<!DOCTYPE>`  : Tag untuk menentukan tipe dokumen <br>
  `<html>`      : Tag untuk membuat sebuah dokumen HTML <br>
  `<head>`      : Tag untuk meletakkan metadata <br>
  `<body>`      : Tag untuk membuat tubuh dari sebuah halaman
  
### D. Tag HTML
```html
<p>contoh</p>
```
> `<p>`     : Tag Pembuka <br>
  `contoh`  : Konten HTML <br>
  `</p>`    : Tag Penutup
  
#### 1. Tag Text
```html
    <h1>Heading 1</h1>
    <h2>Heading 2</h2>
    <h3>Heading 3</h3>
    <h4>Heading 4</h4>
    <h5>Heading 5</h5>
    <h6>Heading 6</h6>
    <p>Paragraph</p>
```
Hasil :

![image](https://cdn.discordapp.com/attachments/773086561696612372/1023961110707179580/unknown.png)

#### 2. Tag Content
- Gambar
```html
    <img src="https://cdn.discordapp.com/attachments/773086561696612372/1023963985151799416/unknown.png" alt="Foto Kucing">
```
> `src` : Attribute untuk memberitahukan sumber gambar <br>
  `alt` : Attribute yang digunakan untuk memberikan keterangan gambar, apabila gambar tidak tampil

Hasil :

![image](https://cdn.discordapp.com/attachments/773086561696612372/1023963985151799416/unknown.png)

- Video
```html
<video><source src="movie.mp4" type="video/mp4" alt="movie"></video>
```
> `type` : Attribute untuk memberitahukan tipe konten

Hasil :

![image](https://user-images.githubusercontent.com/82355658/192154869-0a7e8a47-8b4c-434e-96ff-990d01ba177a.png)

- Table
```html
    <table>
        <thead>
            <tr>
              <th>Month</th>
              <th>Savings</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>January</td>
              <td>$100</td>
            </tr>
            <tr>
              <td>February</td>
              <td>$80</td>
            </tr>
          </tbody>
    </table>
```
> `<table>` : Tag untuk membuat dan membungkus tabel <br>
  `<thead>` : Tag untuk mengelompokan isi header dalam sebuah tabel <br>
  `<tbody>` : Tag untuk mengelompokan isi tubuh dalam sebuah tabel <br>
  `<tr>`  : Tag untuk membuat baris dalam sebuah tabel <br>
  `<th>`  : Tag untuk membuat sebuah sel header tabel <br>
  `<td>`  : Tag untuk membuat sel dalam sebuah tabel
  
Hasil :

![image](https://cdn.discordapp.com/attachments/773086561696612372/1023969518927753226/unknown.png)

### E. Deploy
Deploy merupakan sebuah proses untuk mengupload atau mempublikasi website atau aplikasi yang sudah dibuat sedemikian rupa sehingga dapat diakses oleh orang-orang. Dalam kasus deploy website, diperlukan yang namanya hosting dan domain. Hosting diperlukan untuk penyimpanan file atau database yang sudah kita buat kedalam server online sehingga website yang sudah dibuat dapat diakses secara online oleh orang-orang. Domain diperlukan untuk menamai atau memberikan alamat untuk website yang sudah dibuat sehingga pengguna dapat mencari website tersebut sesuai dengan alamat website tersebut. Hosting dan Domain memiliki variant harga yang bermacam-macam. Untuk latihan, developer dapat menggunakan `Netlify` sebagai penyedia layanan hosting untuk static site.

#### Tutorial mendeploy website melalui Netlify
- Buka website Netlify dengan mengklik link berikut https://www.netlify.com/.
![image](https://user-images.githubusercontent.com/82355658/192666546-2c853a36-6dca-4a7f-9409-6edf41a8f1dd.png)

- Masuk ke tab Sites, lalu pilih `Import an existing project` atau `drag & drop` seluruh folder html.

![image](https://user-images.githubusercontent.com/82355658/192665549-c50b1371-0f99-469b-a0b9-e055a90db8ed.png)

- Otorisasi Netlify.

![image](https://user-images.githubusercontent.com/82355658/192666645-1df918f4-147a-45c6-be13-1ae6af9e2167.png)

- Pilih repository yang ingin dideploy.

![image](https://user-images.githubusercontent.com/82355658/192666817-0500c3a7-d748-438a-98cf-0b51b1c949c8.png)

- Menyesuaikan konfigurasi.

![image](https://user-images.githubusercontent.com/82355658/192666843-c98a528a-285d-421f-867e-769f451e3f9d.png)

- Deploy website.

## 4. CSS (_Cascading Style Sheets_)
![image](https://skilvul-prod-01.s3.ap-southeast-1.amazonaws.com/course/Skilvul%20asset%20volume%202-04.jpg)

### A. Definisi
CSS (_Cascading Style Sheets_) merupakan bahasa yang digunakan untuk menentukan dan menghias tampilan dan format halaman pada website dan aplikasi web. Dengan CSS, developer dapat mengubah dan mengatur warna, font, tata letak, dan tampilan pada konten-konten.

#### B. CSS Syntax
```css
selector{property: value;}
```
> `selector`    : Tag atau element HTML yang akan diinisialisasikan <br>
`property`  : Attribute yang akan dikustomisasi nilainya <br>
`value` : Nilai yang diberikan untuk property yang di kustomisasi pada selector tersebut

### C. Penggunaan CSS
#### 1. Inline CSS
Meyisipkan kode CSS langsung di dalam halaman HTML dengan cara menambahkan attribute style pada element HTML secara langsung. Cara ini digunakan untuk mengatur komponen CSS pada element HTML tertentu saja secara spesifik.
- Contoh :
```css
<h1 style="color:blue">Contoh Inline CSS</h1>
```
- Hasil :

![image](https://cdn.discordapp.com/attachments/773086561696612372/1024649644585783427/unknown.png)

#### 2. Internal CSS
Menyusun atau membuat kustomisasi CSS di dalam tag `<style>` yang diletakkan di dalam tag `<head>`. Cara ini digunakan untuk mengatur komponen CSS sesuai dengan kelompok element HTML tertentu yang ada pada satu halaman website tersebut.
- Contoh :
```css
<head>
    <style>
        h2 {color: red;}
    </style>
</head>
<body>
    <h1 style="color:blue">Contoh Inline CSS</h1>
    <h2>Contoh Internal CSS</h2>
</body>
```
- Hasil :

![image](https://cdn.discordapp.com/attachments/773086561696612372/1024652544972181514/unknown.png)

#### 3. Eksternal CSS
Menyusun atau membuat kustomisasi CSS dengan cara membuat file CSS terpisah dengan file HTML. Kemudian untuk menautkannya dengan halaman atau file HTML dapat dilakukan dengan cara menambahkan tag atau element `<link>` yang diletakkan di dalam tag `<head>`. Cara ini digunakan untuk mengatur komponen CSS sesuai dengan kelompok element HTML tertentu yang ada pada beberapa halaman website yang berbeda.
- Contoh :
1. File CSS `style.css`
```css
h3{color: green;}
```
2. File HTML `index.html`
```html
<head>
    <link rel="stylesheet" href="style.css">
    <style>
        h2 {color: red;}
    </style>
</head>
<body>
    <h1 style="color:blue">Contoh Inline CSS</h1>
    <h2>Contoh Internal CSS</h2>
    <h3>Contoh Eksternal CSS</h3>
</body>
```
- Hasil :

![image](https://cdn.discordapp.com/attachments/773086561696612372/1024655032332857514/unknown.png)

### D. Responsive Design
Responsive web design atau desain web responsif adalah sebuah teknik atau metode bagi web designer untuk membuat suatu layout website yang dapat menyesuaikan diri sesuai dengan ukuran layar pengguna.

### E. Flexbox
Flexbox merupakan salah satu cara untuk menata, menyelaraskan dan mendistribusikan ruang di antara item tertentu dalam satu wadah konsten dengan lebih efisien. Ada dua komponen utama pada layout Flexbox yaitu `container` dan `item`.

#### Langkah-langkah pembuatan Flexbox
1. Membuat `Container`
File CSS
```css
.container{display: flex;}
```
File HTML
```html
<section class="container">
    <div>Home</div>
    <div>About</div>
    <div>Contact Us</div>
</section>
```

![image](https://cdn.discordapp.com/attachments/773086561696612372/1024663105982189688/unknown.png)

2. Mengatur `Justify Content` dan `Align Items`
Justify-content dan align-items adalah dua properti CSS yang membantu kita mendistribusikan item-item di dalam container dengan mengontrol bagaimana item diposisikan secara `horizontal` dan `vertikal`.
File CSS
```css
.container{
display: flex;
justify-content: center;
}
```
File HTML
```html
<section class="container">
    <div>Home</div>
    <div>About</div>
    <div>Contact Us</div>
</section>
```

![image](https://cdn.discordapp.com/attachments/773086561696612372/1024662999094546472/unknown.png)

- Beberapa jenis nilai pada `justify-content`
> `flex-start` (default)    : Nilai bawaan. Item diposisikan di awal wadah <br>
`flex-end`  : Item diposisikan di ujung wadah <br>
`center`    : Item diposisikan di tengah wadah <br>
`space-between` : Item akan memiliki ruang di antara item yang lain <br>
`space-around`  : Item akan memiliki ruang sebelum, di antara, dan setelahnya <br>
`space-evenly`  : Item akan memiliki ruang yang sama di sekitar mereka

- Beberapa jenis nilai pada `align-items`
> `stretch` (default)    : Item diregangkan agar sesuai dengan wadahnya <br>
`center`    : Item diposisikan di tengah wadah <br>
`flex-start`  : Item diposisikan di awal wadah <br>
`flex-end`  : Item diposisikan di ujung wadah <br>
`baseline` : Item diposisikan di garis dasar wadah

## 5. Algoritma dan Pseudcode
![image](https://skilvul-prod-01.s3.ap-southeast-1.amazonaws.com/course/intro-to-coding-1626243909763.jpg)

### A. Definisi
- Algoritma adalah deskripsi berupa step by step yang dibutuhkan untuk menyelesaikan suatu masalah tertentu. Algoritma digunakan untuk menyelesaikan suatu permasalahan tertentu dengan menggunakan cara dan data yang ada. Dalam menyelesaikan suatu masalah bisa menggunakan beberapa macam algoritma yang berbeda.

Contoh :
Untuk mendapatkan sebuah nilai 10 bisa didapatkan dengan cara sebagai berikut.
1. 10 x 1 = 10
2. 9 + 1 = 10
3. 15 - 5 = 10

Semua cara atau algoritma di atas sama-sama bernilai benar.

- Pseudcode atau kode semu dapat diartikan sebagai deskripsi dari algoritma pemrograman yang dituliskan secara sederhana dibandingkan dengan sintaksis bahasa pemrograman. Tujuannya, agar lebih mudah dibaca dan dipahami manusia.
```js
    Menentukan sebuah bilangan adalah ganjil atau genap
    Judul
    Program ganjil_genap
    
    Deskripsi
    var bilangan : integer
    
    Implementasi
    READ bilangan
    IF (bilangan modulus 2 = 0) THEN
        PRINT ???genap???
    ELSE
    PRINT ???ganjil???
    ENDIF
```

### B. Big O Notatiom
#### 1. Definisi
Sebuah cara atau metode untuk melakukan analisa terhadap sebuah algoritma pemrograman terhadap waktu eksekusi. Tentang seberapa efisien dan kompleksitas barisan kode dalam dimensi waktu.

#### 2. Tujuan
Metode untuk menghitung kompleksitas dari potongan kode yang kita buat. Sehingga dapat menumbuhkan kesadaran kita untuk mencari alternatif yang lebih baik sebelum data semakin besar dan berdampak kepada performa aplikasi yang kita buat.

#### 3. Kategori
- **Time Complexity**
adalah seberapa lama waktu yang diperlukan untuk menjalankan suatu algoritma.
    
- **Space Complexity**
adalah seberapa besar memori yang kita gunakan untuk menjalankan suatu algoritma.

## 6. JavaScript
![image](https://skilvul-prod-01.s3.ap-southeast-1.amazonaws.com/course/Skilvul%20asset%20volume%202-02.jpg)

### A. Definisi
JavaScript merupakan bahasa pemrograman tingkat tinggi dan dinamis. JavaScript populer di internet dan dapat bekerja di sebagian besar penjelajah web populer seperti Google Chrome, Internet Explorer, Mozilla Firefox, Netscape dan Opera. Kode JavaScript dapat disisipkan dalam halaman web menggunakan tag script. Untuk mengecek bagaimana javascript berjalan pada browser, dapat dilihat dengan cara menekan kombinasi tombol `ctrl` + `shift` + `i` untuk membuka `inspect element` dan kemudian pilih `console`.

### B. Statement dan Syntax JavaScript
#### 1. Alert()
Untuk menampilkan sebuah pesan peringatan atau informasi.
```html
<button onClick="alert('Notifikasi Alert!')">Tombol Alert</button>
```

Hasil :

![image](https://cdn.discordapp.com/attachments/773086561696612372/1024680051612057650/unknown.png)

#### 2. Confirm()
Untuk melakukan konfirmasi dalam melakukan tindakan tertentu.
```js
<script>
    var yakin = confirm("Contoh Notifikasi Confirm?");

    if (yakin) {
        window.location = "#";
    } else {
        document.write("Confirm Dibatalkan");
    }
</script>
```

Hasil :

![image](https://cdn.discordapp.com/attachments/773086561696612372/1024682346869436448/unknown.png)

#### 3. Prompt()
Untuk mengambil sebuah inputan dari pengguna.
```js
<script>
    var contoh = prompt("Masukkan Inputan?", "");
    document.write("<p>Isi Inputan adalah "+ contoh +"</p>");
</script>
```

Hasil :

![image](https://cdn.discordapp.com/attachments/773086561696612372/1024683663033638912/unknown.png)

![image](https://cdn.discordapp.com/attachments/773086561696612372/1024683833964101712/unknown.png)

#### 4. Console.log()
Untuk mengecek atau menampilkan nilai atau teks pada console javascript. `console.log()` biasanya digunakan untuk proses debugging pada pemrograman website untuk mengecek apakah fungsi atau code sudah berjalan sesuai dengan apa yang diinginkan atau belum.
```js
console.log('nilai yang ingin dicek')
```

#### 5. Comment
Untuk memberikan keterangan atau menonaktifkan code program tertentu sehingga tidak dieksekusi ketika program dijalankan. Comment di javascript memiliki dua jenis yaitu `Single Comments` dan `Multiline Comments`.
- Single Comments
```js
//Single Comments
```
- Multiline Comments
```js
/*
line 1;
line 2;
*/
```

### C. Tipe Data
#### 1. Definisi
Tipe data adalah klasifikasi yang diberikan untuk berbagai macam jenis data yang digunakan dalam programming.

#### 2. Jenis Tipe Data
a. number => mengandung semua angka termasuk desimal.

b. string => kumpulan kelompok karakter seperti huruf, angka, dan simbol. 

c. boolean => mempunyai 2 nilai yaitu `TRUE` atau `FALSE`.

d. null => data yang tidak memiliki nilai.

e. undefined => tipe data yang merepresentasikan variabel/data yang tidak atau belum terdefinisikan.

f. object => dapat menyimpan data dengan tipe data apapun.

### D. Variabel
#### 1. Var
#### 2. Let
#### 3. Const

### E. Operator
#### 1. Operator Aritmatika
- Tambah(+)
- Kurang(-)
- Perkalian(*)
- Pembagian(/)
- Modulus(%)

Contoh :
```js
var a = 2;
var b = 3;

// menggunakan operator perkalian
var c = a * b;
console.log(c);
```

Hasil :

![image](https://cdn.discordapp.com/attachments/773086561696612372/1024690607198842920/unknown.png)

#### 2. Operator Perbandingan
- Nilai kurang dari (<)
- Nilai lebih dari (>)
- Nilai kurang dari sama dengan (<=)
- Nilai lebih dari sama dengan (>=)
- Nilai sama dengan (===)
- Nilai tidak sama dengan (!==)

Contoh :
```js
<script>
var a = 3;
var b = 3;

if(a>b){
    console.log("Nilai a lebih besar")
} else if(a<b){
    console.log("Nilai a lebih kecil")
} else if(a===b){
    console.log("Nilai a sama dengan b")
} else {
    console.log('Error')
}
</script>
```

Hasil :

![image](https://cdn.discordapp.com/attachments/773086561696612372/1024692625015590983/unknown.png)

#### 3. Operator Logika 
- AND (&&)
- OR (||)
- NOT (!)

Contoh :
```js
<script>
var a = 3;
var b = 3;

if(a>1 && b>1){
    console.log("Nilai a dan b lebih besar dari 1")
} else if(a>1 || b>1){
    console.log("Nilai a atau b lebih besar dari 1")
} else if(a != b){
    console.log("Nilai a tidak sama dengan b")
} else {
    console.log('Error')
}
</script>
```

Hasil :

![image](https://cdn.discordapp.com/attachments/773086561696612372/1024694175700090960/unknown.png)

### F. Conditional
#### 1. Definisi
Conditional merupakan statemen percabangan yang menggambarkan suatu kondisi. Apakah kondisi tersebut TRUE (benar) atau FALSE (salah). Apabila TRUE maka code akan dijalankan sesuai dengan alurnya, namun apabila FALSE maka akan berjalan sesuai dengan perintah ketika FALSE atau program akan berhenti ditempat apabil kondisi FALSE belum didefinisikan.

#### 2. Jenis
- TRUTHY AND FALSY ASSIGNMENT
```js
<script>
var a = 3;
var b = 3;

if(a>1 && b>1){
    console.log("Nilai a dan b lebih besar dari 1")
} else if(a>1 || b>1){
    console.log("Nilai a atau b lebih besar dari 1")
} else if(a != b){
    console.log("Nilai a tidak sama dengan b")
} else {
    console.log('Error')
}
</script>
```

Hasil :

![image](https://cdn.discordapp.com/attachments/773086561696612372/1024694175700090960/unknown.png)

- SWITCH CASE CONDITIONAL
```js
<body>
<!-- <button id="yakin">Tombol Confirm</button> -->
<div id="hasil"></div>
<script>
var warna = "merah";

switch (warna){
case "hitam":
teks = "warna hitam";
break;
case "merah":
teks = "Warna merah";
break;
case "hijau":
teks = "Warna hijau";
break;
default:
teks = "Warna tidak terdeteksi";
}		

document.getElementById("hasil").innerHTML = teks;
</script>

</body>
```

Hasil :

![image](https://cdn.discordapp.com/attachments/773086561696612372/1024698046413557780/unknown.png)

- TERNARY OPERATOR
```
let a = true;
a ? console.log('Sesuai') : console.log('Tidak Sesuai');
```

Hasil :

![image](https://cdn.discordapp.com/attachments/773086561696612372/1024699450381324369/unknown.png)

### G. Function
#### 1. Definisi
Function adalah sebuah blok kode untuk menyelesaikan sebuah task atau fitur.
```js
function nama(){
    return "Output";
}
```
> `function`    : Inisialisasi function <br>
`nama()`    : Nama function <br>
`return "Output"`    : Isi function

#### 2. Jenis
A. Default Parameters

B. Function Helper

C. Arrow Function

D. Short Syntax Function
- Zero Parameters
```js
const functionName = () => {};
```
- One Parameter
```js
const functionName = paramOne => {};
```
- Two or More Parameters
```js
const functionName = (paramOne, paramTwo) => {};
```
- Single-Line Block
```js
const sumNumbers = number => number + number;
```
- Multi Line Block
```js
const sumNumbers = number => {
const sum = number + number;
return sum;
};
```
