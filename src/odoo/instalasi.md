# Instalasi

#### 1. Pastikan working directory berada pada home directory user OS

Jalankan sintaks berikut:

```bash
cd ~
````
Abaikan langkah ini jika Anda sudah berada pada *home directory*

#### 2. Buat direktori untuk meletakan aplikasi

Jalankan sintaks berikut:

````bash
mkdir {nama-folder-odoo}
````

Penamaan {nama-folder-odoo} disamakan dengan domain production yang akan digunakan.
Apabila domain production yang akan digunakan adalah **latihan.simetri-sinergi.id**,
maka {nama-folder-odoo} adalah **latihan1.simetri-sinergi.id**


#### 3. Copy aplikasi dengan menggunakan copier

Jalankan sintaks berikut:

```bash
copier copy {alamat-copier-template} {nama-folder-odoo}
```
Jawab pertanyaan-pertanyaan yang muncul. Pertanyaan-pertanyaan yang diajukan tergantung dari template copier yang digunakan.
Daftar copier template yang dapat digunakan dapat dilihat disini.

#### 4. Masuk ke direktori {nama-folder-odoo}/odoo/custom/ssh

Jalankan sintaks berikut:

````bash
cd {nama-folder-odoo}/odoo/custom/ssh
````

#### 5. Copy isi ssh private key ke dalam file id_rsa

Jalankan sintaks berikut

````bash
cat {path-to-ssh-private-key} id_rsa
````

#### 6. Copy isi ssh public key ke dalam file id_rsa

Jalankan sintaks berikut

````bash
cat {path-to-ssh-public-key} id_rsa.pub
````

#### 7. Build aplikasi

Jalankan sintaks berikut:

````bash
sudo docker-compose -f prod.yaml build --no-cache
````
