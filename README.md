# Vagrant Prestashop
A vagrant box for Prestashop development.

## Dependences
* [Vagrant](https://www.vagrantup.com/)
* [VirtualBox](https://www.virtualbox.org/) / [VmWare](https://www.vmware.com/es.html)

## How to install
````
git clone https://github.com/sinermedia/prestashop-vagrant.git prestashop-vagrant
cd prestashop-vagrant
vagrant up
````
Go to http://192.168.22.10/prestashop and follow the installation steps.

**Create more than one virtual Machine**        
If you want create more than one Virtual Machine, you must change the <code>server_ip</code> and <code>hostname</code> values on the VagrantFile of your new installation with differents values than another VM created in your system. If you don't change this values, you will overwrite your created VM. 

## Database connection
**Database name:** prestashop     
**User:** root     
**Password:** prestashop       

## Prestashop Version
You can install any PHP version hosted on ppa:ondrej/php. Edit <code>phpVersion</code> variable on bootstrap.sh.

## Prestashop Version
You can install any Prestashop version. Edit <code>prestaShopFile</code> variable on bootstrap.sh.

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
