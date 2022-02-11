# RANGKUMAN 6

## Git Branch & Merge
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
 
 Sedangkan untuk three-way merge, contohnya terjadi jika kita ingin menggabungkan cabang "bagian-2" dengan cabang hasil gabungan tadi. Posisikan kita di cabang bagian satu dengan perintah "checkout", lalu ketik ini pada terminal.
 ```
 $ git merge bagian-2
 ```
 Maka bagian-2 akan tergabung.

 Selanjutnya, jika kita ingin mengetahui cabang mana saja yang sudah terhubung dengan cabang yang aktif, maka gunakan perintah berikut.
 ```
 $ git branch --merged
 ```
Contoh hasilnya sebagai berikut ini.
![Screen Shot 2022-02-11 at 19 43 49](https://user-images.githubusercontent.com/99285819/153593559-c94747b4-b83f-433c-aeab-f30cfa6c0255.png)
Itu menunjukkan nama-nama cabang yang sudah terhubung dengan cabang utama yang aktif (warna hijau).

 Lalu, jika kalian ingin menghapus suatu cabang, maka gunakan perintah berikut.
 ```
 $ git -d <nama cabang>
 ```
 Jika menggunakan perintah tersebut, biasanya akan terdapat pertanyaan apakah cabang sudah digabungkan atau belum. Namun, jika ingin langsung dihapus, maka gunakan perintah berikut.
 ```
 $ git -D <nama cabang>
 ```
 Hasilnya sebagai berikut.
 ![Screen Shot 2022-02-11 at 19 48 11](https://user-images.githubusercontent.com/99285819/153594149-f38d3807-f879-4ea7-9300-d4afc65d6911.png)

 Terakhir, jika kalian ingin melihat visualisasi dari proyek kalian, maka gunakan perintah berikut.
```
$ git log --all -- decorate --oneline --graph
```
Hasilnya akan menjadi sebagai beriktut.
![Screen Shot 2022-02-11 at 19 52 30](https://user-images.githubusercontent.com/99285819/153594722-af5857e2-ce25-4d70-9cdb-64ccdc4102ce.png)
- Tanda garis-garis menunjukkan visualisasi dari perjalanan proyek kita, mirip dengan apa yang ditampilkan fitur "network" di github.

Namun, mungkin saja cukup melelahkan menulis perintah sepanjang itu, maka kita dapat gunakan alias untuk menyingkatnya dengan perintah berikut.
```
$ alias <nama alias>=" git log --all -- decorate --oneline --graph"
```
Contohnya adalah:
![Screen Shot 2022-02-11 at 20 00 27](https://user-images.githubusercontent.com/99285819/153595801-f85eedc2-6247-427e-b9ad-a5dfb6dba961.png)

Lalu, keluarkan visualnya dengan perintah ini.
```
$ <nama alias>
```
Maka akan keluar tampilan sebagai berikut.
![Screen Shot 2022-02-11 at 20 01 24](https://user-images.githubusercontent.com/99285819/153596005-33e290c6-7178-4176-9843-6712ee6e8d04.png)
- Tampilan yang sama dengan sebelumnya