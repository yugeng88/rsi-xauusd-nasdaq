# Tutorial membuat repository dan mengaktifkan GitHub Pages

## A. Buat repository baru
1. Masuk ke https://github.com dan login.
2. Tekan tombol **+** di kanan atas, lalu pilih **New repository**.
3. Isi nama, misalnya `rsi-xauusd-nasdaq`.
4. Pilih **Public** (atau Private jika sesuai paket/akses Pages Anda).
5. Centang **Add a README file** bila ingin, lalu tekan **Create repository**.

## B. Upload file aplikasi
1. Buka repository yang baru dibuat.
2. Tekan **Add file** → **Upload files**.
3. Ekstrak ZIP aplikasi di HP/komputer terlebih dahulu.
4. Pilih dan upload file `index.html`, `README.md`, serta folder/file panduan yang disediakan. Pastikan `index.html` berada langsung di root repository, bukan di dalam folder bertingkat.
5. Isi pesan commit, misalnya `Add RSI dashboard`, lalu tekan **Commit changes**.

## C. Aktifkan website GitHub Pages
1. Di repository, buka **Settings**.
2. Pilih **Pages** pada menu sebelah kiri.
3. Pada **Build and deployment**, pilih **Deploy from a branch**.
4. Branch pilih **main**, folder pilih **/(root)**.
5. Tekan **Save** dan tunggu proses deployment selesai.
6. Buka alamat yang muncul, biasanya `https://USERNAME.github.io/NAMA-REPOSITORY/`.

## D. Jika menggunakan iPhone
- ZIP dapat diekstrak dari aplikasi **Files** dengan mengetuk file ZIP.
- Di GitHub melalui Safari, buka repository → **Add file** → **Upload files**. Jika pemilih file sulit digunakan, aktifkan **Request Desktop Website** di Safari atau lakukan dari komputer.
- Untuk menambahkan file satu per satu: **Add file** → **Create new file**, ketik nama `index.html`, tempel isi file, lalu **Commit changes**. Cara upload ZIP yang sudah diekstrak biasanya lebih praktis.

## E. Memperbarui aplikasi
Edit `index.html` melalui repository → buka file → ikon pensil/Edit → ubah kode → **Commit changes**. GitHub Pages akan menerbitkan pembaruan otomatis setelah beberapa saat.
