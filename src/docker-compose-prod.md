# Docker Compose Prod

Pada proses [Doodba Template](./doodba-template.md) sebelumnya, maka akan terbuat <b>prod.yaml</b> yang kemudian akan kita build.

- <h4>Melakukan build pada <b>prod.yaml</b></h4>
```bash
cd <nama-project>
sudo docker-compose -f prod.yaml build --no-cache
```
- <h4>Menjalankan docker-compose prod.yaml menggunakan parameter <b>-d</b> agar dijalankan di <i>background</i>:</h4>
```bash
sudo docker-compose -f prod.yaml up -d
```
- <h4>Pastikan docker-compose prod sudah running:</h4>
```bash
sudo docker-compose -f prod.yaml ps
```
