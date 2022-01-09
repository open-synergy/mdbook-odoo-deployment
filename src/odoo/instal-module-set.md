# Instal Module Set

#### <a name="langkah1">1. Pastikan working directory berada pada home directory [\<\<USER OS\>\>](/placeholder.md#user-os)</a>

Jalankan sintaks berikut:

```bash
cd ~
````

#### <a name="langkah2">2. Masuk ke [\<\<PROJECT DIRECTORY\>\>](/placeholder.md#project-directory)</a>

Jalankan sintaks berikut:

```bash
cd <<PROJECT DIRECTORY>>
````

Abaikan langkah ini jika working directory sudah berada pada [\<\<PROJECT DIRECTORY\>\>](/placeholder.md#project-directory)

#### <a name="langkah3">3. Tentukan Modul Set Yang Akan Diinstal</a>

Jalankan sintaks berikut:

````bash
modules=$(<module-set/nama-set.txt)
````

Sesuaikan nama-set.txt dengan set module yang akan diinstal. Daftar file module set dapat dilihat pada direktori \<\<PROJECT DIRECTORY\>\>/module-set

#### <a name="langkah3">4. Install Modul</a>

Jalankan sintaks berikut:

````bash
sudo docker-compose -f prod.yaml run --rm odoo odoo -i $modules --without-demo --stop-after-init
````
