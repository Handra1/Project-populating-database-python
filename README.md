# Project-populating-database-python
This project about learning populating the database in python (In Indonesia)

Create Database and Table:
Pertama, kita akan membuat database dan tabel dengan nama demography, serta membuat hak akses untuk mengelola tabel tersebut. Dari file demography terdapat 6 kolom, yaitu: Kode BPS, Nama, Ibu Kota, Populasi, Luas dan Pulau.
Disini, kita set kolom kode_bps sebagai Primary Key dan untuk membuat tabel demography kita dapat menggunakan perintah create_all(engine). Maka sekarang kita sudah memiliki tabel demography untuk menyimpan data dari file csv tersebut. Kemudian membuat file csv tersebut ke dala lists.
Import List to Table demography:
Setelah memiliki data list tersebut, langkah selanjutnya adalah menginput data tersebut kedalam tabel demography. Disini kita sudah meng-import package insert dan select pada saat membuat database dan tabel, maka kita langsung saja menuliskan perintah query insert ke tabel demography.
Select Data From Table:
Untuk menampilkan data dari tabel, kita gunakan perintah select. Fungsi fetchall() disini untuk menampilkan semua data dari tabel tersebut.
Group by Pulau:
Kita akan menghitung total populasi dari nama pulau berdasarkan kolom pulau dan data diurutkan berdasarkan nama pulau secara alphabet (A-Z). Pertama kita import func dari SQLAlchemy, kemudian kita replace dot separator yang dari kolom nilai populasi terlebih dahulu agar bisa dilakukan perhitungan. Lalu kita hitung total populasi dengan fungsi sum(). Kemudian kita kelompokan hasil query berdasarkan kolom pulau dengan perintah group_by().
Kita simpan hasil query tersebut ke dalam DataFrames dengan menggunakan package Pandas.
