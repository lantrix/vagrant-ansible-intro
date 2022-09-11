# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  # General Vagrant VM configuration
  config.vm.box = "centos/7"

  # Ansible demo server
  config.vm.define "ansible-demo" do |server|
    server.vm.hostname = "ansible-demo"
  end

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
  end
end
