# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  config.vm.box = "ubuntu/trusty64"
  config.vm.define "pyspark-box"

  # config.vm.network :private_network, ip: "192.168.33.44"

  config.vm.provider "virtualbox" do |v|
    v.memory = 2048
  end

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "ansible/playbook.yml"
    ansible.verbose = 'vvvv'
  end

end
