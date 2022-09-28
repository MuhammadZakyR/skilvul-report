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

