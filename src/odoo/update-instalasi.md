# Update Instalasi

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

#### 3. Update Copier Template

Jalankan sintaks berikut:

````bash
copier update
````
