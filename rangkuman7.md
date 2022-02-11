# RANGKUMAN 7

## Gitignore
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
