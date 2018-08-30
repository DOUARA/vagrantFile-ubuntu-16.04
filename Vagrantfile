# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-16.04"
  config.ssh.username = 'root'
  config.ssh.insert_key = 'true'
  config.vm.synced_folder ".", "/docker-vagrant"
  config.vm.network "forwarded_port", guest: 1992, host: 8080, host_ip: "127.0.0.1"
end
