# Vagrant Development PHP
This my personal development environment

## License
GPL-3.0

## Content
* Oracle Instant Client 11.2
* Apache 2.2.29
* PHP 5.6.18 Compile like this:

```bash
./configure \
--prefix=/usr/local/php/php_5.6.14 \
--with-apxs2=/usr/local/apache2/bin/apxs \
--disable-all \
--enable-session \
--enable-libxml \
--enable-dom \
--enable-filter \
--enable-pdo \
--enable-phar \
--enable-simplexml \
--enable-soap \
--enable-sockets \
--enable-bcmath \
--enable-ftp \
--enable-mbstring \
--enable-tokenizer \
--enable-xml \
--enable-mysqlnd \
--with-sqlite3 \
--with-libxml-dir=/usr/bin \
--with-openssl \
--with-openssl-dir=/usr/bin \
--with-zlib \
--with-curl \
--with-gettext \
--with-mysql=mysqlnd \
--with-mysqli=mysqlnd \
--with-oci8=instantclient \
--with-readline \
--with-pdo-mysql=mysqlnd \
--with-pdo-oci \
--with-pdo-sqlite \
--with-snmp \
--with-openssl-dir \
--with-pear \
--enable-mysqlnd-compression-support \
--enable-inline-optimization \
--with-zend-vm=GOTO \
--enable-static \
--enable-re2c-cgoto \
--enable-cli \
--enable-json \
--with-iconv \
--with-mcrypt \
--with-mhash \
--enable-ctype \
--enable-xmlwriter \
--enable-xmlreader \
--enable-posix \
--enable-ipv6 \
--enable-calendar \
--with-xsl \
--with-gd \
--with-freetype-dir \
--with-jpeg-dir \
--with-png-dir
```
* Xdebug
* PHP ZIP Extension
* Composer
* Memcached
* PHP Memcached Extension
* LDAP Extension
* OCI8 Extension
* MySQL Server

## MYSQL Server
* user = root
* password = vagrant

## Usage
* Clone this repository
```bash
$> git clone git@github.com:irgalieri/vagrant_dev.git
```
* Enter in the repository folder
```bash
$> cd vagrant_dev
```
* Run Vagrant up
```bash
$> vagrant up
```
* Test enter to http://127.0.0.1:8888/index.php
* To login into VM run:
```bash
$> vagrant ssh
```
* clone your favourite repository into public and enjoy the ride
