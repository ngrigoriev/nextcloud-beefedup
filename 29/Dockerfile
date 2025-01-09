FROM nextcloud:29.0.10-apache

RUN apt-get update
RUN apt install -y bzip2 libbz2-dev && docker-php-ext-install bz2
RUN apt install -y libgmp3-dev && docker-php-ext-install gmp
RUN apt install -y procps smbclient libsmbclient-dev && pecl install smbclient && docker-php-ext-enable smbclient
RUN apt install -y libmagickcore-6.q16-6-extra
