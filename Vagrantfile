# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  config.vm.hostname = "prometheus.local"

  config.vm.define :server do |server|
    server.vm.hostname = "server.prometheus.local"
    server.vm.network :private_network, ip: "192.168.10.11"
  end

  config.vm.define :node do |node|
    node.vm.hostname = "node.prometheus.node"
    node.vm.network :private_network, ip: "192.168.10.21"
  end
end
