# Vagrant Prestashop
A vagrant box for Prestashop development.

## Dependences
* [Vagrant](https://www.vagrantup.com/)
* [VirtualBox](https://www.virtualbox.org/) / [VmWare](https://www.vmware.com/es.html)

## PHP Version
You can install any PHP version hosted on ppa:ondrej/php. Edit <code>phpVersion</code> variable on bootstrap.sh.

## Prestashop Version
You can install any Prestashop version. Edit <code>prestaShopFile</code> variable on bootstrap.sh.

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

## Database connection Navicat
On General     
**Host Name/IP Address:** localhost     
**Port:** 3306 (see if the VM fixed port collision on start)     
**User Name:** root        
**Password:** wordpress                
        
SSH        
**Host Name/IP Address:** 192.168.22.10 (see vagrantFile if you changed this IP)        
**Port:** 22        
**User Name:** ubuntu        
**Authentication Method:** Password        
**Password:** See https://askubuntu.com/a/875659/451151 to get VM password (~/.vagrant.d/boxes/...)        
        
        
````
vagrant ssh
mysql -h localhost -u root -pprestashop prestashop
````

## Includes: 
* wget 
* php
* libapache2-mod-php
* php-gd
* mysql-server-5.7
* php-xml
* php-mcrypt
* php-mbstring
* php-mysql
* php-zip
* php-curl
* php-intl
* Prestashop

## Based on:
https://github.com/gorkau/vagrant-prestashop
