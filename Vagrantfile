# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.ssh.insert_key = false

  config.vm.define "etcd1" do |etcd|
    etcd.vm.hostname = "etcd1"
    etcd.vm.box = "centos/7"
    etcd.vm.network :private_network, ip: "192.168.0.15"
    etcd.vm.network :forwarded_port, guest: 22, host: 2215, id: "ssh"
    etcd.vm.provider "virtualbox" do |vb|
      vb.gui = false
      vb.cpus = 1
      vb.memory = 1024
    end
  end

  config.vm.define "etcd2" do |etcd|
    etcd.vm.hostname = "etcd2"
    etcd.vm.box = "centos/7"
    etcd.vm.network :private_network, ip: "192.168.0.16"
    etcd.vm.network :forwarded_port, guest: 22, host: 2216, id: "ssh"
    etcd.vm.provider "virtualbox" do |vb|
      vb.gui = false
      vb.cpus = 1
      vb.memory = 1024
    end
  end

  config.vm.define "etcd3" do |etcd|
    etcd.vm.hostname = "etcd3"
    etcd.vm.box = "centos/7"
    etcd.vm.network :private_network, ip: "192.168.0.17"
    etcd.vm.network :forwarded_port, guest: 22, host: 2217, id: "ssh"
    etcd.vm.provider "virtualbox" do |vb|
      vb.gui = false
      vb.cpus = 1
      vb.memory = 1024
    end
  end
end