# **Rangkuman Minggu Ke-8**
## A. React Context 
<br>

- Context menyediakan cara untuk membagikan data melalui sebuah komponent tanpa harus menurunkan props 
  
- Cara kerja context tidak jauh beda dengan **Redux** === Menghindari props drilling 
  
- Perbedaan **Context** dan **Redux** terletak pada dependecy yang digunakan
  
- Context digunakan untuk melakukan passing data yang dianggap  `global` 

### 1. Cara Membuat sebuah Context 
---

- React.createContext() 

    ```js
    import React from "react";

    const MyContext = React.createContext()

    export default MyContext 

    ``` 

- Selanjutnya context dapat digunakan dengan menjalankan/ menuliskan 

    - Context.Provider
        > digunakan untuk menyediakan data yang nantinya data tersebut dapat diakses oleh komponents yang ada didalamnya 

    - Context.Costumer
        > digunakan untuk mengakses data    yang berada atau disediakan oleh Context.Provider 
<br>

- Selain menggunakan _Context.Costumer_ bisa juga menggunakan **Hooks** berupa **useContext()** untuk mengakses data yang ada pada Context.Provider 

--- 

<br>

## B. React Testing

<br>

- Testing adalah step pengecekan / uji coba yang dilakukan saat tahap development untuk melihat apakah ekspetasi dari web / product yang sedang dikembangkan sesuai dengan yang diinginkan 
  
- Testing terbagi menjadi 2 yaitu 

    - Automated
    Yang dimaksud dengan automated atau otomatis adalah, dengan menjalankan sebuah code untuk memeriksa apakah ekspetasi dan susunan code sudah terjalankan dengan baik 

    - Manual
    Yang dimaksud dengan Manual Testing adalah, dengan melihat menggunakan browser pada kontent yang telah disusun
  
Automated Testing terbagi menjadi 3 

- Unit test, melakukan pengujian pada bagian yang paling kecil (contohnya testing sebuah function ) `menggunakan RTL dan Jest` 
  
- Integration, dilakukan saat product memiliki hubungan ke app atau sebuah sistem (c/o: terhubung ke database)
  
- end 2 end, testing yang dilakukan secara sisi pengguna 

<br>

### 1. RTL ( REACT TESTING LIBRARY )
<br>

- React Testing Library adalah salah satu cara untuk melakukan testing pada komponents React

- Installasinya dapat menggunakan _npm_ atau _yarn_ 
  
  ```

    npm install --save-dev @testing-library/react 

    yarn add --dev @testing-library/react

  ```
  

- 2 cara penulisan testing 
  
    - `Buat fitur lalu lakukan testing ( `biasanya dilakukan oleh startup` ) 
      
    - Lakukan testing lalu buat fitur -> TDD 
      
        - Ketika masih membuat ekspetasi dan code masih tidak terjalankan akan masuk kedalam ranah `red zone`

        - saat kode sudah dibuat maka akan masuk kedalam ranah `green zone` lalu disesuaikan dengan ekspetasi 
      
        - `blue zone` disaat ekspetasi dikembangk`an
