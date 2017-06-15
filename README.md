# Vagrant Prestashop
A vagrant box for Prestashop development.

## Dependes
* Vagrant
* VirtualBox/VmWare

## How to install
````
git clone https://github.com/sinermedia/prestashop-vagrant.git prestashop-vagrant
cd prestashop-vagrant
vagrant up
````
Go to http://192.168.22.10/prestashop and follow the installation steps.

## Database connection
**Database name:** prestashop     
**User:** root     
**Password:** prestashop       

## Prestashop Version
You can install any PHP version hosted on ppa:ondrej/php. Edit phpVersion variable on bootstrap.sh.

## Prestashop Version
You can install any Prestashop version. Edit prestaShopFile variable on bootstrap.sh.

## Includes: 
* wget 
* php7.1
* libapache2-mod-php7.1
* php7.1-gd
* mysql-server-5.7
* php7.1-xml
* php7.1-mcrypt
* php7.1-mbstring
* php7.1-mysql
* php7.1-zip
* php7.1-curl
* php7.1-intl
* Prestashop 1.7.1.2

## Based on:
https://github.com/gorkau/vagrant-prestashop
