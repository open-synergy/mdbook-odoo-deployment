# Instalasi

#### <a name="langkah1">1. Pastikan working directory berada pada home directory user OS</a>

Jalankan sintaks berikut:

```bash
cd ~
````
Abaikan langkah ini jika Anda sudah berada pada *home directory*

#### <a name="langkah2">2. Clone aplikasi inverseproxy</a>

Jalankan sintaks berikut:

````bash
git clone https://github.com/open-synergy/docker-compose-inverseproxy.git {nama-folder-inverse-proxy}
````

Keterangan placeholder:

* *{nama-folder-inverse-proxy}*. Nama folder yang akan dibuat untuk menyimpan kode inverseproxy. Nama folder bebas.

#### <a name="laangkah3">3. Masuk ke direktori {nama-folder-inverse-proxy}</a>

Jalankan sintaks berikut:

````bash
cd {nama-folder-inverse-proxy}
````

Keterangan placeholder:

* *{nama-folder-inverse-proxy}*. Nama folder tempat menyimpan kode inverseproxy. Harus sesuai dengan nama folder pada [langkah ke-2](./instalasi.md#langkah2)


#### <a name="langkah4">4. Sesuaikan nilai ACME.Email pada file inverseproxy.yaml</a>

Ubah nilai ACME.Email pada file inverseproxy.yaml menjadi alamat email yang valid.
