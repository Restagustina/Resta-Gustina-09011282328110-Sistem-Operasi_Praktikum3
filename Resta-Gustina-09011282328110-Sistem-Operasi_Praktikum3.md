### Nama : Resta Gustina
### NIM : 09011282328110
### Kelas : SK3B
### Matkul : Sistem Operasi
<br>
<br>
<br>

1. Lihat peralatan I/O, character device, yang ada pada system komputer
   - Melihat block device (peralatan I/O)\
     <img width ="500" alt="1 a" src="https://github.com/user-attachments/assets/2543cd6d-c4ef-4e02-97af-8b812457bf87"> 
   - Melihat character device (peralatan I/O) \
     <img width ="500" alt="1 b" src="https://github.com/user-attachments/assets/b814242f-1109-4324-a7d4-56bbf272f5af">
   - Melihat \
     <img width ="500" alt="1 c" src="https://github.com/user-attachments/assets/246a12fa-d9f7-4358-a312-7cf03767a295"> 
   - Melihat direktori \
     <img width ="500" alt="1 d" src="https://github.com/user-attachments/assets/4126406e-e945-4ab2-9803-6a659ad848df"> 
   - Melihat ordinary file \
     <img width ="500" alt="1 e" src="https://github.com/user-attachments/assets/3d54722e-11a8-400a-b232-72198ed21b98">
     
     #### Penjelasan :

2. Buatlah sub direktori januari, februari dan maret sekaligus pada direktori latihan5
   
     <img width ="500" alt="2 Buat sub direktori januari, februari dan maret" src="https://github.com/user-attachments/assets/b962c732-7a3c-42c6-971e-2767f5147428"> 
     
     #### Penjelasan :
   Untuk membuat subdirektori januari, februari, dan maret secara bersamaan pada direktori latihan5 di command line, Anda dapat menggunakan perintah mkdir dengan opsi -p untuk membuat direktori yang tidak ada dan membuatnya secara bersamaan. Pada perintah mkdir, opsi -p digunakan untuk membuat direktori yang secara bersamaan.

3. Buatlah file dataku yang berisi nama, nim dan alamat anda pada sub direktori januari dan copy-kan file tersebut ke sub direktori februari dan maret\ 
   - Buat file dataku berisi nama, nim dan alamat :
     
<img width ="500" alt="3 buat dataku nama nim" src="https://github.com/user-attachments/assets/a59b82f0-e25a-4061-837d-e29daa1994e9">

 simbol > dan >> memiliki fungsi yang berbeda:\
   - > : digunakan untuk menulis output dari perintah ke sebuah file. Jika file tersebut belum ada, maka perintah akan membuatnya. Jika file sudah ada, maka konten lama file akan dihapus dan digantikan dengan output dari perintah.\
   Contoh : echo "Nama : Resta Gustina" > dataku akan membuat file 'dataku' dengan isi "Nama : Resta Gustina".\
   - >> : Untuk menambahkan output dari perintah ke akhir file yang sudah ada. Jika file belum ada, maka perintah akan membuatnya. Jika file sudah ada, maka konten baru akan ditambahkan ke akhir file.\
   Contoh :  echo "Nama : Resta Gustina" >> dataku akan menambahkan "Nama : Resta Gustina" ke akhir file 'dataku' jika sudah ada, atau membuat file baru jika belum ada.\
   - Copy file 'dataku' dari subdirectori 'januari' ke subdirectori 'februari' dan 'maret' :\
   <img width ="500" alt="cp februari dan maret" src="https://github.com/user-attachments/assets/93c8358d-daf0-4fa5-aed3-61a70947a566">
  
   Setelah menjalankan perintah di atas, Anda akan memiliki file dataku di subdirektori januari, februari, dan maret.\

   ## Untuk melihat isi file dataku :
   - cd januari
     cat dataku
   - cd februari
     cat dataku
   - cd maret
     cat dataku

4. Ubahlah ijin akses file dataku pada sub direktori januari sehingga group dan others dapat melakukan write.
   
  <img width ="500" alt="4 akses januari" src="https://github.com/user-attachments/assets/c95cdbdd-4d49-4584-8b33-b21e02dc2722">
 <img width ="500" alt="akses januari rw" src="https://github.com/user-attachments/assets/14f49fdd-2608-4fea-a453-f3886089407c">

5. Ubahlah ijin akses file dataku pada sub direktori pebruari sehingga user dapat 
melakukan baik write, read maupun execute, tetapi group dan others hanya bisa read dan execute. \
<img width ="500" alt="4 akses februari" ssrc="https://github.com/user-attachments/assets/00e013a9-bc64-409a-a611-27c0e1899eca">
<img width ="500" alt="akses februari rwx" src="https://github.com/user-attachments/assets/a70fd82e-fc46-4f29-8751-a105acc64d48">

6. Ubahlah ijin akses file dataku pada sub direktori maret sehingga semua dapat 
melakukan write, read dan execute.\
<img width ="500" alt="4 akses maret" ssrc="https://github.com/user-attachments/assets/ee236a40-08ca-43df-bcf2-d8e7c0cce104">

7. Hapuslah direktori maret
   <img width ="500" alt="7 rm directory maret" src="https://github.com/user-attachments/assets/b35c2712-9552-4d04-aafb-a438c2d80682">

8. Ubahkan kepemilikan sub direktori februari sehingga user dan group hanya dapat 
melakukan read, dan cobalah untuk membuat direktori baru haha pada sub direktori 
februari\

<img width ="500" alt="no 8" src="https://github.com/user-attachments/assets/cf0ab9c0-c7b1-4ccd-a735-23adb2554c15">


     
<br>
<br>
<br>


