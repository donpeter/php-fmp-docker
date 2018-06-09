# Docker PHP-FMP  
This image is designed to be used with a web server like Nginx to serve your PHP app, it include some important php modules like mysqli and PDO which is not available in the official image.
You can use docker networking to create a network and attach all the containers to that network.

```sh
$ docker pull patunalu/php-fmp
```