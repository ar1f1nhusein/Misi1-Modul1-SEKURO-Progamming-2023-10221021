# RANGKUMAN 5

## Bekerja dengan Git
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

Namun, jika kita ingin memindahkan file yang belum di-track ke spacing area, maka gunakan perintah:
```
$ git add .
```

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