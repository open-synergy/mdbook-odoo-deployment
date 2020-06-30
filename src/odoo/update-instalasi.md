# Update Instalasi

#### 1. Masuk ke direktori {nama-folder-odoo}

Jalankan sintaks berikut:

````bash
cd {nama-folder-odoo}
````

Abaikan langkah ini jika ada sudah berada pada {nama-folder-odoo}

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
