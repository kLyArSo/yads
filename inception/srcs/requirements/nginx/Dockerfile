FROM debian:buster
RUN apt-get update
RUN apt-get install -y nginx openssl
RUN mkdir /etc/nginx/ssl
RUN openssl req -newkey rsa:2048 -x509 -sha256 -days 365 -nodes -out /etc/nginx/ssl/ylhouari.cert -keyout /etc/nginx/ssl/ylhouari.key -subj "/C=MA/ST=Kech/L=Benguerir/O=UM6P/OU=1337/CN=ylhouari/"
COPY ./nginx.conf /etc/nginx/conf.d
ENTRYPOINT ["nginx", "-g", "daemon off;"]
