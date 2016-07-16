# Supported tags and respective Dockerfile links

#### Apache

* 7.0-apache-oraclelinux [(7.0/apache/oraclelinux/Dockerfile)](https://github.com/krike06/docker-php-containers/blob/master/7.0/apache/oraclelinux/Dockerfile)
* 5.5-apache-oraclelinux [(5.5/apache/oraclelinux/Dockerfile)](https://github.com/krike06/docker-php-containers/blob/master/5.5/apache/oraclelinux/Dockerfile)

# How to use this image

#### Apache

    php:
      image: krike06/php:7.0-apache-oraclelinux
      volumes:
        - .:/var/www/project/
      environment:
        - ENVIRONMENT=dev
        - DEBUG=1
        - BASE_PATH=/var/www/project/
      links:
        - mongodb
      ports:
        - 80
