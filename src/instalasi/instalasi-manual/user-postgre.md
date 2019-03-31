# Membuat User Pada Postgre

#### 1. Pastikan Anda login sebagai ```postgres```
#### 2. <a name="l2">Tentukan</a> username dan password yang akan digunakan untuk membuat user postgresql
#### 3. Buat user postgresql

Jalankan sintaks berikut di terminal:

````bash
createuser --createdb --username postgres --no-createrole --no-superuser --pwprompt nama_user_postgresql
````

Catatan:

```nama_user_postgresql``` pada sintaks di atas adalah username yang telah ditentukan pada [langkah ke-2](#l2)
