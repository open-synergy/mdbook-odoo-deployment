# Prasyarat Instalasi
- <h4>Melakukan <i>upgrade</i> dan <i>update</i> apt:</h4>
```bash
sudo apt-get update && sudo apt-get -y upgrade
```
- <h4>Melakukan instalasi docker dan docker.io:</h4>
```bash
sudo apt-get install docker docker.io
```
- <h4>Melakukan instalasi docker-compose. Dokumentasi dapat dilihat <a href="https://docs.docker.com/compose/install/">disini</a>:</h4>
```bash
sudo curl -L "https://github.com/docker/compose/releases/download/1.26.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
```
- <h4>Melakukan cloning docker compose inverseproxy:</h4>
```bash
git clone https://github.com/open-synergy/docker-compose-inverseproxy.git <nama-folder-inverse-proxy>
```
- <h4>Melakukan instalasi doodba copier:</h4>
<b>Python ver.3</b>:

```bash
python3 -m pip install --user pipx
pipx install copier
pipx install invoke
pipx install pre-commit
pipx ensurepath
```
<b>Python ver.2</b>:

```bash
sudo apt-get install python3-pip
python3 -m pipx ensurepath
sudo apt-get install python3-venv
python3 -m pip install --user pipx
```
<b><i>Logout</i> ssh dengan meggunakan Ctrl+D kemudian <i>Re-Login</i></b>
```bash
pipx install copier
pipx install invoke
pipx install pre-commit
pipx ensurepath
```
