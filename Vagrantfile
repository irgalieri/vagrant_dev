# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/vivid64"
  config.vm.network "forwarded_port", guest: 80, host: 8888
  config.vm.network "forwarded_port", guest: 11213, host: 11213
  config.vm.network "private_network", type: "dhcp"
  config.vm.synced_folder "./public", "/var/www/html"
  config.vm.synced_folder "./logs", "/var/log/apache2"
  config.vm.provision :shell, :path => "./bootstrap.sh"
  config.vm.provider :virtualbox do |vmUBU|
     vmUBU.customize ['modifyvm', :id,'--memory', '2048']
  end
end
