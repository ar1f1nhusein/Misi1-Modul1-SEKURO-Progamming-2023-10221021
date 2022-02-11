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
Bekerja dengan sebuah github dapat dilakukan dengan langkah pertama yaitu sign in ke akun github di "https://github.com". Lalu, kita 

<p>&nbsp;</p>

## 3) Github: Branch
Pada dasarnya, branch merupakan sebuah cabang independen tempat kita melakukan suatu proyek. Namun, proyek tersebut tidak akan mengubah cabang di rantai utama. 

<p>&nbsp;</p>

## 4) Github: Fork
Pada dasarnya, fork adalah suatu tindakan menduplikasi suatu repository untuk kemudian kita edit. 

<p>&nbsp;</p>

## 5) Bekerja dengan Git
Untuk bekerja dengan git, maka pertama kita harus mengunduh dulu git pada tautan "https://git-scm/com/". Di sini, pertama-tama kita harus mengaktifkan terlebih dahulu github. Maka ketikkan ini pada terminal/gitbash

```
$ git init
```

Selanjutnya, kita dapat menjadikan sebuah folder menjadi repository. Untuk itu, maka kita dapat ketikkan ini pada terminal/gitbash
```
$ cd <nama folder>
```
Jika terdapat subfolder dalam folder, maka ketikkan ini pada terminal/gitbash setelah menjalankan perintah di atas
```
$ cd <nama subfolder>
```
Setelah itu, buka fas

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

- Pointer akan berubah tanda dari "master" ke "bagian-2" karena kita sudah berpindah branch. Lakukan cara yang sama untuk kembali ke cabang utama.

Lalu, untuk menggabung merge, kita memiliki dua cara yaitu fast forward dan three-way merge. Fast forward dapat terjadi apabila cabang tersebut memiliki jalur langsung dengan cabang yang ingin digabungkan. Sedangkan three-way merge dapat terjadi jika cabang tersebut tidak memiliki jalur langsung dengan cabang yang ingin digabungkan.

Contoh merge fast forward dapat terjadi antara cabang "bagian-1" dengan "master". Ketikkan 

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



