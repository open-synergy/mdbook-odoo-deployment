# Installasi AerooDocs

#### 1. Buka terminal
#### 2. Pastikan Anda login sebagai [user default](../../terminologi.md#user-default)
Abaikan apabila Anda sudah login sebagai user OS yang akan menjalankan Odoo
#### 3. Install Dependensi
```bash
sudo apt-get install python3-pip
sudo pip3 install jsonrpc2 daemonize
```
#### 4. Clone Aeroo Docs dari github
* **Langkah-1:** Masuk ke dalam folder aeroo
```bash
cd /opt/aeroo
```
* **Langkah-2:** Clone modul Aeroo Docs Via github
```bash
sudo git clone https://github.com/aeroo/aeroo_docs.git
```
#### 5. Konfigurasi File Daemon
* **Langkah-1:** Copy dan jalankan file daemon aeroo docs
```bash
sudo python3 /opt/aeroo/aeroo_docs/aeroo-docs start -c /etc/aeroo-docs.conf
```
* **Langkah-2:** Membuat symbolic link untuk file daemon
```bash
sudo ln -s /opt/aeroo/aeroo_docs/aeroo-docs /etc/init.d/aeroo-docs
```
* **Langkah-3:** Edit file daemon
```bash
sudo pico /etc/init.d/aeroo-docs
```
* **Langkah-4:** Tambahkan LSB tags pada Daemon
Copy LSB tags dibawah ini dan paste pada bagian paling atas
```bash
### BEGIN INIT INFO
# Provides:          aeroo-docs
# Required-Start:    $remote_fs $syslog
# Required-Stop:     $remote_fs $syslog
# Default-Start:     2 3 4 5
# Default-Stop:      0 1 6
# Short-Description: aeroo-docs
# Description:       Aeroo Docs daemon
### EDIT INIT INFO
```
#### 6. Jalankan File Daemon sebagai service auto-start
```bash
sudo update-rc.d aeroo-docs defaults
```
#### 7. Menjalankan File Daemon
```bash
sudo service aeroo-docs start
```