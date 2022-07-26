FROM debian:buster
RUN apt-get update
RUN apt-get install -y wget
RUN wget https://wordpress.org/latest.tar.gz
RUN tar -xzvf latest.tar.gz
RUN mkdir -p /var/www/html
RUN mv wordpress/* /var/www/html
#COPY wp-config.php /var/www/html/ 
