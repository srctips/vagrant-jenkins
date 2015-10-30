# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "box-cutter/centos66"
  config.vm.box_check_update = false
  config.vm.hostname = "jenkins-dev"

  config.vm.network "forwarded_port", guest: 8080, host: 8080
  
  config.vm.provider "virtualbox" do |vb|
     vb.name = "Jenkins_Development"
     vb.memory = "1024"
     vb.cpus = 2
  end
end