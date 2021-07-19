FROM openjdk:11-slim

RUN apt-get update && apt-get install git -y \
    && git config --global user.name "takeshi" \
    && git config --global user.email t.onodera.1.2.1.5@gmail.com
    
WORKDIR /home/www-data/src
RUN usermod -u 1000 -o www-data
RUN chown -R www-data:www-data /home/www-data
WORKDIR /var/www
RUN chown -R www-data:www-data /var/www