# Build Aplikasi

#### <a name="langkah1">1. Pastikan working directory berada pada home directory [\<\<USER OS\>\>](/placeholder.md#user-os)</a>

Jalankan sintaks berikut:

```bash
cd ~
````

#### <a name="langkah2">2. Masuk ke [\<\<PROJECT DIRECTORY\>\>](/placeholder.md#project-directory)</a>

Jalankan sintaks berikut:

```bash
cd <<PROJECT DIRECTORY>>
````

#### <a name="langkah3">3. Build Aplikasi</a>

Jalankan sintaks berikut:

```bash
sudo docker-compose -f prod.yaml build --no-cache
````