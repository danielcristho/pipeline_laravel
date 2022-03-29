# Project kelompok 2 - Deploy Laravel using Jenkins
#### How to build
```yml
$ cd /var/www/html/
$ git clone https://github.com/danielcristho/pipeline_laravel.git
```

#### Run in jenkins dashboard (ip_addr:8080)

```yml
cd /var/www/html/pipeline_laravel/ && composer install
php artisan key:generate
php artisan migrate
date >> resources/views/index.blade.php
```
