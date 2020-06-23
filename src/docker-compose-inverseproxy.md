# Docker Compose Inverseproxy

Proses dibawah ini adalah lanjutan setelah [Melakukan cloning docker compose inverseproxy](./prasayarat-instalasi.md#15).

- <h4>Mengubah isian <b>ACME.Email</b> dengan alamat email yang aktif pada inverseproxy.yaml:</h4>
```bash
cd <path-to-inverseproxy-folder>
pico inverseproxy.yaml
```
- <h4>Menjalankan docker-compose inverseproxy menggunakan parameter <b>-d</b> agar dijalankan di <i>background</i>:</h4>
```bash
sudo docker-compose -f inverseproxy.yaml up -d
```
- <h4>Pastikan docker-compose inverseproxy sudah running:</h4>
```bash
sudo docker-compose -f inverseproxy.yaml ps
```
