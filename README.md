vagrant debian lamp setup
================================

**vagrant setup for modern php projects**

Requirements
------------

* [Vagrant](https://www.vagrantup.com/)
* [VirtualBox](https://www.virtualbox.org/)
* [Ansible](http://www.ansible.com/)

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
* php
* exim4
* git
* midnight commander
* java openjdk

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

Links
-----
* [Ansible](http://www.ansible.com) - "The simplest way to automate." 
* [Vagrant](https://www.vagrantup.com) - "Development environments made easy."
* [Composer](https://getcomposer.org) - "Dependency Manager for PHP"
* [Symfony Installer](https://symfony.com/doc/current/book/installation.html) - "Installing the Symfony Installer"
* [Drush](http://www.drush.org/en/master/) - "Drupal Shell"
* [Drupal Console](https://drupalconsole.com/) - "The new CLI for Drupal"
* [Laravel Installer](https://laravel.com/docs/5.2#installing-laravel) - "Via Laravel Installer"