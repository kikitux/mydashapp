Vagrant.configure("2") do |config|
  config.vm.box = "alvaro/xenial64"
  config.vm.hostname = "dash01"
  config.vm.network "forwarded_port", guest: 8050, host: 8050
  config.vm.provision "shell", path: "scripts/provision.sh", privileged: false
  config.vm.provision "shell", path: "scripts/runme.sh", privileged: false, run: "always"
end
