# Tugas-6
TUGAS PERTEMUAN 11
Nama	 : Mamat Sutrisno
NIM	 : 312010082
Kelas 	 : TI.20.D1
Matkul	 : Sistem Basis Data

1. Masuk ke databse nama_nim 
- use mamat_312010082;
![1](https://user-images.githubusercontent.com/101656195/171832271-0e8c9f96-1f8c-40be-85fc-78279c9d8fb0.png)

2. Lakukan proses backup dan recovery dengan sql dari database tugas seblumnya 
- SELECT * INTO OUTFILE 'backup_mamatsutrisno_31201082' FROM mamatsutrisno_312010082;
![2](https://user-images.githubusercontent.com/101656195/171832282-7da0e6cc-45a8-4b14-b96c-1d8576da7343.png)

3.Cek file backup pada This PC > Acer (C:) > xampp > mysql > data > mamat_312010082
![3](https://user-images.githubusercontent.com/101656195/171832289-812c2275-463c-4f23-9b08-86c5fb9e524c.png)

4. Menghapus data dan mencoba backup ulang data dengan syntac (LOAD DATA INFILE 'backup_mamatsutrisno_31201082' INTO TABLE mamatsutrisno_312010082;)
![4](https://user-images.githubusercontent.com/101656195/171832295-2304a487-9140-43b5-8f39-0fa00c39aff3.png)

5. Lakukan proses backup dan recovery dengan sqldump dari database tugas seblumnnya 
a. Ketikkan perintah untuk memulai dump database (MySQLDUMP –u root –p mamat_312010082 > backup2.sql)
![5](https://user-images.githubusercontent.com/101656195/171832298-e15eb591-c1da-410f-bbd7-c0d6b395af86.png)

b. Data yang telah di-backup dapat di restrore kembali ke dalam database dengan perintah 
(mysqldump -u root -p mamat_312010082 < c:\xampp\mysql\bin\backup2.sql)
![6](https://user-images.githubusercontent.com/101656195/171832302-97f41ebe-40b5-4ff8-8f24-e19c56da9a68.png)
![7](https://user-images.githubusercontent.com/101656195/171832306-7d3f8c29-87f9-4dd0-bc91-3e3be316cb5c.png)

6. Membuat script cron job untuk melakukan backup otomatis setiap hari minggu jam 12 malam 
 - Jawab : 0 0 * * 7
