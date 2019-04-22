# Installasi Dependensi

#### 1. Buka terminal
#### 2. Pastikan Anda login sebagai [user default](../../terminologi.md#user-default)
Abaikan apabila Anda sudah login sebagai user OS yang akan menjalankan Odoo
#### 3. Install wkhtmltopdf
Jalankan sintaks berikut di terminal:

```bash
sudo wget https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.4/wkhtmltox-0.12.4_linux-generic-amd64.tar.xz
tar -xvf wkhtmltox-0.12.4_linux-generic-amd64.tar.xz
sudo cp ./wkhtmltox/bin/wkhtmltoimage /usr/bin/
sudo cp ./wkhtmltox/bin/wkhtmltopdf /usr/bin/
```
#### 4. Install git
Jalankan sintaks berikut di terminal:

```bash
sudo apt-get install git
```
#### 5. Install python-setuptools
Jalankan sintaks berikut di terminal:

```bash
sudo apt-get install python-setuptools
```
#### 6. Install python-genshi
Jalankan sintaks berikut di terminal:

```bash
sudo apt-get install python-genshi
```
#### 7. Install python-cairo
Jalankan sintaks berikut di terminal:

```bash
sudo apt-get install python-cairo
```
#### 8. Install python-lxml
Jalankan sintaks berikut di terminal:

```bash
sudo apt-get install python-lxml
```
#### 8. Install libreoffice-script-provider-python
Jalankan sintaks berikut di terminal:

```bash
sudo apt-get install libreoffice-script-provider-python
```
#### 9. Install python-cups
Jalankan sintaks berikut di terminal:

```bash
sudo apt-get install python-cups
```
#### 10. Install libreoffice-base
Jalankan sintaks berikut di terminal:

```bash
sudo apt-get install libreoffice-base
```
