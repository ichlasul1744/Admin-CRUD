# Aplikasi CRUD Admin dengan Laravel

Aplikasi ini dikembangkan menggunakan framework Laravel dan mengimplementasikan autentikasi multi-user dengan Breeze. Aplikasi ini memungkinkan untuk pendaftaran pengguna dan admin, dimana hanya admin yang dapat melakukan Create, Read, Update, dan Delete (CRUD) pada entitas produk.

## Fitur

- **Autentikasi Multi-User**: Mendukung pendaftaran dan autentikasi untuk dua jenis pengguna: Admin dan User.
- **CRUD Produk**: Admin dapat menambah, melihat, mengubah, dan menghapus produk.
- **Dashboard Admin**: Sebuah antarmuka untuk admin untuk mengelola produk.
- **Pendaftaran Pengguna**: Pengguna dapat mendaftar dan masuk ke dalam sistem.

## Persiapan

Sebelum Anda memulai, pastikan Anda telah menginstal PHP, Composer, dan Laravel pada sistem Anda. Aplikasi ini dikembangkan menggunakan Laravel versi 11.

## Instalasi

1. **Klon Repositori**

    ```bash
    git clone https://your-repository-url.git
    cd your-project-directory
    ```

2. **Instal Dependencies**

    ```bash
    composer install
    ```

3. **Konfigurasi Environment**

    Salin file `.env.example` ke file baru bernama `.env` dan sesuaikan konfigurasinya dengan sistem Anda.

    ```bash
    cp .env.example .env
    ```

4. **Generate Application Key**

    ```bash
    php artisan key:generate
    ```

5. **Migrasi Database**

    Pastikan Anda telah membuat database dan mengonfigurasinya di file `.env`, kemudian jalankan migrasi.

    ```bash
    php artisan migrate
    ```

6. **Seeding Database (Opsional)**

    Jika Anda ingin mengisi database dengan data awal:

    ```bash
    php artisan db:seed
    ```

7. **Jalankan Server Pengembangan**

    ```bash
    php artisan serve
    ```

    Akses aplikasi di `http://localhost:8000`.

## Penggunaan

- **Daftar sebagai Admin/User**: Buka `http://localhost:8000/register` untuk membuat akun baru.
- **Login**: Buka `http://localhost:8000/login` untuk masuk ke dalam sistem.
- **Dashboard Admin**: Setelah login sebagai admin, Anda dapat mengakses dashboard admin untuk mengelola produk.
- **Output**: output dari aplikasi berada di file output.pdf.

