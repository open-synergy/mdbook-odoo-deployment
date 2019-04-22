# Installasi Aeroolib

#### 1. Buka terminal
#### 2. Pastikan Anda login sebagai [user default](../../terminologi.md#user-default)
Abaikan apabila Anda sudah login sebagai user OS yang akan menjalankan Odoo
#### 3. Clone Aeroolib Via Github
* **Langkah-1:** Membuat folder baru untuk aeroolib.

```bash
sudo mkdir /opt/aeroo
```
* **Langkah-2:** Masuk ke dalam folder yang sudah dibuat pada proses diatas.

```bash
cd /opt/aeroo
```
* **Langkah-3:** Clone modul aeroolib via github.

```bash
sudo git clone https://github.com/aeroo/aeroolib.git
```
#### 4. Checkout SHA Yang Kompatibel untuk Odoo V8
* **Langkah-1:** Masuk ke dalam modul aeroolib yang sudah di-_cloning_ pada proses sebelumnya.

```bash
cd /opt/aeroo/aeroolib
```
* **Langkah-2:** Checkout SHA Yang Kompatibel

```bash
git checkout b591d23c98990fc358b02b3b78d46290eadb7277
```
#### 5. Installasi Aeroolib
* **Langkah-1:** Masuk ke dalam modul aeroolib yang sudah di-_cloning_ pada proses sebelumnya.

```bash
cd /opt/aeroo/aeroolib
```
* **Langkah-2:** Install aeroolib

```bash
sudo python setup.py install
```