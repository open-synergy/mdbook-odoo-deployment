# Pembuatan File Konfigurasi

#### 1. Pastikan Anda login sebagai [user default](../terminologi.md#user-default)
#### 2. Pindah ke direktori ```/etc```

Jalankan sintaks berikut di terminal:
```
cd /etc
```
#### <a name="l3">3.</a> Download Template File Konfigurasi

Jalankan sintaks berikut di terminal

```bash
wget https://gist.githubusercontent.com/andhit-r/67db49ec574d61901cc39a87c537f33a/raw/46b24589e62dfb1bfef69720a568ab4e38587136/odoo-8.0.conf
```

Secara default file konfigurasi akan bernama **odoo-8.0.conf**. Anda bisa mengganti nama file konfigurasi tersebut jika dibutuhkan. Penyebutan **<a name="odoo-daemon-file">odoo-configuration-file</a>** akan merujuk pada nama file yang Anda tentukan pada langkah ini.

#### 4. Sesuaikan Ownership Dari File Konfigurasi

Jalankan sintaks berikut di terminal

```bash
sudo chown odoo: /etc/odoo-configuration-file
```

Catatan:

Sesuaikan ```odoo-configuration-file``` dengan nama file konfigurasi yang Anda tentukan pada [langkah ke 3](#l3)
