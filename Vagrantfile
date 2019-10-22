# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  ## Escolha da Box
  config.vm.box = "ubuntu/bionic64"

  ## Configuração de Rede
  config.vm.hostname = "ubuntulab"
  #config.vm.network "forwarded_port", guest: 80, host: 8080
  #config.vm.network "private_network", ip: "192.168.X.X"

  ## Configurações de Size da VM
  config.vm.provider "virtualbox" do |v|
     v.name = "ubuntu"
     v.memory = 1024
     v.cpus = 2
  end
  
  ## Opções para Configurar a Máquina sem Gerência de Configuração

  #config.vm.provision :shell, path: "shellscript.sh"

  config.vm.provision "shell", inline: <<-SHELL
    touch /tmp/teste.txt
  SHELL

end