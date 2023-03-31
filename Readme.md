To make a fresh installation of WordPress 6.2 with PHP-FPM, Nginx and MariaDB (MySQL-compliant) database, follow these steps:-

```
git clone git@github.com:masterboy/dc-wordpress-6.2.git
```

Then copy then `.env.example` file to `.env`

```
cp .env.example .env
```

By default, the WordPress installation will be available on `http://localhost:8001` and the database will be available on `http://localhost:3001` once you perform docker compose up. You can modify the ports in the `.env` file.

You may want to check the docker-compose.yml file and make some personal modifications.

Finally,

```
docker compose up -d
```
Or, for older versions:-

```
docker-compose up -d
```

You have your custom WordPress installation ready on `./src` directory which is bind mounted to docker containers.
