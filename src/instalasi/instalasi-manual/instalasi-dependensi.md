# Instalasi Dependensi

#### 1. Buka terminal
#### 2. Login sebagai user OS yang akan menjalankan Odoo.
Abaikan apabila Anda sudah login sebagai user OS yang akan menjalankan Odoo. Jalankan sintaks berikut di terminal

```bash
sudo su - nama_user_os -s /bin/bash
```

**nama_user_os** adalah username yang sudah ditentukan pada [prosedur pembuatan user OS](./user-os.md#l3)
Untuk memastikan Anda sudah login sebagai user OS yang benar. Jalankan sintaks berikut di terminal

```bash
who -H
```

Pastikan bahwa nilai dari kolom ```NAME``` pada output yang muncul sama dengan username yang sudah ditentukan pada [prosedur pembuatan user OS](./user-os.md#l3)
#### 3. Pindah ke direktori home dari user OS.
Abaikan apabila Anda sudah berada pada direktori home. Jalankan sintaks berikut di terminal

```bash
cd ~
```

Untuk memastikan Anda sudah berada pada direktori home dari user OS. Jalankan sintaks berikut di terminal:

```bash
pwd
```

Pastikan output yang keluar sama dengan ```/opt/nama_user_os```. **nama_user_os** adalah username yang sudah ditentukan pada [prosedur pembuatan user OS](./user-os.md#l3)

#### 4. Pindah ke Direktori ```odoo```

Jalankan sintaks berikut di terminal:

```bash
cd ~/odoo
```

#### 5. Instalasi Dependensi Odoo

Jalankan sintaks berikut di terminal:

```bash
sudo pip install -r requirement.txt
```
