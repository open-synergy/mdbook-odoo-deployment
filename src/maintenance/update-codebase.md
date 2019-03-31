# Update Codebase

#### 1. Pastikan Anda login sebagai [user odoo](../terminologi.md#user-odoo)
#### <a name="l2">2.</a> Pindah ke direktori codebase yang akan diupdate
#### 3. Fetch codebase

Jalankan sintaks berikut:

```bash
git fetch origin 8.0
```

#### 4. Rebase

```bash
git rebase origin/8.0
```

#### 4. Ulangi [langkah ke-2](#l2) untuk setiap repository yang akan diupdate
