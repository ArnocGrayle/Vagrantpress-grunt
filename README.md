# Cohaesus VagrantPress
Forked from VagrantPress (http://vagrantpress.org/) this project is a packaged development environment for Wordpress. 

## Requirements
* [Vagrant](http://www.vagrantup.com/)
* [VirtualBox](https://www.virtualbox.org/) or [VMWare Fusion 5](http://www.vmware.com/products/fusion/overview.html)

## What's inside?
* Latest version of Wordpress
* [Grunt.js / Bower](http://gruntjs.com/)
* [Bones - Wordpress theme boilerplate](http://themble.com/bones/)
* PHP5
* Mysql 

## Get Started
Clone this project, and from the root of this project start the vm with the following command
	
	vagrant up

This creates the VM with the default virtualbox provider, you can specify the provider (such as VMWare Fusion 5) with the following
	
	vagrant up --provider vmware_fusion

The VM will start up and in the process will pull and install the latest version of Wordpress, 
and create the symlinks nessecary to run the project. Once complete you can view the 
project on 

	http://localhost:8080

## Start developing

You can ignore the */wordpress* directory as nothing in here should be edited. All
development files are contained in */source* where you will find plugins, themes and wp-config.
The contents of */source* are symlinked to the */wordpress* directory.

## Defaults
* Default Wordpress login is username: 'admin' and password: 'vagrant'
* To login to anything in the VM the password should be 'vagrant' (MySQL for example)