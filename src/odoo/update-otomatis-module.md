# Update Otomatis Addons Odoo

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

#### 3. Update otomatis modul-modul Odoo

Jalankan sintaks berikut:

````bash
sudo docker-compose -f prod.yaml run --rm odoo click-odoo-update -d {nama-database}
````

#### 4. Jalankan service odoo

Jalankan sintaks berikut:

````bash
sudo docker-compose -f prod.yaml start odoo
````
