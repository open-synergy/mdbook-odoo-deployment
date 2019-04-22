# Membuat Init Script untuk OpenOffice (Headless Mode)

#### 1. Buka terminal
#### 2. Pastikan Anda login sebagai [user default](../../terminologi.md#user-default)
Abaikan apabila Anda sudah login sebagai user OS yang akan menjalankan Odoo
#### 3. Membuat file daemon
Jalankan sintaks berikut di terminal:

```bash
sudo pico -w /etc/init.d/office
```
#### 4. Copy dan Paste script dibawah ini:
```bash
#!/bin/bash
### BEGIN INIT INFO
# Provides:          office
# Required-Start:    $remote_fs $syslog
# Required-Stop:     $remote_fs $syslog
# Should-Start:      $network
# Should-Stop:       $network
# Default-Start:     2 3 4 5
# Default-Stop:      0 1 6
# Short-Description: Start daemon at boot time
# Description:       Enable service provided by daemon.
### END INIT INFO

/usr/bin/soffice --nologo --nofirststartwizard --headless --norestore --invisible "--accept=socket,host=localhost,port=8100,tcpNoDelay=1;urp;" &
```
#### 5. Memberikan akses pada file daemon
Jalankan sintaks berikut di terminal:

```bash
sudo chmod +x /etc/init.d/office
```
#### 6. Menjalankan file daemon
Jalankan sintaks berikut di terminal:

```bash
sudo /etc/init.d/office start
```
#### 7. Menambahkan File Daemon kedalam service
Jalankan sintaks berikut di terminal:

```bash
sudo update-rc.d office defaults
```
#### 8. Melakukan pengecekan terhadap File Daemon
Jalankan sintaks berikut di terminal:

```bash
telnet localhost 8100
```
**Hasil:**
```bash
Trying 127.0.0.1...
Connected to localhost.
Escape character is '^]'.
e--'com.sun.star.bridge.XProtocolPropertiesUrpProtocolProperties.UrpProtocolPropertiesTidE--L
```
