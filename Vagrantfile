# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
  config.vm.box = "offensive-security/kali-linux"
  config.vm.hostname = 'kali-vagrant'


  config.vm.provider :virtualbox do |v|
    v.customize ["modifyvm", :id,
                 "--name", 'kali-vagrant',
                 "--memory", "2048",
                 "--nictype1", "Am79C973",
                 "--nictype2", "Am79C973",
                 "--natdnshostresolver1", "on"]
    v.gui = false
  end
end
