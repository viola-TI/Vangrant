Vagrant.configure("2") do |config|

  config.vm.box = "hashicorp/bionic64"
  config.vm.network "forwarded_port", guest: 80, host: 8009
  config.vm.network "public_network", ip: "192.168.0.55"
  config.vm.provision "shell", path: "script.sh"
  config.vm.synced_folder "site/" , "/var/www/html"
end



