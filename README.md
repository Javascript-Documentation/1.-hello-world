# Pengenalan dan Console

# Materi:

- [x]  Pengertian js
- [x]  macam2 console
- [x]  prompt dan alert

## Apa itu javascript:

Javascript adalah bahasa pemrograman untuk website, yang merupakan bahasa scripting yang berjalan di sisi client (browser). Yang mana javascript ini berperan dalam membuat website lebih dinamis dan interaktif. Yang mana kita bisa mengubah html, mengatur gaya css bahkan bisa berdasarkan perkondisian, dan menanggapi input pengguna (klik, ketikan, gerakan cursor, dll)

## Console Browser

pada browser kita bisa melakukan namanya inspect, disitu ada banyak menu. salah satunya itu console, yang mana kita bisa ke console juga dengan cara F12 atau fn+F12.

1. **console.log()**
Fungsi ini digunakan untuk mencetak pesan atau nilai variabel ke console. ini tipenya umum
    
    ```jsx
    console.log("Hello, world!");
    ```
    
    contoh:
    
    ```jsx
    let nama = "John";
    let usia = 30;
    console.log("Nama:", nama, ", Usia:", usia);
    ```
    
2. **console.error()**
    
    Digunakan untuk mencetak pesan kesalahan ke console. menandakan bahwa terjadi kesalahan dalam eksekusi kode yang harus diperbaiki. Kesalahan sering kali menghentikan aliran eksekusi kode atau menyebabkan hasil yang tidak diinginkan dalam aplikasi.
    
    ```jsx
    console.error("Terjadi kesalahan!");
    ```
    
    contoh:
    
    ```jsx
    let hasil = 10 / "a";
    if (isNaN(hasil)) {
        console.error("Operasi pembagian tidak valid!");
    } // karena a tidak terdefinisi atau harus dibagi dengan angka!
    ```
    
3. **console.warn()**
Mencetak pesan peringatan ke console. biasanya mengindikasikan situasi yang tidak diharapkan atau potensial masalah yang perlu diperhatikan, tetapi tidak menghentikan aliran eksekusi kode atau tidak secara langsung menyebabkan kegagalan atau kesalahan dalam aplikasi.
    
    ```jsx
    console.warn("Ini peringatan!");
    ```
    
    contoh kasus:
    
    ```jsx
    let nilai = 70;
    if (nilai < 75) {
        console.warn("Anda belum mencapai nilai minimal yang diperlukan.");
    }
    ```
    
4. **console.info()**
    
    Mencetak pesan informasi ke console. bedanya dengan console.log itu memberikan informasi yang lebih spesifik atau relevan. Beberapa pengembang menggunakan **`console.info()`** untuk mencetak pesan yang mereka anggap sebagai informasi penting atau pesan spesifik yang perlu ditekankan.
    
    ```jsx
    console.info("Ini informasi.");
    ```
    
    contoh:
    
    ```jsx
    let jumlahData = 100;
    console.info("Mengolah", jumlahData, "data...");
    ```
    
5. **console.table()**:
Mencetak array atau objek dalam bentuk tabel di console. Yang mana ini dipake buat kita dapatin bentukan table dari data kita baik dalam bentuk array maupun object.
    
    ```jsx
    let mahasiswa = [{nama: "John", usia: 25}, {nama: "Jane", usia: 22}];
    console.table(mahasiswa);
    ```
    
    mari ke contoh lain:
    
    ```jsx
    let buku = {
      judul: "JavaScript for Beginners",
      penulis: "John Doe",
      tahun_terbit: 2022,
      harga: 150000
    };
    
    console.table(buku);
    ```
    
6. **console.clear()**
    
    Digunakan untuk menghapus semua pesan dari console.
    
    ```jsx
    console.clear();
    ```
    
    

---

## Prompt dan Alert

1. **prompt()**
    
    Fungsi ini digunakan untuk meminta input dari pengguna melalui dialog box.
    
    ```jsx
    let nama = prompt("Masukkan nama Anda:");
    alert("Halo, " + nama + "! Selamat datang!");
    ```
    
2. **alert()**
    
    Fungsi ini digunakan untuk menampilkan pesan kepada pengguna melalui dialog box. 
    
    ```jsx
    alert("Terjadi kesalahan! Silakan coba lagi.");
    ```
