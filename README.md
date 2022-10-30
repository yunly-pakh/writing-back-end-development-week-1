# Day 5
## Design Database With MySQL (Lanjutan)
- # Membuat design db data film kesukaan :
- mahasiswa dapat menyukai banyak film

![image](https://user-images.githubusercontent.com/113356785/198856812-220f7e65-8dc7-419e-a7fb-ee7c81518dc2.png)

- Mahasiswa dapat menyukai banyak film. tiap film memiliki informasi terkait genre, tiap film mempunyai banyak genre

![image](https://user-images.githubusercontent.com/113356785/198857161-fe4e5bb2-3748-43f7-ab3e-3547b33cd35d.png)

- # Apa Itu Primary Key Dan Foreign Key Di SQL Database?

- primary key adalah tanda pengenal unik yang membedakan satu record dari yang lain. Oleh karena itu, setiap record dalam SQL database management system harus memiliki primary key.

    ada beberapa aturan yang harus kalian ikuti ketika menentukan primary key untuk tabel:
    
     - Primary key harus berisi nilai unik
     - Kolom primary key tidak boleh berisi nilai NULL
     - Sebuah tabel hanya memiliki satu primary key
     

- Foreign key adalah pengenal unik atau kombinasi pengenal unik yang menghubungkan dua tabel atau lebih dalam database.

    Saat memutuskan tabel mana dalam database relasional yang harus memiliki foreign key, harus terlebih dahulu mengidentifikasi tabel mana yang merupakan subjek dan objek dalam hubungannya.

- Perbedaan Primary Key Dan Foreign Key

    - Tidak ada dua baris yang dapat memiliki value identik untuk primary key sedangkan Foreign key dapat berisi value duplikat.
    
    - Tidak ada batasan dalam memasukkan value ke dalam kolom tabel primary key ssedangkan Saat memasukkan value apa pun dalam tabelforeign key, pastikan bahwa value tersebut ada di kolom primary key.
    
    - dapat memiliki satu primary key dalam sebuah tabel sedangkan foreign key dapat memiliki beberapa dalam satu tabel.
    
 - Unnormalized Form

    Unnormalized Form adalah suatu kondisi dimana sebuah tabel yang memiliki rangkap atau data yang terduplikasi.  Unnormalized Form ini sebenarnya adalah kumpulan data data mentah yang dimasukkan semua dalam satu tabel yang sama (tidak dipecah ke tabel lain). Data tersebut di input dengan apa adanya dan tidak dipilah sesuai dengan jenisnya.
    

  - NORMALISASI
  
    proses pengelompokan atribut data yang membentuk entitas sederhana, nonredundan, fleksibel, dan mudah beradaptasi, Sehingga dapat dipastikan bahwa database yang dibuat berkualitas baik.

    
  - 1nf
     
     Suatu relasi disebut memenuhi bentuk normal pertama (1NF) jika dan hanya jika
setiap atribut dari relasi tersebut hanya memiliki nilai tunggal dan tidak ada
pengulangan grup atribut dalam baris. Bentuk 1NF tidak boleh mengandung grup atribut yang berulang.
 Tujuan membentuk 1N

![image](https://user-images.githubusercontent.com/113356785/198860020-1d68eeff-0023-436f-9ea5-aa38aa8ccccc.png)

   - 2nf
   
   Suatu relasi disebut memenuhi bentuk normal kedua (2NF) jika dan hanya jika memenuhi 1NF, setiap atribut yang bukan kunci utama tergantung secara fungsional terhadap semua atribut kunci dan bukan hanya sebagian atribut kunci (fully functionally dependent).

![image](https://user-images.githubusercontent.com/113356785/198860076-7fab9bd8-2d44-44e3-90f1-8c76d29fda9a.png)

![image](https://user-images.githubusercontent.com/113356785/198860086-66ae3800-8b2c-446b-b8cc-12ca02ab5fa5.png)

![image](https://user-images.githubusercontent.com/113356785/198860093-f0ac38e2-2b24-4127-bade-8e7fb081e45a.png)



  - 3nf
  
  Suatu relasi disebut memenuhi bentuk normal ketiga (3NF) jika dan hanya jika memenuhi 2NF, setiap atribut yang bukan kunci tidak tergantung secara fungsional terhadap atribut bukan kunci yang lain dalam relasi tsb (tidak terdapat ketergantungan transitif pada atribut bukan kunci).
  
  Jika suatu relasi sudah memenuhi 2NF tapi tidak memenuhi 3 NF, maka untuk normalisasi ke bentuk 3NF, tabel 2NF didekomposisi menjadi beberapa tabel hingga masing-masing memenuhi 3NF. 
  
![image](https://user-images.githubusercontent.com/113356785/198860497-d81a02f3-0e2e-497b-b4b8-9a33070e9883.png)

![image](https://user-images.githubusercontent.com/113356785/198860508-1c4b90b0-2497-4c5c-9cc1-8bc79d8219b5.png)

![image](https://user-images.githubusercontent.com/113356785/198860514-30181a18-e434-4580-9291-afba97e87dde.png)

![image](https://user-images.githubusercontent.com/113356785/198860521-bbfc091d-13af-4bcc-85b9-6dc5c5d42076.png)




