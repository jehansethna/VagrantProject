# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
  # The most common configuration options are documented and commented below.
  # For a complete reference, please see the online documentation at
  # https://docs.vagrantup.com.

  # Every Vagrant development environment requires a box. You can search for
  # boxes at https://atlas.hashicorp.com/search.
  config.vm.box = "hashicorp/precise64"
  config.vm.provision "shell", inline: <<-SHELL
     apt-get update
     apt-get install -y python-pip
     pip install boto3
     apt-get install tmux
     apt-get install -y git
     wget https://packages.chef.io/stable/ubuntu/12.04/chefdk_0.15.15-1_amd64.deb --no-check-certificate
     dpkg -i chefdk*.deb
     rm chefdk*.deb
  SHELL
end
