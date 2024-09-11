<div align="center">

## LAPORAN PRAKTIKUM SISTEM OPERASI

## SISTEM FILE (FILE SYSTEM)

*Dosen Pengampu :*\
Ahmad Heryanto, M. T.\
Adi Hermansyah, M. T.\
Dr. Ahmad Zarkarsi, M. T.\
Iman Saladin B. Azhar, S. Kom., M. M.SI.\
Sutarno, M.T.

<img width ="200" alt="Logo Universitas Sriwijaya" src="https://github.com/user-attachments/assets/779b597e-6a81-451b-b849-34d7648e8998">

*Disusun Oleh:*\
Nama: Resta Gustina\
NIM : 09011282328110

*JURUSAN SISTEM KOMPUTER*  
*FAKULTAS ILMU KOMPUTER*  
*UNIVERSITAS SRIWIJAYA*  
*2024*
<br>
<br>
<br>
<br>
</div>

1. Lihat peralatan I/O, character device, yang ada pada system komputer
     <img width ="500" alt="1 ls -l  dev" src="https://github.com/user-attachments/assets/075f4e26-81f7-46bb-81e1-21491d823a8e">
     
     #### Penjelasan :
       - Jalankan perintah `ls -l /dev` untuk menampilkan daftar file dan direktori di dalam folder `/dev/`, termasuk perangkat I/O yang menggunakan character device.
       - Perintah ls -l /dev/tty0 untuk melihat informasi detail tentang perangkat /dev/tty0, yang merupakan contoh perangkat I/O yang menggunakan character device.

<br>

2. Buatlah sub direktori januari, februari dan maret sekaligus pada direktori latihan5
   
     <img width ="500" alt="2 Buat sub direktori januari, februari dan maret" src="https://github.com/user-attachments/assets/b962c732-7a3c-42c6-971e-2767f5147428"> 
     
     #### Penjelasan :
         Membuat subdirektori januari, februari, dan maret secara bersamaan pada direktori latihan5 gunakan perintah mkdir dengan opsi -p.
<br>

3. Buatlah file dataku yang berisi nama, nim dan alamat anda pada sub direktori januari dan copy-kan file tersebut ke sub direktori februari dan maret
    >  Buat file dataku berisi nama, nim dan alamat :
     
   <img width ="500" alt="3 buat dataku nama nim" src="https://github.com/user-attachments/assets/a59b82f0-e25a-4061-837d-e29daa1994e9">

    >  Copy file 'dataku' dari subdirectori 'januari' ke subdirectori 'februari' dan 'maret' :
    > Gunakan perintah cp untuk mengcopy
    <img width ="500" alt="cp februari dan maret" src="https://github.com/user-attachments/assets/93c8358d-daf0-4fa5-aed3-61a70947a566">

       Untuk melihat isi file dataku gunakan'cat':
          - cd januari
            cat dataku
          - lakukan hal yang sama untuk februari dan maret 

<br>
4. Ubahlah ijin akses file dataku pada sub direktori januari sehingga group dan others dapat melakukan write.\
      - Gunakan perintah chmod dengan opsi :\
      - g+w: Memberikan hak write kepada grup.\ 
      - o+w: Memberikan hak write kepada orang lain.
     <img width ="500" alt="4 akses januari" src="https://github.com/user-attachments/assets/c95cdbdd-4d49-4584-8b33-b21e02dc2722">
     
  - Verifikasi Hak Akses gunakan perintah ls -l
    
    <img width ="500" alt="akses januari rw" src="https://github.com/user-attachments/assets/14f49fdd-2608-4fea-a453-f3886089407c">

<br>
5. Ubahlah ijin akses file dataku pada sub direktori februari sehingga user dapat melakukan baik write, read maupun execute, tetapi group dan others hanya bisa read dan execute.
   <br>
   <img width ="500" alt="4 akses februari" src="https://github.com/user-attachments/assets/00e013a9-bc64-409a-a611-27c0e1899eca">
   
  #### Penjelasan Opsi chmod :
          >  u=rwx: Memberikan hak read, write, dan execute kepada user.
          >  g=r: Memberikan hak read kepada grup.
          >  o=r: Memberikan hak read kepada orang lain.
     
   > - Verifikasi Hak Akses gunakan perintah ls -l
<img width ="500" alt="akses februari rwx" src="https://github.com/user-attachments/assets/a70fd82e-fc46-4f29-8751-a105acc64d48">

<br>
<br>
6. Ubahlah ijin akses file dataku pada sub direktori maret sehingga semua dapat melakukan write, read dan execute.
   <img width ="500" alt="4 akses maret" src="https://github.com/user-attachments/assets/ee236a40-08ca-43df-bcf2-d8e7c0cce104">
   
   #### Penjelasan Opsi chmod :
      
          >  u=rwx: Memberikan hak read, write, dan execute kepada user.
          >  g=rwx: Memberikan hak read, write, dan execute kepada grup.
          >  o=rwx: Memberikan hak read, write, dan execute kepada orang lain.

<br>
7. Hapuslah direktori maret \
     - perintah 'rmdir' untuk menghapus direktori kosong atau perintah rm -r untuk menghapus direktori beserta isinya.
   <img width ="500" alt="7 rm directory maret" src="https://github.com/user-attachments/assets/b35c2712-9552-4d04-aafb-a438c2d80682">

<br>
<br>
8. Ubahkan kepemilikan sub direktori februari sehingga user dan group hanya dapat melakukan read, dan cobalah untuk membuat direktori baru haha pada sub direktori februari 
<br>
   <img width ="500" alt="no 8" src="https://github.com/user-attachments/assets/cf0ab9c0-c7b1-4ccd-a735-23adb2554c15">

<br>
<br>
9. Modifikasi umask dari file dataku pada sub direktori januari menjadi 027 dan berapakan nilai default-nya ? 
     Penjelasan :
    
     - Umask adalah nilai yang menetapkan izin akses default untuk file dan direktori baru di Linux, seperti read, write, dan execute. 
     - Nilai default umask biasanya adalah 022 yaitu file dan direktori baru yang dibuat akan memiliki hak read dan write untuk user dan grup, tetapi tidak memiliki hak read atau write untuk orang lain.
   <br>  
   <img width ="500" alt="9" src="https://github.com/user-attachments/assets/8a9e37d0-9ad8-4bf5-8d32-cad19e400068">
   
     > nilai umask 027 berarti file dan direktori baru yang dibuat akan memiliki hak read, write, dan execute untuk user, tetapi hanya memiliki hak read dan execute untuk grup dan orang lain.
     
<br>

10. Buatlah link dari file dataku ke file dataku.ini dan file dataku.juga dan dengan perintah list perhatikan berapa link yang terjadi ?
    
   <img width ="500" alt="10" src="https://github.com/user-attachments/assets/f5e80a63-5e7c-4958-b592-a8cb6aab06c5">
    
         - Gunakan perintah ln untuk membuat link simbolik dan hard link
         - ln -s dataku dataku.ini  # Membuat link simbolik
         - ln dataku dataku.j  # Membuat link hard
         - ls -l  # Melihat informasi detail tentang file dan link

     
<br>
<br>
<br>


