# Command Line Tool

List command line tool yang akan bermanfaat.

- <h4>Stop Service docker-compose prod.yaml</h4>
```bash
sudo docker-compose -f prod.yaml down
```
- <h4>Menghapus semua service beserta database docker-compose prod.yaml</h4>
```bash
sudo docker-compose -f prod.yaml down -v
```
- <h4>Mengupdate copier template. Biasanya digunakan apabila ada perubahan pada prod.yaml</h4>
```bash
cd <nama-project>
copier update
```
- <h4>Melihat logs Odoo</h4>
```bash
sudo docker-compose -f prod.yaml logs --tail=100 odoo
```
- <h4>Stop service Odoo</h4>
```bash
sudo docker-compose -f prod.yaml stop odoo
```
- <h4>Start service Odoo</h4>
```bash
sudo docker-compose -f prod.yaml start odoo
```
