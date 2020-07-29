# Instalasi Addons Odoo

#### 1. Masuk ke direktori *{nama-folder-odoo}*

Jalankan sintaks berikut:

````bash
cd {nama-folder-odoo}
````

Keterangan placeholder:

* *{nama-folder-odoo}*. Nama folder sesuai dengan *{nama-folder-odoo}* pada [langkah ke-2 halaman instalasi](./instalasi.md#langkah2)

Abaikan langkah ini jika ada sudah berada pada *{nama-folder-odoo}*

#### 2. Hentikan service odoo

Jalankan sintaks berikut:

````bash
sudo docker-compose -f prod.yaml stop odoo
````

#### 3. Tentukan modul-modul yang akan diinstall

Jalankan sintaks berikut untuk menentukan modul yang diinstall secara manual:

````bash
modules=modul-1,modul-2,modul-3,...,modul-n
````

atau

Jalankan sintaks berikut untuk menginstall modul-modul yang telah didefinisikan dalam file tertentu

````bash
modules=$(<{path-to-file})
````

Keterangan placeholder:

* *{path-to-file}*. Path ke file yang berisi daftar modul yang akan diinstall.

#### 4. Instalasi modul-modul Odoo

Jalankan sintaks berikut:

````bash
sudo docker-compose -f prod.yaml run --rm odoo odoo -i $modules --without-demo --stop-after-init
````

#### 5. Jalankan service odoo

Jalankan sintaks berikut:

````bash
sudo docker-compose -f prod.yaml start odoo
````
