# Docker_Wordpress_Nginx_MariaDB

docker-compose version: docker-compose version 1.21.2, build a133471
docker version: Docker version 18.09.4, build d14af54266
docker-compose service version: 3.6

modify the .env to your liking
# wordpress
WORDPRESS_DB_NAME=wordpress_uk
WORDPRESS_TABLE_PREFIX=wp_
WORDPRESS_DB_HOST=db
WORDPRESS_DB_USER=root
WORDPRESS_DB_PASSWORD=Kennedy

# mariadb
MYSQL_ROOT_PASSWORD=Kennedy
MYSQL_USER=root
MYSQL_PASSWORD=Kennedy
MYSQL_DATABASE=wordpress_uk

# volumes on host
#NGINX_CONF_DIR=./nginx
#NGINX_LOG_DIR=./logs/nginx

save and finish

run:

docker-compose up -d

run part:

docker-compose up -d db
docker-compose up -d wp nginx

running site

web http://xxxx.xxxx.xxxx.xxxx and wala!

Stop and remove containers

Run the script stop_remove_container.sh
