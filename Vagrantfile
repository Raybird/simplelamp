# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  config.vm.box = "raybird/lamp"

  config.vm.network "forwarded_port", guest: 80, host: 1888

  config.vm.provider "virtualbox" do |vb|
    vb.memory = "1024"
  end

  config.vm.provision "shell", path: "provision/welcome.sh", run: "always"
end
