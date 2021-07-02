# BASIC WIP CRUD - Laravel 8 Docker/ Set Up
This is a simple laravel 8 CRUD app.

## How to install and run on your local system
1. git clone https://github.com/Glendoni/CRUDORDERBACKEND.git
2. Terminal cd [to root folder]/
3. Terminal run: docker-compose - build to pull down all dependencies  
4. Termiinal run: docker-compose up -d
5. Terminal run: docker exec -it  qdoctor_php-fpm_1  bash
6. In Docker Shell Run: cd source
7. In Docker Shell Run: composer update
8. If .env does not exsit in open docker shell: Run: cp .env.example .env
9. In Source folder open .env file and update the DB creds that can be found in the docker-compose.yml file.
   
EXAMPLE<br>
   DB_CONNECTION=mysql<br>
   DB_HOST=192.168.32.1<br>
   DB_PORT=10002<br>
   DB_DATABASE=qdoctor<br>
   DB_USERNAME=qdoctor<br>
   DB_PASSWORD=secret
   
10. Return back to the docker shell Run: php artisan key:generate
11. In Docker Shell Run: php artisan migrate
12. Visit page: http://localhost:10000. You should see

OK Lets move to https://github.com/Glendoni/basic_angular11_crud_client


## POSTMAN
Collection file is in root: HSO.postman_collection.json

