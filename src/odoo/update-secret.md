# Update Secret

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

#### <a name="langkah3">3. Jalankan Copier Update Untuk Mengupdate Secret</a>

Jalankan sintaks berikut:


```bash
copier -a .copier-secret-answer.yml update
```

#### <a name="langkah4">4. Commit Project</a>

Jalankan sintaks berikut:

```bash
git add -u .copier-secret-answer.yml
git commit -m "Update secret"
```