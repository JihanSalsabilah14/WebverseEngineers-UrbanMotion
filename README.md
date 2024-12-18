# Urban Motion

**Urban Motion** adalah aplikasi penyewaan kendaraan yang memungkinkan pengguna untuk menyewa kendaraan dengan mudah kapan saja, di mana saja. Repositori ini berisi kode sumber untuk **Frontend** dan **Backend** aplikasi.

## Prasyarat
Sebelum memulai, pastikan Anda telah menginstal:  
- [Node.js](https://nodejs.org/)  
- Git  

## Cara Menjalankan Aplikasi

### 1. Clone Repositori
Clone repositori ini ke komputer lokal Anda menggunakan git bash:
```bash
    git clone <REPOSITORY_URL> 
    cd <REPOSITORY_NAME>
```

### 2. Setup Backend 

1. Buatlah database di MySQL dengan nama "car_rental"

2. Masuk ke direktori backend di terminal:
   ```bash
    cd backend
   ```

3. Instal Dependensi
    Jalankan perintah berikut untuk menginstal semua paket yang diperlukan:
   ```bash
    npm install
   ```
4. Buka File .env.example lalu rename menjadi .env
5. ubahlah code yang terdapat pada .env menjadi berikut
  ```bash
    DB_DBNAME=car_rental
    DB_USERNAME=root
    DB_PASSWORD=""
    DB_HOSTNAME=localhost
    DB_PORT=3306
    APP_PORT = 5000
    NODE_ENV = 'development'
    JWT_SECRET_KEY= "secret_key"
    MIDTRANS_SERVER_KEY = "SB-Mid-server-BnJiF_UbSvvwjIW-r2O9TN6G"
    MIDTRANS_CLIENT_KEY = "SB-Mid-client-qobw5pB_yws0iwwJ"
    MIDTRANS_CALLBACK_URL = "http://localhost:5173"
    OAUTH_CLIENT_ID = "192573977992-jlhe722hi206jkaqluais2qrng1lk461.apps.googleusercontent.com"
    OAUTH_CLIENT_SECRET = "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"
   ```
6. Jalankan Migrasi dan Seed Database

    Pastikan database Anda berjalan, lalu eksekusi perintah berikut:
    i. Jalankan Migrasi:
   ```bash
   npm run migrate-up
   ```

    ii. Seed Database:
     ```bash
        npm run seed-up
   ```
        
8. Jalankan Aplikasi
    Setelah pengaturan selesai, Anda dapat memulai aplikasi dengan menjalankan:
   ```bash
    npm run dev
   ```

### 3. Setup Frontend 
1. Masuk ke direktori frontend
    ```bash
    cd frontend
    ```

2. Instal Dependensi
    Jalankan perintah berikut untuk menginstal semua paket yang diperlukan:
   ```bash
    npm install
   ```
        
3. Jalankan Aplikasi
    Setelah pengaturan selesai, Anda dapat memulai aplikasi dengan menjalankan:
   ```bash
    npm run dev
   ```


### 4. Akses Aplikasi
    Frontend akan tersedia di: http://localhost:5173  
    Backend akan tersedia di: http://localhost:5000 (atau sesuai konfigurasi Anda)

