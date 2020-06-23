# Doodba Template

- <h4></i>Copy</i> template doodba milik Tecnativa menggunakan copier</h4>
```bash
copier copy gh:Tecnativa/doodba-copier-template <nama-project>
```
- <h4>Isi Pertanyaan-pertanyaan yang diberikan:</h4>

    *   <b>project_author?</b> (Format: &lt;<i>str</i>&gt;)
        > Nama pembuat project

    *   <b>project_name?</b> (Format: &lt;<i>str</i>&gt;)
        > Nama project

    *   <b>project_license?</b> (Format: &lt;<i>Multiple Choice</i>&gt;)
        > Pilih: [4] GNU Affero General Public License (AGPL) 3.0 or later

    *   <b>gitlab_url?</b> (Format: &lt;<i>str</i>&gt;)
        > Url Gitlab.
        >
        > Pilih: None(dengan menekan Enter)

    *   <b>domain_prod?</b> (Format: &lt;<i>str</i>&gt;)
        > Domain yang digunakan.
        >
        > Contoh: www.latihan1.simetri-sinergi.id

    *   <b>domain_prod_alternatives?</b> (Format: &lt;<i>yaml</i>&gt;)
        > Domain yang digunakan. Pengisian menggunakan bracket []
        >
        > Contoh: [latihan1.simetri-sinergi.id]

    *   <b>domain_test?</b> (Format: &lt;<i>str</i>&gt;)
        > Nama test domain.
        >
        > Pilih: None(dengan menekan Enter)

    *   <b>paths_without_crawlers?</b> (Format: &lt;<i>yaml</i>&gt;)
        > Nama test domain.
        >
        > Pilih: None(dengan menekan Enter)

    *   <b>cidr_whitelist?</b> (Format: &lt;<i>yaml</i>&gt;)
        > Nama test domain.
        >
        > Pilih: None(dengan menekan Enter)

    *   <b>odoo_version?</b> (Format: &lt;<i>Multiple Choice</i>&gt;)
        > Versi odoo yang akan digunakan

    *   <b>odoo_initial_lang?</b> (Format: &lt;<i>str</i>&gt;)
        > Bahasa yang akan digunakan.

    *   <b>odoo_oci_image?</b> (Format: &lt;<i>str</i>&gt;)
        > Image odoo opsional.

    *   <b>odoo_listdb?</b> (Format: &lt;<i>boolean</i>&gt;)
        > [y] - Yes. List Database akan dipublikasikan
        >
        > [n] - No. List Database tidak akan dipublikasikan
        >
        > Pilih: n


    *   <b>odoo_admin_password?</b> (Format: &lt;<i>str</i>&gt;)
        > Password administrator Odoo

    *   <b>odoo_dbfilter?</b> (Format: &lt;<i>str</i>&gt;)
        > Isi dengan <b>%h</b>

    *   <b>odoo_proxy?</b> (Format: &lt;<i>yaml</i>&gt;)
        > Pilih: [2] Traefik

    *   <b>postgres_version?</b> (Format: &lt;<i>yaml</i>&gt;)
        > Versi postgreSQL yang akan digunakan

    *   <b>postgres_username?</b> (Format: &lt;<i>str</i>&gt;)
        > User Postgre yang akan digunakan
        >
        > Pilih: Default(dengan menekan Enter)

    *   <b>postgres_dbname?</b> (Format: &lt;<i>str</i>&gt;)
        > Nama Database
        >
        > Isian: Nama database biasanya disamakan dengan nama domain tanpa menggunakan dot(.)
        >
        > Contoh: latihan1-simetri-sinergi-id

    *   <b>postgres_password?</b> (Format: &lt;<i>str</i>&gt;)
        > Password database PostgreSQL

    *   <b>smtp_default_from?</b> (Format: &lt;<i>str</i>&gt;)
        > SMTP untuk mengirim email.
        >
        > Pilih: None(dengan menekan Enter)

    *   <b>smtp_relay_host?</b> (Format: &lt;<i>str</i>&gt;)
        > SMTP relay host.
        >
        > Pilih: None(dengan menekan Enter)

    *   <b>smtp_relay_port?</b> (Format: &lt;<i>int</i>&gt;)
        > SMTP relay port.
        >
        > Pilih: 587(dengan menekan Enter)

    *   <b>smtp_relay_user?</b> (Format: &lt;<i>str</i>&gt;)
        > SMTP relay user.
        >
        > Pilih: None(dengan menekan Enter)

    *   <b>smtp_relay_password?</b> (Format: &lt;<i>str</i>&gt;)
        > SMTP relay password.
        >
        > Pilih: None(dengan menekan Enter)

    *   <b>smtp_canonical_default?</b> (Format: &lt;<i>str</i>&gt;)
        > SMTP canonical default.
        >
        > Pilih: None(dengan menekan Enter)

    *   <b>smtp_canonical_domains?</b> (Format: &lt;<i>yaml</i>&gt;)
        > SMTP canonical domains.
        >
        > Pilih: None(dengan menekan Enter)

    *   <b>backup_dst?</b> (Format: &lt;<i>str</i>&gt;)
        > Tempat dimana backup akan disimpan apabila ingin menggunakan backup.
        >
        > Pilih: None(dengan menekan Enter)

    *   <b>backup_email_from?</b> (Format: &lt;<i>str</i>&gt;)
        > Alamat email yang akan mengirimkan report backup.
        >
        > Pilih: None(dengan menekan Enter)

    *   <b>backup_email_to?</b> (Format: &lt;<i>str</i>&gt;)
        > Alamat email yang akan dikirimkan report backup.
        >
        > Pilih: None(dengan menekan Enter)

    *   <b>backup_deletion?</b> (Format: &lt;<i>boolean</i>&gt;)
        > Otomatisasi penghapusan backup.
        >
        > Pilih: None(dengan menekan Enter)

    *   <b>backup_tz?</b> (Format: &lt;<i>str</i>&gt;)
        > Backup TimeZone.
        >
        > Pilih: UTC(dengan menekan Enter)

    *   <b>backup_aws_access_key_id?</b> (Format: &lt;<i>str</i>&gt;)
        > Backup Aws Access Key.
        >
        > Pilih: None(dengan menekan Enter)

    *   <b>backup_aws_secret_access_key?</b> (Format: &lt;<i>str</i>&gt;)
        > Backup Aws Secret Access.
        >
        > Pilih: None(dengan menekan Enter)

    *   <b>backup_passphrase?</b> (Format: &lt;<i>str</i>&gt;)
        > Backup Password untuk sekuriti.
        >
        > Pilih: Default(dengan menekan Enter)
