# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

	config.vm.provider "virtualbox" do |v|
  	v.memory = 2048
  	v.cpus = 2
	end

  config.vm.define "master" do |master|
    master.vm.box = "ubuntu/focal64"
    master.vm.hostname = "master"
    master.vm.network "private_network", ip: "192.168.63.10"
    master.vm.network "forwarded_port", guest: 6443, host: 6443
  end

  config.vm.define "worker" do |worker|
    worker.vm.box = "ubuntu/focal64"
    worker.vm.hostname = "worker"
    worker.vm.network "private_network", ip: "192.168.63.20"
  end

end

