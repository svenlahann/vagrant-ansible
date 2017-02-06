Vagrant Debian LAMP Setup
================================

**vagrant setup for professional modern php development**

Requirements
------------

* [Vagrant](https://www.vagrantup.com/)
* [VirtualBox](https://www.virtualbox.org/)
* [Ansible](http://www.ansible.com/)

Compatibility
-------------

* OSX
* Windows 10
* Linux

Recommendations
---------------
```
vagrant plugin install vagrant-vbguest
vagrant plugin install vagrant-hostmanager
```

Usage
-----
#### Boot-up / stop machine

```
$ vagrant up
$ vagrant halt
```

#### Suspend / resume machine

```
$ vagrant suspend
$ vagrant resume
```

#### Reload machine with provisioning

```
$ vagrant reload --provision
```

#### SSH into machine

```
$ vagrant ssh
```

#### Compatibility and Installation

The system is compatible with OSX, Windows and Linux. It´s tested on OSX Yosemite and El Capitan and Windows 10. I will not go into installation details here, but on Windows 10 you´ll need to install a proper windows shell like [Babun](http://babun.github.io/) or [Cygwin](https://www.cygwin.com/). Please take note, that in most of cases you should use the current stable version of any software installed for the best experience.

System Configuration
--------------------
* OS: Debian Jessie
* RAM: 2GB

SSH Configuration
-----------------
* System IP: 192.168.33.10
* Hostname: app.loc

Shares
------
* /craft
* /htdocs
* /log

PHP Configuration
-----------------
* Depending on developer´s need, the system is able to run either php5 (as debian core package) or php7 (php7.1).

Application Configuration
-------------------------
* Apache´s running on default port 80
* Tomcat´s running on default port 8080
* Redis´s running on default port 6379

Setup
-----
#### Installed system packages

* imagemagick
* curl
* memcached
* mysql
* apache
* php / php7.1
* exim4
* git
* midnight commander
* java 8 openjdk
* ant

#### Installed applications

* apache tomcat 8
* apache solr 4.10.4
* redis

#### Installed php modules

* gd
* imagemagick
* mysql
* xdebug
* curl
* memcached
* mcrypt

#### Global helpers

* composer
* symfony installer
* drush
* drupal console
* laravel
* shopware cli tools
* npm
* grunt
* gulp

Links
-----
* [Ansible](http://www.ansible.com) - "The simplest way to automate." 
* [Vagrant](https://www.vagrantup.com) - "Development environments made easy."
* [Composer](https://getcomposer.org) - "Dependency Manager for PHP"
* [Symfony Installer](https://symfony.com/doc/current/book/installation.html) - "Installing the Symfony Installer"
* [Drush](http://www.drush.org/en/master/) - "Drupal Shell"
* [Drupal Console](https://drupalconsole.com/) - "The new CLI for Drupal"
* [Laravel Installer](https://laravel.com/docs/5.2#installing-laravel) - "Laravel Installer"
* [Shopware CLI Tools](https://github.com/shopwareLabs/sw-cli-tools) - "The shopware CLI tools are your console helpers for all kind of Shopware tasks."
* [npm](https://www.npmjs.com/) - "NPM is the package manager for JavaScript."
* [grunt](http://gruntjs.com/) - "The JavaScript Task Runner"
* [gulp](http://gulpjs.com/) - "The streaming build system"
* [Tomcat](http://tomcat.apache.org/) - "Apache Tomcat"
* [Solr](http://tomcat.apache.org/) - "Apache Solr"
* [Redis](http://redis.io/) - "Redis is an in-memory data structure store"