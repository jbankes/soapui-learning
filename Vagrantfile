# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"

  # Port Forwarding
  config.vm.network "forwarded_port", guest: 8080, host: 8080

  # Synced Folder
  config.vm.synced_folder ".", "/home/vagrant/app"

  # Config VB
  config.vm.provider "virtualbox" do |vb|
    # Customize the amount of memory on the VM:
    vb.memory = "4096"
  end
 
end
