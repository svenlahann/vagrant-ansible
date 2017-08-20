Vagrant LEMP Setup for modern web development
=============================================

**vagrant setup for professional modern web development**
This vagrant box is preconfigured to use either with Virtualbox or Parallels provider.

Requirements
------------
* [Vagrant](https://www.vagrantup.com/)
* [VirtualBox](https://www.virtualbox.org/)
* [Ansible](http://www.ansible.com/)
* [rsync](https://en.wikipedia.org/wiki/Rsync)

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

The system is compatible with OSX, Windows and Linux. It´s tested on OSX Yosemite and El Capitan and Windows 10. I will not go into installation details here, but on Windows 10 you´ll need to install a proper shell like [Babun](http://babun.github.io/) or [Cygwin](https://www.cygwin.com/). Please take note, that in most of cases you should use current stable versions of the software required for best experience.

System Configuration
--------------------
* OS: Ubuntu 16.04 LTS (Xenial Xerus)
* RAM: 2GB

SSH Configuration
-----------------
* System IP: 11.11.11.111
* Hostname: app.dev

Shares
------
* /craft
* /htdocs
* /log

PHP Configuration
-----------------
* The system uses the os packaged php version - in case of ubuntu 16.04 it´s php7.0.

Application Configuration
-------------------------
* Nginx is running on default port 80
* MongoDB is running on default port 27017
* Redis is running on default port 6379
* Elasticsearch is running on default port 9200
* Beanstalkd is running on default port 11300

Setup
-----
#### Installed system packages

* imagemagick
* curl
* memcached
* mysql
* sqlite3
* apache
* php / php7.0
* exim4
* git
* midnight commander
* java 8 openjdk
* ruby 2.4
* python
* ant
* ack-grep
* vim

#### Installed applications

* mongodb
* redis
* beanstalkd
* elasticsearch
* apache solr
* docker
* deployer

#### Installed php modules

* gd
* imagemagick
* mysql
* xdebug
* curl
* memcached
* sqlite3
* mcrypt
* xml
* mbstring
* zip
* ldap
* mongodb
* ioncube

#### Global helpers

* composer
* symfony installer
* drush
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
* [Laravel Installer](https://laravel.com/docs/5.4#installing-laravel) - "Laravel Installer"
* [Shopware CLI Tools](https://github.com/shopwareLabs/sw-cli-tools) - "The shopware CLI tools are your console helpers for all kind of Shopware tasks."
* [npm](https://www.npmjs.com/) - "NPM is the package manager for JavaScript."
* [grunt](http://gruntjs.com/) - "The JavaScript Task Runner"
* [gulp](http://gulpjs.com/) - "The streaming build system"
* [Tomcat](http://tomcat.apache.org/) - "Apache Tomcat"
* [Solr](http://tomcat.apache.org/) - "Apache Solr"
* [Redis](http://redis.io/) - "Redis is an in-memory data structure store"
* [Elasticsearch](https://www.elastic.co/products/elasticsearch) - "Elasticsearch is a distributed, RESTful search and analytics engine capable of solving a growing number of use cases."
* [MongoDB](https://www.mongodb.com/) - "MongoDB is a document database with the scalability and flexibility that you want with the querying and indexing that you need"
* [Beanstalkd](http://kr.github.io/beanstalkd/) - "Beanstalk is a simple, fast work queue."
* [Docker](https://www.docker.com/) - "Build, Ship, and Run Any App, Anywhere"
* [Deployer](https://deployer.org/) - "Deployment Tool for PHP"
