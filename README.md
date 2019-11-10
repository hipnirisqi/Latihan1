#latihan 1

instlasi git
-dowload git, buka website resminya git (git-scm.com)
-kemudian unduh git sesuai dengan aarsitektur komputer kita. kalau menggunakan 64 bit,unduh yang 64 bit. begitu juga kalau menggunakan32 bit.
-selamat,git sudah terital di windows. untuk mencobanya, silahakan buka cmd atau power shell, kemudian ketik perintah git --version.berikut tampilan nya:

![](screenshot/langkah%201.jpg)

menambahkan global config
-pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi user.name dan user.emaial
-konfigurasi ini bisa dilakukan untuk global repository atau individual repository
-apabila belium dilakukan konfigurasi,akan mengakibatkan terjadi kegagalan saat menjalankan perintah git commit
-config global repository 
 $ git config --global user.name "nama_user"
 $ git config --global user.email "nama_user"
 ![](screenshot/langkah%202.jpg)

membuat repository local
-buka directory aktif, misal: d\labs_pemrograman1 (buka menggunkan windows explorer)
-klik kanan pada directory aktif tersebut, dan pilih menu Git bash, sehungga muncul git bash commend
-buat directorry project praktukum pertama dengan nama latihan1
 $ mkdir latihan1
 $ cd latihan1
-sehingga terbentuk satu direktori baru dibawahnya, selanjutnya masuk kedalam direktori tersebut dengan perintah cd( change directory) 
-directory aktif menjadi :d\labs_pemrograman1\latihan1
![](screenshot/langkah%203.jpg)

membuat repository local
-jalankan perintah git init, untuk membuat repository local.
$ git init
-repository baru berhasil di inisialisasi, dengan terbentuknya satu direktori hidden dengan nama .git
-pada direktori tersebut, semua perubahan pada working directory akan di simpan
![](screenshot/lankah%204.jpg)

menambah file baru pada repository
-untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif (repository)
-disini kita akan mencoba buat satu file bernama README.md(text file)
$ echo "#lLatihan 1">>README.md
-file README.md berhasil dibuat.
![](screenshot/langkah%205.jpg)

menambahakan file baru pada repository
-untuk menambahakan file yanf baru saja di buat tersebut gunakan perintah git add.
$ git add README.md
-file README.md berhasil ditambahakan
![](screenshot/langkah%206.jpg)

commit(menyimpan perubahan ke database)
-untuk menyimpan perubahan yang ada ke dalam database repository local, gunakan perintah git commit -m"komentar commoit"
$ git commot -m" file pertama saya"
-perubahan berhasil di simpan
![](screeenshot/langakah%207.jpg)

membuat repository server
-server repository yang akan kita gunakan adalah http://github.com
-anda harus membuat akun terlebih dahulu
-pada laman github, klik tombol start a project, atan
-dari menu (icon+)klik tombol repository
![](screenshot/langkah%208.jpg)

membuat repository server
-isi nama repositorynya, misal: labpy1.
-lalu klik tombol creat repository
![](screenshot/langkah%209.jpg)

menambahakan remote repository 
-remote refisitory merupakan resipitory server yang akan di gunakan untuk menyimpan setiap perubahan pada local repository,sehingga dapat di akses oleh banyak user.
-untuk menambahkan remote repisitory server, gianakan perintah git remote add origin [url]
$ git remote add origin http://github.com/hipnirisqi/latihan1.git
![](screenshot/langkah%2010.jpg)

push (mengirim perubahan ke server)
-untuk mengirim perubahan pada local repository ke server gunakan perintah git push
$ git push -u origin master
-perintah inia akan meminta memasuakan username dan password pada akun github.com
![](screenshot/langkah%2011.jpg)

melihat hasilnya pada server repository
-buka lama github.com, arahkan pada repisitorynya
-maka perubahan akan terlihat pada laman tersebut
![](screenshot/langakah%2012.jpg)
