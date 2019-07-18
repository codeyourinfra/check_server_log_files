# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.define "jenkins" do |jenkins|
    jenkins.vm.box = "codeyourinfra/jenkins"
    jenkins.vm.network "private_network", ip: "192.168.33.10"
  end

  config.vm.provider "virtualbox" do |v|
    v.linked_clone = true
  end
end
