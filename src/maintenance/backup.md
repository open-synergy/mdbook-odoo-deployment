# Backup Database

#### 1. Pastikan Anda login sebagai [user odoo](../terminologi.md#user-odoo)
#### 2. Jalankan sintaks berikut:

```bash
pg_dump --host=localhost --port=5432 --username=odoo --password -v --format=c --no-owner --file=path_to_backup_file nama_database
```

Sesuaikan beberapa parameter sintaks di atas:

* ```host``` Alamat postgresql
* ```port``` port dimana service postgresql berjalan
* ```username``` [user odoo](../../terminologi.md#user-odoo)
* ```file``` nama file hasil backup
