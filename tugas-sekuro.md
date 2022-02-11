# TUGAS URO MODUL 1 PROGRAMMING

<p>&nbsp;</p>

## Penulis
### 16021048 - Muhammad Arifin Husein

<p>&nbsp;</p>

## Daftar Isi
1. [Apa itu Git & Github?](https://youtu.be/lTMZxWMjXQU)
2. [Bekerja dengan Github](https://youtu.be/Q3Id0DgcrXY)
3. [Github: Branch](https://youtu.be/k1QXd-8VbPY)
4. [Github: Fork](https://youtu.be/8rry2ncZmfg)
5. [Bekerja dengan Git](https://youtu.be/e-6OkXRqWaE)
6. [Git Branch & Merge](https://youtu.be/EGl7KxVOyNs)
7. [Gitignore](https://youtu.be/LK3kX4n-vLM)

<p>&nbsp;</p>

## 1) Apa itu Git & Github
Git merupakan salah satu VCS (Visual Control System) yang tersedia pada komputer. Fungsi dari git adalah menyediakan fasilitas agar kita dapat bekerja sama secara tim, spesifiknya adalah saat kita melakukan pekerjaan dengan coding. Github sendiri merupakan aplikasi online yang dapat kia gunakan untuk menggunakan git itu sendiri tanpa mengunduhnya terlebih dahulu. Pada git terdapat beberapa istilah sebagai berikut.

- Respository, semacam folder yang tempat kita menyimpan file pada Git

- Commit, rekaman/snapshot dari repository

- Hash, penanda unik pada sebuah commit, biasanya berupa kombinasi angka dan huruf seperti kode.

- Checkout, berpindah ke sebuah commit

- Branch, percabangan bebas dari sebuah commit

- Merge, penggabungan beberapa branch

- Remote, sumber yang memiliki repository

- Clone, mengambil repository dari remote

- Push, mengirimkan commit ke repository

- Pull, mengambil commit dari repository

<p>&nbsp;</p>


## 2) Bekerja dengan Github
Bekerja dengan sebuah github dapat dilakukan dengan langkah pertama yaitu sign in ke akun github di "https://github.com". Setelah itu, kita harus memberi nama dari repository terlebih dahulu. Lalu, kita dapat melakukan berbagai hal dengan website tersebut. Kita bisa mulai membuat file suatu proyek di repository yang kita buat, namun kita harus selalu "commit" setiap perubahan pada proyek atau repository yang kita lakukan dengan memberikan keterangan perubahan apa yang dilakukan, tujuannya adalah agar tidak membingungkan pemilik asli dari proyek tersebut. Kita bisa melihat commit yang dilakukan pada repository atau file tersebut berdasarkan fitur "history" atau "commits", dan di fitur "network" pada menu "insights" dapat memperlihatkan kita "commit" yang disimbolkan titik hitam pada proyek yang kita lakukan.

<p>&nbsp;</p>

## 3) Github: Branch
Pada dasarnya, branch merupakan sebuah cabang independen tempat kita melakukan suatu proyek. Namun, proyek tersebut tidak akan mengubah cabang di rantai utama. Suatu repository selalu memiliki "main branch" atau cabang utama, dan dari cabang utama tersebut, dapat dibuat bercabang-cabang dengan nama yang berbeda, namun cabang-cabang tersebut tidak akan memengaruhi cabang utama. Cabang tersebut dapat kita katakan sebagai tempat mengerjakan proyek dari cabang utama, namun pada saat pengerjaan tidak akan mengubah proyek aslinya, mirip dengan duplikat. Namun, bila kita sudah yakin, maka kita bisa menggabungkannya ke cabang utama atau kita sebut sebagai "merge", ini akan memodifikasi proyek asli yang dimiliki. Branch dapat dilakukan dengan memilih pilihan "create new branch" sebelum melakukan "commit" dan memberi nama "commit" tersebut. Cabang yang sudah matang dapat kita "pull request" pada pemilik cabang utama, meskipun itu diri kita sendiri. Jika sudah, maka di cabang utama atau "branch master" akan ada pesan "pull request", dan dapat langsung di-"merge" jika disetujui. Namun, terkadang ada juga "merge conlict" karena adanya beberapa masalah saat merge, seperti misalnya penggantian baris yang sama oleh beberapa cabang, maka kita harus diselesaikan atau "resolve" terlebih dahulu untuk melakukannya. Jika sudah berhasil, maka di visualisasi pada fitur "network" akan terdapat cabang dari cabang utama, itu adalah bukti adanya cabang atau "branch" dari proyek atau cabang utama, dan jika ada gambar cabang bergabung, itu artinya sudah dilakukan "merge".

<p>&nbsp;</p>

## 4) Github: Fork
Pada dasarnya, "fork" adalah suatu tindakan menduplikasi suatu repository milik akun lain untuk kemudian kita edit, ini berguna jika kita ingin melakukan kontribusi terhadap repository milik orang lain. Kita bisa melihat repository akun lain terlebih dahulu, lalu fork file yang ingin kita edit. Setelah itu, kita bisa melakukan "pull request" kepada akun orang tersebut dan menentukan cabang mana dari akun orang tersebut yang ingin kita tambahkan dari perubahan yang kita lakukan, lalu pemilik akun tersebut dapat melakukan "merge" dari perubahan yang dilakukan pelaku "fork" dan melengkapi repository yang dimiliki.

<p>&nbsp;</p>

## 5) Bekerja dengan Git
Untuk bekerja dengan git, maka pertama kita harus mengunduh dulu git pada tautan "https://git-scm/com/". 

Untuk mengetahui nama user, kita bisa ketikkan
```
$ pwd
```
Tampilan sebagai berikut.
![Screen Shot 2022-02-11 at 18 54 35](https://user-images.githubusercontent.com/99285819/153587155-82926b61-ee74-48fe-ab7d-48c9d6af801e.png)


Di sini, pertama-tama kita harus mengaktifkan terlebih dahulu github. Maka ketikkan ini pada terminal/gitbash

```
$ git init
```

Selanjutnya, kita dapat menjadikan sebuah folder menjadi repository. Untuk itu, maka kita dapat ketikkan ini pada terminal/gitbash
```
$ cd <nama folder>
```
Untuk mengecek ada subfolder/file apa saja dalam suatu folder, maka kita bisa gunakan perintah berikut.
```
$ ls
```
Hasilnya ditunjukkan sebagai berikut.
![Screen Shot 2022-02-11 at 18 59 37](https://user-images.githubusercontent.com/99285819/153587989-85d14eb4-fe01-499a-9e74-554bb6da84de.png)

Jika terdapat subfolder dalam folder, maka ketikkan ini pada terminal/gitbash setelah menjalankan perintah di atas
```
$ cd <nama subfolder>
```
Setelah itu, buka source code editor, misalkan seperti VS Code untuk membuat proyek. Kita bisa membuat file dalam repository tersebut dan mulai mengeditnya. Untuk mengecek file apa yang kita punya dalam repository tersebut, kita dapat ketikkan ini.
```
$  git status
```
Hasilnya sebagai berikut.
![Screen Shot 2022-02-11 at 17 55 53](https://user-images.githubusercontent.com/99285819/153579939-416cbbc7-3c60-4230-a897-a44de0a9bb61.png)

File berwarna merah menunjukkan file yang belum di-track atau dimasukkan ke staging area pada git. Untuk dimasukkan, ketikkan ini pada terminal.
```
$ git add <nama file>
```
Setelah itu, jika dilihat lagi status dari folder, maka hasilnya sebagai berikut.
![Screen Shot 2022-02-11 at 18 01 03](https://user-images.githubusercontent.com/99285819/153580579-b8a9f705-6243-4fba-9054-77037984bdb0.png)
Itu artinya file sudah berhasil dimasukkan ke staging area. 
- Langkah yang sama harus dilakukan apabila kita memodifikasi suatu file dalam repository meskipun sudah di-track sebelumnya, ini disebabkan adanya perubahan yang harus di-add kembali.

Selanjutnya, setiap perubahan pada folder harus dilakukan "commit". Untuk melakukan "commit", ketikkan berikut.
```
$ git commit -m "<pesan commit>"
```
Pesan commit harus ditambahkan untuk memberikan keterangan. Hasilnya adalah berikut.
![Screen Shot 2022-02-11 at 18 26 21](https://user-images.githubusercontent.com/99285819/153583792-b55010d6-1f5b-4579-9e25-1b650e8ed574.png)

Jika kita ingin melihat semua commit yang telah kita lakukan, maka ketikkan berikut.
```
$ git log
```
Hasilnya adalah sebagai berikut.
![Screen Shot 2022-02-11 at 18 31 36](https://user-images.githubusercontent.com/99285819/153584403-ac2b3b8f-b7a3-4cef-a0a5-b589292c571c.png)

Namun, jika kita ingin melihat hanya beberapa "commit" terakhir, maka ketikkan berikut.
```
$ git log -<jumlah commit terakhir yang diinginkan>
```
Contohnya adalah sebagai berikut.
![Screen Shot 2022-02-11 at 18 34 35](https://user-images.githubusercontent.com/99285819/153584787-0840825c-b843-444b-83ea-d4248da07852.png)

- Pada foto itu, yang berwarna kuning kehitaman adalah "hash" sebagai penanda dari "commit" yang kita lakukan.

Selanjutnya, apabila kita ingin mengetahui jumlah "commit" spesifik untuk suatu file dalam repository, maka ketikkan berikut.
```
$ git lof -- <nama file>
```
Contohnya sebagai berikut.
![Screen Shot 2022-02-11 at 18 41 50](https://user-images.githubusercontent.com/99285819/153585641-e408a962-152f-44b7-9e29-62d1913b32c0.png)

Terakhir, kalau misalkan kalian ingin mengembalikan perubahan suatu file pada suatu "commit", maka ketikkan hal berikut.
```
$ git checkout <5 kode pertama dari "hash" suatu "commit"> -- <nama file>
```
Contohnya misalkan kita mencari tahu daftar commit pada file "tes-git" sebagai berikut.
![Screen Shot 2022-02-11 at 18 47 35](https://user-images.githubusercontent.com/99285819/153586298-d0c3d3a6-50ca-4758-9c38-9bed7d4ec69d.png)

Lalu, setelah menggunakan perintah tadi, kita ingin mencari tahu keadaan ketika "commit" pertama, maka hasilnya seperti ini.
![Screen Shot 2022-02-11 at 18 50 25](https://user-images.githubusercontent.com/99285819/153586691-797f4c00-d483-4cf7-8b8a-51ecaae3aeb2.png)
File pun akan kembali pada keadaan tersebut.

<p>&nbsp;</p>

## 6) Git Branch & Merge
Pada git, branch dapat dibuat sebagai berikut. Dalam hal ini, misalkan saya ingin membuat branch dengan nama "bagian-1" dan "bagian-2"
```
$ git branch <bagian-1>
$ git branch <bagian-2>
```
Untuk melihat semua cabang, ketikkan:
```
$ git branch
```
![Screen Shot 2022-02-11 at 14 23 32](https://user-images.githubusercontent.com/99285819/153551977-bc64721f-40a2-4aa5-a8cb-8d15020e32cd.png)
- Pointer berada pada cabang "master" karena itu merupakan cabang utama.

Lalu, misalkan kita ingin berpindah cabang ke bagian-1, maka ketikkan pada terminal/gitbash
```
$ git checkout <bagian-1>
```
Maka cabang akan berpindah, dan jika kita lalu melihat seluruh cabang, maka hasilnya seperti berikut.
![Screen Shot 2022-02-11 at 14 27 28](https://user-images.githubusercontent.com/99285819/153552367-2323e95f-f1db-4e2f-9f8b-7620452d2652.png)

- Pointer akan berubah tanda dari "master" ke "bagian-1" karena kita sudah berpindah branch. Lakukan cara yang sama untuk kembali ke cabang utama.

Lalu, untuk menggabung merge, kita memiliki dua cara yaitu fast forward dan three-way merge. Fast forward dapat terjadi apabila cabang tersebut memiliki jalur langsung dengan cabang yang ingin digabungkan. Sedangkan three-way merge dapat terjadi jika cabang tersebut tidak memiliki jalur langsung dengan cabang yang ingin digabungkan.

Contoh merge fast forward dapat terjadi antara cabang "bagian-1" dengan "master" (Untuk saat ini, posisi adalah cabang "master"). Ketikkan ini pada terminal:
```
$ git merge bagian-1
```
 
 Sedangkan untuk three-way merge, contohnya terjadi jika kita ingin menggabungkan cabang "bagian-2" dengan cabang "bagian-1". Posisikan kita di cabang bagian satu dengan perintah "checkout", lalu ketik ini pada terminal.
 ```
 $ git merge bagian-2
 ```
 Maka bagian-1 dan bagian-2 akan tergabung.

<p>&nbsp;</p>

## 7) Gitignore
Gitignore merupakan langkah yang dapat dilakukan agar kita tidak memasukkan suatu file dengan karakteristik tertentu dari working tree menuju staging area. Gitignore dapat dilakukan dengan membuat file atau folder berjudul berikut:
```
.gitignore
```

Dengan mendaftarkan file-file atau folder-folder yang tidak diinginkan ke dalam gitignore, maka file tersebut tidak akan dimasukkan ke dalam staging area saat di add pada terminal, misal jika saya mendaftarkan file "script.md" pada gitignore, hasilnya akan seperti berikut:



Sebelum menggunakan gitignore:

![Screen Shot 2022-02-11 at 13 32 33](https://user-images.githubusercontent.com/99285819/153547610-cf43d79c-e4a4-4f9d-9c93-642d0af231de.png)



Setelah menggunakan gitignore:
![Screen Shot 2022-02-11 at 13 38 13](https://user-images.githubusercontent.com/99285819/153547642-87787624-a750-46b3-a502-a18d06d29011.png)

Dapat dilihat bahwa file "script.md" menghilang begitu digunakan gitignore.


* Gitignore hanya berfungsi untuk file yang belum ditrack atau dimasukkan ke staging area, jika sudah dimasukkan, maka file harus di "unstage" agar dapat diabaikan oleh gitignore, maka pastikan file belum ditrack oleh git sebelum menggunakan gitignore

<p>&nbsp;</p>

# Terima kasih, semoga kalian bahagia selalu ;)



