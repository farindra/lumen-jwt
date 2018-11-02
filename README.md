Farindra Project ~ Lumen JWT

Installasi :
1. Clone kemudian masuk ke root project
2. composer install
3. buat file .env baru dari contoh ``` $ cp .env.exampe .env``` edit property database dan app key
5. Migrasi Database ```$ php artisan migrate:fresh --seed```
6. Jalankan lumen ```$ php -S localhost:8000 -t public```

Request Token:
Method : POST
URL : http://localhost:8000/auth/login
BODY Payload : ```{ "email" : "useremail@email.com" , "password" : "secret" }```

Test Middleware URL: http://localhost:8000/users