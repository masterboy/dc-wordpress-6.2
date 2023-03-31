To make a fresh install of WordPress 6.2 with Nginx and MariaDB (MySQL-compliant) database, follow these steps:-

```
git clone git@github.com:masterboy/dc-wordpress-6.2.git
```

Then copy then `.env.example` file to `.env`

```
cp .env.example .env
```

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