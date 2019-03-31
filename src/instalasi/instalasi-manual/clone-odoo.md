# Clone Odoo Codebase

#### 1. Pastikan Anda login sebagai **[user odoo](../../terminologi.md#user-odoo)**
#### 2. Pindah ke direktori home dari [user odoo](../../terminologi.md#user-odoo).
Abaikan apabila Anda sudah berada pada direktori home. Jalankan sintaks berikut di terminal

```bash
cd ~
```

Untuk memastikan Anda sudah berada pada direktori home dari [user odoo](../../terminologi.md#user-odoo). Jalankan sintaks berikut di terminal:

```bash
pwd
```

Pastikan output yang keluar sama dengan ```/opt/user_odoo```. **user_odoo** adalah username yang sudah ditentukan pada [prosedur pembuatan user odoo](./user-os.md#l3)

#### 3. Clone codebase odoo.
Jalankan sintaks berikut di terminal

```bash
git clone -b 8.0 --single-branch https://www.github.com/odoo/odoo.git odoo
```
