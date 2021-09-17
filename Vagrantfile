# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    #config.vm.synced_folder '.', '/vagrant', disabled: true
    config.vm.define "master" do |m|
        m.vm.box = "ubuntu/focal64"
          m.vm.hostname = "flask.localhost"
        m.vm.provider :virtualbox do |vb|
          vb.customize [ 'modifyvm', :id, '--memory', '1024' ]
          vb.customize [ 'modifyvm', :id, '--cpus', '1' ]
          vb.customize [ 'modifyvm', :id, '--name', 'flask-app' ]
          #config.vm.provider "virtualbox" do |vb|
           # vb.customize [ "modifyvm", :id, "--uartmode1", "disconnected" ]
          #end
        end
    end
  end
  
  