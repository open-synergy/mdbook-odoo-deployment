# Menambahkan Repository Modul

#### 1. Pastikan Anda login sebagai [user odoo](../terminologi.md#user-odoo)
#### 2. Pindah ke folder home user odoo

Jalankan sintaks berikut:

```bash
cd ~
```

#### <a name="l3">3.</a> Dapatkan alamat repository modul odoo yang akan ditambahkan

#### <a name="l4">4.</a> Clone repository

Jalankan sintaks berikut di terminal:

```bash
git clone -b <branch> <alamat-repository>
```

Catatan:

* ```branch``` diubah sesuai dengan branch yang dikehendaki. Untuk Odoo v8.0 biasanya menggunakan branch ```8.0```
* ```alamat_repository``` diubah sesuai dengan alamat repository dari [langkah ke-3](#l3)

#### 5. Ulangi [langkah ke-4](#l4) sebanyak repository yang akan ditambahkan

#### <a name="l6">6.</a> Catat folder yang terbuat dari proses clone repository

Proses clone akan membuat sebuah folder yang berisi kumpulan modul odoo. Biasanya nama folder sesuai dengan nama repository.

#### 7. Login sebagai [user default](../../terminologi.md#user-default)

#### 8. Edit [file konfigurasi odoo](./file-konfigurasi.md)

#### 9. Tambahkan daftar addons

Pada parameter ```addons_path```, tambahkan path folder repository yang sudah dicatat pada [langkah ke-6](#l6). Pisahkan masing-masing path folder dengan menggunakan ,

#### 10. Simpan file konfigurasi

#### 11. [Stop service Odoo](../../maintenance/stop-service.md)

#### 12. Pastikan sudah tidak ada service Odoo yang berjalan

Jalankan sintaks berikut:

```bash
ps aux | grep <nama_daemon>
```

Catatan:
* Ubah ```<nama_daemon>``` dengan nama daemon odoo (bukan nama file daemon)

Pastikan tidak ada service odoo yang berjalan di port 8069.

#### 13. (Opsional) Kill manual service Odoo yang tersangkut

Apabila masih ada service Odoo di port 8069 yang tidak mau berhenti. Maka jalankan sintaks berikut:

```bash
sudo kill -KILL <nomor_pid>
```

Catatan:

* Ubah ```<nomor_pid>``` dengan PID odoo yang tersangkut.

#### 14. [Start service Odoo](../../maintenance/start-service.md)
