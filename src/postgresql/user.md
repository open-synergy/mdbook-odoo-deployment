# Membuat User Postgre

1. Buka terminal
2. Login sebagai user **postgres**. Jalankan sintaks berikut di terminal

````bash
sudo su postgres
````

3. <a name="l3">Tentukan</a> username dan password yang akan digunakan untuk membuat user pada postgresql.
4. Buat user postgresql. Jalankan sintaks berikut di terminal:

````bash
createuser --createdb --username postgres --no-createrole --no-superuser --pwprompt nama_user
````

**nama_user** pada sintaks di atas adalah username yang telah ditentukan pada [langkah ke-3](#l3)
5. Keluar dari user **postgres**. Jalankan sintaks berikut di terminal.

````bash
exit
````
