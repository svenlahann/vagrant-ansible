vagrant debian jessie lamp setup
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
* Ports: 80 => 8080, 8000 => 8000, 443 => 8443

Shares
------
* /craft
* /htdocs
* /log

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
* apache solr

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
* laravel

Links
-----
* [Ansible](http://www.ansible.com) - "The simplest way to automate." 
* [Vagrant](https://www.vagrantup.com) - "Development environments made easy."
* [Composer](https://getcomposer.org) - "Dependency Manager for PHP"
* [Symfony Installer](https://symfony.com/doc/current/book/installation.html) - "Installing the Symfony Installer"
* [Drush](http://www.drush.org/en/master/) - "Drupal Shell"
* [Laravel Installer](https://laravel.com/docs/5.2#installing-laravel) - "Via Laravel Installer"