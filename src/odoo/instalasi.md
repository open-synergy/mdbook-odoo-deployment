# Instalasi

#### <a name="langkah1">1. Pastikan working directory berada pada home directory user OS</a>

Jalankan sintaks berikut:

```bash
cd ~
````
Abaikan langkah ini jika Anda sudah berada pada *home directory*

#### <a name="langkah2">2. Buat direktori untuk meletakan aplikasi</a>

Jalankan sintaks berikut:

````bash
mkdir {nama-folder-odoo}
````

Keterangan placeholder:

* *{nama-folder-odoo}*. Penamaan *{nama-folder-odoo}* disamakan dengan domain production yang akan digunakan.
Apabila domain production yang akan digunakan adalah **latihan.simetri-sinergi.id**,
maka *{nama-folder-odoo}* adalah **latihan1.simetri-sinergi.id**


#### <a name="langkah3">3. Copy aplikasi dengan menggunakan copier</a>

Jalankan sintaks berikut:

```bash
copier copy {alamat-copier-template} {nama-folder-odoo}
```

Keterangan placeholder:

* *{alamat-copier-template}*. URL copier template yang digunakan. Daftar copier template yang dapat digunakan dapat dilihat [disini](../copier-template.md).
* *{nama-folder-odoo}*. Nama folder sesuai dengan *{nama-folder-odoo}* pada [langkah ke-2](./instalasi.md#langkah2)

Jawab pertanyaan-pertanyaan yang muncul. Pertanyaan-pertanyaan yang diajukan tergantung dari template copier yang digunakan.

#### <a name="langkah4">4. Masuk ke direktori {nama-folder-odoo}/odoo/custom/ssh</a>

Jalankan sintaks berikut:

````bash
cd {nama-folder-odoo}/odoo/custom/ssh
````

Keterangan placeholder:

* *{nama-folder-odoo}*. Nama folder sesuai dengan *{nama-folder-odoo}* pada [langkah ke-2](./instalasi.md#langkah2)

#### <a name="langkah5">5. Copy isi ssh private key ke dalam file id_rsa</a>

Jalankan sintaks berikut

````bash
cat {path-to-ssh-private-key} > id_rsa
````

Keterangan placeholder:

* *{path-to-ssh-private-key}*. Path ke file ssh private key yang dibuat sesuai dengan instruksi kerja [Membuat SSH Key](../prasyarat/ssh-key.md)

#### <a name="langkah6">6. Copy isi ssh public key ke dalam file id_rsa</a>

Jalankan sintaks berikut

````bash
cat {path-to-ssh-public-key} > id_rsa.pub
````

Keterangan placeholder:

* *{path-to-ssh-public-key}*. Path ke file ssh public key yang dibuat sesuai dengan instruksi kerja [Membuat SSH Key](../prasyarat/ssh-key.md)

#### <a name="langkah7">7. Build aplikasi</a>

Jalankan sintaks berikut:

````bash
sudo docker-compose -f prod.yaml build --no-cache
````
