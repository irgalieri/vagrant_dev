# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/vivid64"
  config.vm.network "forwarded_port", guest: 80, host: 8080
  config.vm.network "private_network", ip: "192.168.33.10"
  config.vm.synced_folder "./public", "/var/www/html"
  config.vm.synced_folder "./logs", "/var/log/apache2"
  config.vm.provision :shell, :path => "./bootstrap.sh"
end
