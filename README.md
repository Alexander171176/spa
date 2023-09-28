### For local dev

1) Create project <br>
   `composer create-project laravel/laravel spa`
   <br>
   or `git clone`
2) Key generate <br>
   `php artisan key:generate --ansi`
3) Make directory for docker: <br>
   `mkdir ./storage/docker`
4) Copy .env.example <br>
   `cp .env.example .env`
5) Add host user to .env <br>
   `echo UID=$(id -u) >> .env` <br>
   `echo GID=$(id -g) >> .env`
6) Run services docker <br>
   `docker-compose up -d --build`
