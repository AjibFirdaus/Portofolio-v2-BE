# Portofolio-v2-BE

## Instalasi

Ikuti langkah-langkah berikut untuk menginstal dan menjalankan proyek ini secara lokal:

1. **Clone repositori**
    ```bash
    https://github.com/AjibFirdaus/Portofolio-v2-BE.git
    cd backend
    ```

2. **Instal dependensi untuk backend**
    ```bash
    npm install
    ```

3. **Konfigurasi lingkungan backend**
    - Buat file `.env` di direktori `backend` dan tambahkan konfigurasi berikut:
        ```env
        DATABASE_URL=mysql://user:password@localhost:3306/dbname
        JWT_SECRET=buat_jwt_key_sendiri
        AES_KEY=buat_aes_key_sendiri
        ```

4. **Migrasi Database**
    ```bash
    npx prisma migrate dev
    npx prisma generate
    sebelum run seed perlu ubah terlebih dahulu di seed.js ubah bagian photo (path photo), username, password (hashed password) setelah itu
    npm run seed
    ```


4. **Jalankan server backend**
    ```bash
    nodemon .
    ```

5. **Buka aplikasi frontend**