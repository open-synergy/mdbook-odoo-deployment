# Inisiasi Database

#### <a name="langkah1">1. Pastikan working directory berada pada home directory [\<\<USER OS\>\>](/placeholder.md#user-os)</a>

Jalankan sintaks berikut:

```bash
cd ~
````

#### 2. Masuk ke direktori [\<\<PROJECT DIRECTORY\>\>](/placeholder.md#project-directory)

Jalankan sintaks berikut:

````bash
cd <<PROJECT DIRECTORY>>
````

Abaikan langkah ini jika ada sudah berada pada [\<\<PROJECT DIRECTORY\>\>](/placeholder.md#project-directory)

#### 2. Inisiasi Database

Jalankan sintaks berikut:

````bash
sudo docker-compose -f prod.yaml run --rm odoo odoo -i base --without-demo --stop-after-init
````
