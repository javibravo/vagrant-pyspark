# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  config.vm.box = "ubuntu/trusty64"
  config.vm.define "pyspark-box"
  # Forward ssh keys from host to guest
  config.ssh.forward_agent = true

  config.vm.provider "virtualbox" do |v|
    v.memory = 2048
  end

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "ansible/playbook.yml"
    ansible.verbose = 'v'
  end

end
