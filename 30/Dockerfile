FROM nextcloud:30.0.6-apache

LABEL org.opencontainers.image.description "Official Nextcloud base image plus some useful Linux packages"

RUN apt-get update
RUN apt install -y bzip2 libbz2-dev && docker-php-ext-install bz2
RUN apt install -y libgmp3-dev && docker-php-ext-install gmp
RUN apt install -y procps smbclient libsmbclient-dev && pecl install smbclient && docker-php-ext-enable smbclient
RUN apt install -y libmagickcore-6.q16-6-extra
