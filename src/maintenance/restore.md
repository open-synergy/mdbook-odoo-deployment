# Restore Database

#### 1. Pastikan Anda login sebagai [user odoo](../terminologi.md#user-odoo)
#### 2. Jalankan sintaks berikut:

```bash
pg_restore --host=<address_postgresql> --port=<port_postgresql> --username=<user_yang_menjalankan_odoo> --password --format=c --no-owner -v --dbname=<nama_database> <path_to_backup_file>
```

Sesuaikan beberapa parameter sintaks di atas:

* ```address_postgresql``` Alamat postgresql
* ```port_postgresql``` port dimana service postgresql berjalan
* ```user_yang_menjalankan_odoo``` [user odoo](../../terminologi.md#user-odoo)
* ```nama_database``` nama database hasil restore
* ```path_to_backup_file``` path ke file backup postgre
