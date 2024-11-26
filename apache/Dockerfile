FROM debian:11

RUN apt-get update && apt-get install -y apache2 php libapache2-mod-php net-tools

RUN apt clean && rm -rf /var/lib/apt/lists/*

RUN a2dissite 000-default.conf

EXPOSE 80

CMD [ "apachectl" , "-D" , "FOREGROUND" ]