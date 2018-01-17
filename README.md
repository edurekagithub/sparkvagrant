# Installing Spark environment in Vagrant
The goal of this post is to setup spark environment in vagrant environment, so that it doesn't corrupt of affect the base OS. 

Vagrant is an open-source software product for building and maintaining portable virtual software development environments,[4] e.g. for VirtualBox, Hyper-V, Docker, VMware, and AWS. More information can be found on https://www.vagrantup.com/intro/getting-started/index.html

## Installing vagrant
Follow the vagrant getting started guide https://www.vagrantup.com/intro/getting-started/index.html
Below are the steps:
* Install vagrant
Download package from https://www.vagrantup.com/downloads.html
* Project Setup
```
$ mkdir vagrant_getting_started
$ cd vagrant_getting_started
$ vagrant init
```
* Installing Box
```
$ vagrant box add hashicorp/precise64
```
** Edit the Vagrantfile
```
Vagrant.configure("2") do |config|
  config.vm.box = "hashicorp/precise64"
end
```
* Starting the machine
```
$ vagrant up
$ vagrant ssh
```
## Installing Java
## Installing Scala
## Installing Hadoop
## Installing Apache Spark
## Installing Apache Livy
## Installing Mysql

