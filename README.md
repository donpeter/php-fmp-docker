# Docker PHP-FPM  
This image is designed to be used with a web server like Nginx to serve your PHP app, it include some important php modules like mysqli and PDO which is not available in the official image.
You can use docker networking to create a network and attach all the containers to that network.

### How to use?
```sh
$ docker pull patunalu/php-fpm
```

#### docker-compose
```docker-compose
# docker-compose.yml

php:
    image: patunalu/php-fpm
    restart: always
    volumes:
      - ./application:/application
    expose:
      - 9000
```