Bagian SOAL 7 (No.7A)<br>
Keterangan : Saya menggunakan DBMS MySQL dengan tool phpMyAdmin<br>

1.Kita lihat bahwa terdapat 3 buah tabel dengan ketentuan :<br>
    1). Tabel Nama :<br>
        - id int<br>
        - name varchar(50)<br>
        - id_hobby int<br>
        (gambar.1)<br>
    2). Tabel Hobi :<br>
        - id int<br>
        - name varchar(50)<br>
        - id_category int<br>
        (gambar.2)<br>
    3). Tabel Kategori :<br>
        - id int<br>
        - name varchar(50)<br>
        (gambar.3)<br><br>     
 
 2.Masukkan query sebagai berikut untuk menggabungkan data dari tiga tabel<br>
    atau sering disebut InnerJoin ThreeTables<br>
        SELECT nama.name, hobi.name, kategori.name FROM <br>
        (<br>
          (nama INNER JOIN hobis ON nama.id_hobby = hobi.id)<br>
            INNER JOIN kategori ON nama.id_category = kategori.id<br>
        );<br>
        (gambar.4)(gambar.5)
