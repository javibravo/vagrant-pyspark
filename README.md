# Vagrant-PySpark

Vagrant-PySpark is a Vagrant box with **Spark 1.6.3** installed, ready to run
Spark jobs (included PySpark) and unit testing for PySpark.

It is intended to be used only for development and testing with small data sets.

## Required

* [Vagrant](https://www.vagrantup.com/)
* [Ansible](https://www.ansible.com/)

## How to use

### Clone your projects
Set up the Vagrant box and clone your projects inside to run you jobs and tests.

### Sync you projects folder
You can fork this repo and extend the Vagrant file to sync your project folders
in the Vagrant box. It will allow you to have all your changes immediatally 
available to run in the Vagrant box.

```ruby
config.vm.synced_folder "/Project/path/in/host/machine", "/Destination/in/vagrant/box"
```

### Copy this project
You can copy this project inside you Spark project and have all together.

## PySpark Unit Testing
You can find good explanation and examples [here](https://github.com/kawadia/pyspark.test)
