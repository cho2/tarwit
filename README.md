# Tarwit
Daftar dan Twit _booth_ openSUSE-ID di Indonesian Linux Connference 2022

---
## Kebutuhan
- Subdomain
- apache2
- mysql-server
- php php-curl php-xml php-mbstring
- composer
- Twitter apps api

## Basis data
- Buat basis data
- Impor `visitor.sql`

* Sunting `databaseFiles/insertDetails.php`
    ```
    $consumerkey = "HERE";
    $consumersecret = "HERE";  
    $accesstoken = "HERE";  
    $accesstokensecret = "HERE";  
    $photoAddr =  
    ```
    Sesuaikan `$photoAddr` dengan domain
* Sunting `databaseFiles/database_connections.php`
* Sunting `js/angular-script.js`
* Sunting dependensi
    ```
    $ cd databaseFiles/twitteroauth 
    $ composer install
    ```

## Todo
* Dockerizing
