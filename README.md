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
