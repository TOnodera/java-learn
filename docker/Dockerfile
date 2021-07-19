FROM openjdk:11-slim

RUN apt-get update && apt-get install git -y
WORKDIR /home/www-data/src
RUN usermod -u 1000 -o www-data
RUN chown -R www-data:www-data /home/www-data
WORKDIR /var/www
RUN chown -R www-data:www-data /var/www