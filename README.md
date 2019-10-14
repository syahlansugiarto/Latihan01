#Latihan 1

	Menambahkan Global Config
- Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi
user.name dan user.email
• konfigurasi ini bisa dilakukan untuk global repostiry atau individual
repository.
• apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi
kegagalan saat menjalankan perintah git commit
• Config Global Repository
$ git config --global user.name “nama_user”
$ git config --global user.email “nama_user”

![ettt1](https://user-images.githubusercontent.com/44828458/66756220-bbe6a880-eec3-11e9-9d9d-0343d8064088.png)

	Membuat Reposiory Local
• Buka direktory aktif, misal: d:\labs_pemrograman1 (buka
menggunakan Windows Explorer)
• klik kanan pada direktory aktif tersebut, dan pilih menu Git Bash,
sehingga muncul git bash commad
• Buat direktory project praktikum pertama dengan nama latihan1
• Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya
masuk kedalam direktori tersebut dengan perintah cd (change
directory)
• direktory aktif menjadi: d:\labs_pemrograman1\latihan1
$ mkdir latihan1
$ cd latihan1

![oiiiiiiiiiiii1235](https://user-images.githubusercontent.com/44828458/66757866-45e44080-eec7-11e9-962e-a2fd0c9f2af9.png)

	Membuat Reposiory Local
• Jalankan perintah git init, untuk membuat repository local.
• Repository baru berhasil di inisialisasi, dengan terbentuknya satu
direktori hidden dengan nama .git
• Pada direktori tersebut, semua perubahan pada working directory
akan disimpan.
$ git init

![gitiu 2-](https://user-images.githubusercontent.com/44828458/66757526-94450f80-eec6-11e9-8ec5-10004cac48a9.png)

	Menambahkan File baru pada repository
• Untuk membuat file dapat menggunakan text editor, lalu menyimpan
filenya pada direktori aktif (repository)
• disini kita akan coba buat satu file bernama README.md (text file)
• File README.md berhasil dibuat.
$ echo “#Latihan 1” >> README.md

![redme `](https://user-images.githubusercontent.com/44828458/66758246-1b46b780-eec8-11e9-8b40-52d071a2188c.png)

	Menambahkan File baru pada repository
• Untuk menambahkan file yang baru saja dibuat tersebut gunakan
perintah git add.
• File README.md berhasil ditambahkan.
$ git add README.md

![redme 34](https://user-images.githubusercontent.com/44828458/66758725-11718400-eec9-11e9-82fb-fc36d70689e9.png)

	Commit (Menyimpan perubahan ke database)
• Untuk menyimpan perubahan yang ada kedalam database repository
local, gunakan perintah git commit -m “komentar commit”
• Perubahan berhasil disimpan.
$ git commit -m “File pertama saya”

![comit](https://user-images.githubusercontent.com/44828458/66758579-bb9cdc00-eec8-11e9-864d-2dadd7c2f23a.png)

	Membuat repository server
• Server reopsitory yang akan kita gunakan adalah http://github.com
• Anda harus membuat akun terlebih dahulu.
• Pada laman github, klik tombol start a project, atau
• Dari menu (icon +) klik New Repository


	Membuat repository server
• Isi nama repositorynya, misal: labpy1.
• lalu klik tombol Create repository

	Menambahkan Remote Repository
• Remote Repository merupakan repository server yang akan
digunakan untuk menyimpan setiap perubahan pada local repository,
sehingga dapat diakses oleh banyak user.
• Untuk menambahkan remote repository server, gunakan perintah
git remote add origin [url]
$ git remote add origin https://github.com/syahlansugiarto/Latihan01.git


	Push (Mengirim perubahan ke server)
• Untuk mengirim perubahan pada local repository ke server gunakan
perintah git push.
• Perintah ini akan meminta memasukkan username dan password
pada akun github.com
$ git push -u origin master

![push 1](https://user-images.githubusercontent.com/44828458/66759244-17b43000-eeca-11e9-8219-b7d344a4f9b7.png)

	Melihat hasilnya pada server repository
• Buka laman github.com,
arahkan pada repositorinya.
• Maka perubahan akan
terlihat pada laman
tersebut

	Clone Repository
• Clone repository, pada dasarnya adalah meng-copy repository server
dan secara otomatis membuat satu direktory sesuai dengan nama
repositorynya (working directory).
• Untuk melakukan cloning, gunakan perintah git clone [url]

![clone 1](https://user-images.githubusercontent.com/44828458/66759455-7d082100-eeca-11e9-91f4-c1a713e53ebc.png)

	Kegunaan file README.md
• Apabila kita menggunakan github, untuk memberikan penjelasan
awal pada project yang kita buat, maka dapat menggunakan sebuah
file yang bernama README.md
• Pada file tersebut kita dapat membuat dokumentasi awal dari setiap
project yang kita buat untuk memberikan penjelasan atau sekedar
cara penggunaan dari aplikasi yang kita kembangkan.
• Penulisan file README.md berbasis teks, dan untuk pemformatannya
menggunakan Markdown format.
• untuk lebih jelasnya, dapat anda pelajari cara penggunaan markdown
pada url berikut: https://guides.github.com/features/masteringmarkdown/


