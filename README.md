# Project kelompok 2 - Deploy Laravel using Jenkins

#### Build in jenkins

```yml
cd /var/www/html/pipeline_laravel/ && composer install
php artisan key:generate
php artisan migrate
date >> resources/views/index.blade.php
```
