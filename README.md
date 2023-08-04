# Simple Appliction with REST API in Laravel 10
A simple application using REST API for handling events with the owner (user) and attendees. An example of using the REST API.
## 

Run docker containers
```` bash
docker-compose up -d
````

Go into php container as user (1000) for artisan command, or composer
```` bash
docker exec -it -u 1000 php /bin/bash
````

## Install Laravel and move to main folder
```` bash
composer install
````
```` bash
php artisan migrate
````
```` bash
php artisan db:seed 
````

## Fix storage permission
```` bash
chmod 777 -R storage
````

## Database local connection
    MYSQL_HOST = mysql <docker mysql container name>
    MYSQL_DATABASE = database
    MYSQL_USER = admin
    MYSQL_PASSWORD = password

## Links
http://localhost:61000 - website

http://localhost:8080 - Adminer (database management in browser)
