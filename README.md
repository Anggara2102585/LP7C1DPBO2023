# LP7C1DPBO2023
 
## Janji

Saya Apri Anggara Yudha NIM 2102585 mengerjakan soal Latihan7 dalam mata kuliah Desain dan Pemrograman Berorientasi Objek untuk keberkahanNya maka saya tidak melakukan kecurangan seperti yang telah dispesifikasikan. Aamiin.

## Keterangan

Perubahan utama dari template yang disediakan adalah:
- Pengecekan arah gerak player. Setiap perubahan arah dari player, properti prevDir dari Player akan diset ulang. Sehingga Controller dapat mengecek apakah arah player berubah untuk menambahkan score.
- Penambahan class RandomSquare yang meng-extend GameObject. Atribut type diisi "Square", dan terdapat tambahan method yaitu respawn().
- AABB(Axis Align Bounding Box) Collision detection. Collision detection diletakkan pada class Handler dan dipanggil properti loop() saat looping tiap GameObject. Jika Square menyentuh object lain, maka dia akan respawn; kemudian jika yang menyentuhnya adalah Player, maka score bertambah melalui variabel scoreIncrease yang nilainya dapat diambil oleh "si pemanggil handler.loop()" (harus gini karena loop() return void).

## Dokumentasi

Hasil program:

![before](https://user-images.githubusercontent.com/100891594/233843899-06eba528-f900-453d-88a3-e58041d2106c.png)
![after](https://user-images.githubusercontent.com/100891594/233843900-a20cc441-1d72-49b8-ae0b-b7f221fdc1bb.png)
