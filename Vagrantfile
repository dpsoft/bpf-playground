# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    config.vm.box = "generic/fedora32"
    config.vm.provision :shell, :privileged => false, :path => "scripts/install-bcc.sh"
end