# Clone Modul Aeroo Reports dari Github

#### 1. Buka terminal
#### 2. Pastikan Anda login sebagai **[user odoo](../../terminologi.md#user-odoo)**
#### 3. Pindah ke direktori home dari [user odoo](../../terminologi.md#user-odoo).
Abaikan apabila Anda sudah berada pada direktori home. Jalankan sintaks berikut di terminal

```bash
cd ~
```

Untuk memastikan Anda sudah berada pada direktori home dari [user odoo](../../terminologi.md#user-odoo). Jalankan sintaks berikut di terminal:

```bash
pwd
```

Pastikan output yang keluar sama dengan ```/opt/user_odoo```. **user_odoo** adalah username yang sudah ditentukan pada [prosedur pembuatan user odoo](./user-os.md#l3)
#### 4. Clone codebase odoo.
Jalankan sintaks berikut di terminal

```bash
git clone -b 8.0 https://github.com/aeroo/aeroo_reports.git
```
#### 5. Tambahkan addons_path aeroo_report pada file konfigurasi odoo

```bash
addons_path = [...],/opt/odoo/aeroo_reports
```