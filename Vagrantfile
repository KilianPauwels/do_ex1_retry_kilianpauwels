Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.hostname="pauwelsk"
  config.vm.network "forwarded_port", guest: 80, host: 8080
  config.vm.provision "shell", inline: "echo hello"
  config.vm.provision "shell", path: "provision_nginx.sh"
  config.vm.provision "shell", path: "provision_php.sh"
end
