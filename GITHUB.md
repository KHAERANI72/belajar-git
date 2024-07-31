# Instalasi Git Bash
1. download Git pada browser ketik 'git-scm'
	![[foto_23.jpg]] 
2. lalu klik Git Hub yang telah di instal 
3. Lalu akan muncul tampilan seperti gambar
	![[foto_12.jpg]] 
4. Maka klik 'next' terus hingga mendapatkan tampilan seperti gambar
	![[foto_25.jpg]]  

# Login Akun Github
1. Buka aplikasi github di browser
2. Lalu lakukan sign up pada github
	![[foto_19.jpg]]
3. Jika sudah memiliki akun langsung masukkan password dan username yang ada
 ![[foto_20.jpg]] 
4. Jika tidak memiliki akun klik tambahkan akun
	![[foto_22.jpg]]
5. Setelah buat akun maka akan tampil seperti gambar
	![[foto_21.jpg]] 
# Buat Repository
1. jika sudah sign up pada github maka akan tampil seperti gambar
	![[foto_1.PNG]] 
2. Lalu klik 'New repository' maka akan tampil seperti gambar
	![[foto_2.PNG]]
3. Setelah itu tambahkan nama repository yang di inginkan
	![[foto_24.PNG]]
4. Lalu klik 'Create repository' maka repository akan di buat
	 ![[foto_3.PNG]]
5. Setelah membuat repository maka akan tampil seperti gambar
	![[foto_28.jpg]]

# Buat File Lokal 
1. Buka aplikasi visual studio code 
	 ![[foto_45.jpg]]
2. lalu buat folder baru dan file baru pada visual studio code
	  ![[foto_46.jpg]]
# Menghubungkan Git dengan Obsidian
1. buka Git bash yang telah di download
	 ![[foto_47.jpg]] 
2. Membuat folder baru pada obsidian 
	 ![[foto_30.jpg]] 
3. Membuat file obsidian pada folder yang telah dibuat
	![[foto_48.jpg]] 
4. Memasukkan username 
  ```bash
	git config --global user.name "username pada git hub"
    ```
   gambar 
    ![[foto_27.jpg]] 
    *analisis* : 
     1. `git config ` : digunakan untuk mengkonfigurasi pengaturan Git.
     2. `--global` :  perintah yang menunjukkan bahwa pengaturan yang dibuat berlaku untuk semua repositori  pada Git. 
     3. `user.name "username pada git"` : kunci konfigurasi yang menyimpan nama pengguna yang akan digunakan pada GitHub.
5. Memasukkan email 
	code:
   ```bash
   git config --global user.email "email pada git "
   ```

	gambar:
   ![[foto_29 _1.jpg]]

	*analisis* : 
	`git config --global user.email "email pada git "` : digunakan untuk mengatur alamat email yang akan dikaitkan dengan commit di Git untuk semua repositori pada sistem 
6. Menampilkan konfigurasi Git yang aktif  
	code: 
	```bash
	git config --list
	```

	gambar: 
	![[foto_29.jpg]]

	*analisis* : 
	 `git config --list ` : digunakan untuk menampilkan konfigurasi Git yang sedang aktif  
7. Membuka folder obsidian pada git 
	 code:
	```bash
	CD d:\
	```

	gambar: 
	![[foto_31.jpg]] 
8. Menampilkan daftar file dan direktori
	code:
	
	```bash
	 ls
   ```
   
   gambar:
	![[foto_34.jpg]]
	
	*analisis* : 
	 `ls` : digunakan untuk menampilkan daftar file dan direktori dalam direktori kerja saat ini
9. lalu ketik seperti gambar/code 
	```bash
	git init
	```
	
	![[foto_34 - Copy.jpg]]

	*analisis* : 
	`git init` : digunakan untuk menginisialisasi repositori Git baru di dalam direktori 
10. setelah  itu ketik 
	```bash
	git remote add origin 'url'
	```
	
	 ![[foto_35.jpg]]
	*analisis:*
	1. `git remote` : adalah suatu perintah yang digunakan untuk mengelola repositor remote (server Git) yang tehubung pada repositori lokal.
	2. `add` : digunakan untuk menambahkan repositori remote baru. 
	3. `origin` : adalah *nama konvensional* untuk repositori remote utama yang digunakan untuk merujuk pada repositori pusat.
	4. `URL` : adalah URL  repositori yang ingin di tambahkan
11. lalu masukkan kode untuk menambahkan direktori ke Git 
	 code: 
	 ```bash
	 git add .
  ```
  gambar 
  ![[foto_36.jpg]]
  *analisis* : 
   `git add` : digunakan untuk menambahkan perubahan file ke staging area (atau index) sebelum melakukan commit. 
   `.` :  simbol titik menunjukkan ketika ingin menambahkan semua perubahan dari direktori ke staging area.
   
 >[!NOTE]
 >Kesimpulan
 > *staging area* adalah tempat berkumpulnya/ mengumpulkan perubahan yang dimasukkan 
 > Dengan menggunakan `.` sebagai parameter, memastikan bahwa setiap perubahan file dalam direktori akan dimasukkan ke staging area.
 
12.  membuat commit baru pada repositori yang dibuat
    code : 
 ```bash
 git commit -m "nama_commit"
 ```
  gambar
  ![[foto_36 _1.jpg]]
  *analisis* : 
  `git commit` : digunakan untuk menyimpan perubahan dari staging area ke dalam riwayat commit di repositori Git.
  `-m` : digunakan untuk menyertakan pesan commit langsung di baris perintah. 
  `"nama_commit"` : adalah pesan commit yang mendeskripsikan perubahan yang Anda buat.

 > [!NOTE]
 > Kesimpulan
 > `git commit` menyimpan snapshot dari perubahan yang ada di staging area (file yang ditambahkan dengan git add) ke dalam riwayat commit.
 > `-m` memungkinkan untuk memberikan pesan commit tanpa harus membuka editor teks.
 > Pesan commit sebaiknya deskriptif dan memberikan informasi tentang apa yang diubah atau ditambahkan dalam commit 

13. mengirim perubahan dari repositori lokal ke repositori remote
	code 
	```bash 
	git push origin master
  ```
  gambar 
   ![[foto_37.jpg]]
   *analisis* : 
   `git push` : digunakan untuk mengirim perubahan yang telah di-commit dari repositori lokal ke repositori remote.
   `origin` : adalah nama default untuk repositori remote utama yang dikonfigurasi untuk repositori lokal.
   `master` : adalah nama cabang (branch) yang dikirimkan ke repositori remote.

   >[!NOTE]
   >Kesimpulan 
   >`git push`  memperbarui repositori remote dengan commit terbaru dari cabang yang sudah ditentukan.
   >`master` master adalah nama cabang default dalam repositori Git, meskipun beberapa repositori modern mungkin menggunakan nama cabang lain seperti main.

14. setelah itu, tampil halaman login GitHub klik "Sign in with your browser" 
  ![[foto_38.jpg]] 
15. login sesuai username dan password yang telah dibuat pada GitHub
  ![[foto_39.jpg]]
16. setelah login maka muncul tampilan seperti pada gambar
  ![[foto_40.jpg]]
17. pindah ke halaman browser GitHub lalu pilih repositori yang dibuat sebelumnya, maka akan tampil file yang telah dibuat di obsidian 
  ![[foto_41.jpg]]



