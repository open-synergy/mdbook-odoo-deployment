# Pembuatan Folder Log


#### 1. Pastikan Anda login sebagai [user default](../terminologi.md#user-default)
#### 2. Buat Folder Untuk File Log

Jalankan sintaks berikut di terminal

```bash
sudo mkdir /var/log/odoo
```

#### 3. Sesuaikan Ownership Dari Folder Log

Jalankan sintaks berikut di terminal

```bash
sudo chown -R nama_user_odoo:root /var/log/odoo
```

Catatan:

**user_odoo** adalah [User Odoo](../terminologi.md#user-odoo) yang sudah ditentukan pada prosedur [Pembuatan User Odoo](./user-od.md)
