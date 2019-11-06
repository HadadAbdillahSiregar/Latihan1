# Latihan1
Instalasi Git
pertama download terlebih dahulu git nya di (git-scm.com)
sesuaikan komputer anda tapi saya saran kan memakai yg 64bit jika kalian bisa
selamat kalian sudah selesai mengisntal git .
Menambahkan Config
pada saat pertama kali menggunakan git,perlu dilakukan konfigurasi username dan email
konfigurasi ini bisa dilakukan untuk global repostiry atau individual repository.
jika kalian tidak konfigurasi terlebih dahulu maka akan terjadi error saat menjalan kan perintah git init commit
CONFIG GLOBAL REPO $ git config --global user.name “nama_user” $ git config --global user.email “nama_user”
[1](https://user-images.githubusercontent.com/56785643/68269532-fb11a080-000e-11ea-8bc0-cd5095670e35.PNG)
Membuat Repo lokal
Buka direktory aktif, misal: d:\labs_pemrograman1 (buka menggunakan Windows Explorer)
klik kanan pada direktory aktif tersebut, dan pilih menu Git Bash, sehingga muncul git bash command
Buat direktory project praktikum pertama dengan nama latihan1
$ mkdir latihan1 $ cd latihan1
Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya masuk kedalam direktori tersebut dengan perintah cd (change directory)
direktory aktif menjadi: d:\labs_pemrograman1\latihan1
![2](https://user-images.githubusercontent.com/56785643/68269579-24323100-000f-11ea-8070-9bc7a84e83c5.PNG)
Membuat repo lokal 1.2
jalankan perintah git init,untuk membuat repo lokal
$ git init
Repository baru berhasil di inisialisasi, dengan terbentuknya satu direktori hidden dengan nama .git
Pada direktori tersebut, semua perubahan pada working directory akan disimpan. 
![3](https://user-images.githubusercontent.com/56785643/68269591-38762e00-000f-11ea-843d-89a4dfa7455a.PNG)Menambahkan File baru pada repository
Untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif (repository)
disini kita akan coba buat satu file bernama README.md (text file)
$ echo “#Latihan 1” >> README.md
File README.md berhasil dibuat.
![4](https://user-images.githubusercontent.com/56785643/68269628-53e13900-000f-11ea-939a-8db2f873d7d6.PNG)
Menambahkan File baru pada repository
Untuk menambahkan file yang baru saja dibuat tersebut gunakan perintah git add.
File README.md berhasil ditambahkan.
$ git add README.md
![5](https://user-images.githubusercontent.com/56785643/68269650-652a4580-000f-11ea-8813-2080a47e0a20.PNG)
Commit (Menyimpan perubahan ke database)
Untuk menyimpan perubahan yang ada kedalam database repository local, gunakan perintah git commit -m “komentar commit”
Perubahan berhasil disimpan.
$ git commit -m “File pertama saya”
![6](https://user-images.githubusercontent.com/56785643/68269661-72473480-000f-11ea-9b1d-bca3707d6ee1.PNG)
Menambahkan Remote Repository
Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.
Untuk menambahkan remote repository server, gunakan perintah git remote add origin [url]
$ git remote add origin
![7](https://user-images.githubusercontent.com/56785643/68269677-868b3180-000f-11ea-9529-a87f39a1e584.PNG)
Push (Mengirim perubahan ke server)
Untuk mengirim perubahan pada local repository ke server gunakan perintah git push.
Perintah ini akan meminta memasukkan username dan password pada akun github.com
$ git push -u origin master
![8](https://user-images.githubusercontent.com/56785643/68269692-96a31100-000f-11ea-83cb-c934fc24ddf0.PNG)
