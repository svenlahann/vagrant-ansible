vagrant jessie lamp setup
=========================

**vagrant setup for modern php projects**

Requirements
------------

* [Vagrant](https://www.vagrantup.com/)
* [Ansible](http://www.ansible.com/)

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
* RAM: 1GB

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
* tomcat7

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

Links
-----
* [Ansible](http://www.ansible.com) - "The simplest way to automate." 
* [Vagrant](https://www.vagrantup.com) - "Development environments made easy."
* [Composer](https://getcomposer.org) - "Dependency Manager for PHP"
* [Symfony Installer](https://symfony.com/doc/current/book/installation.html) - "Installing the Symfony Installer"