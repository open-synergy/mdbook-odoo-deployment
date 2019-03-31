# Pembuatan Daemon

#### 1. Pastikan Anda login sebagai [user default](../terminologi.md#user-default)
#### 2. Pindah ke direktori ```/etc/init.d```

Jalankan sintaks berikut di terminal:
```
cd /etc/init.d
```
#### <a name="l3">3. Download Template File Daemon</a>

Jalankan sintaks berikut di terminal

```bash
wget https://gist.githubusercontent.com/andhit-r/3b161c07216314d0a02ab2e325a1f352/raw/80ce366a2f9b696b231cf95051e2d428baf5a353/odoo-8.0
```

Secara default file daemon akan bernama **odoo-8.0**. Anda bisa mengganti nama file daemon tersebut jika dibutuhkan. Penyebutan **<a name="odoo-daemon-file">odoo-daemon-file</a>** akan merujuk pada nama file yang Anda tentukan pada langkah ini.

#### 5. Sesuaikan File Akses File Daemon

```bash
sudo chmod 755 /etc/init.d/odoo-daemon-file
```

Catatan:

Sesuaikan ```odoo-daemon-file``` dengan nama file daemon yang Anda tentukan pada [langkah ke 3](#l3)

#### 6. Sesuaikan Ownership Dari File Konfigurasi

Jalankan sintaks berikut di terminal

```bash
sudo chown root: /etc/init.d/odoo-daemon-file
```

Catatan:

Sesuaikan ```odoo-daemon-file``` dengan nama file daemon yang Anda tentukan pada [langkah ke 3](#l3)
