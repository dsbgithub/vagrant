Vagrant.configure("2") do |config|
  config.vm.box = "hashicorp/precise32"
  config.vm.hostname= "web-dev"
  
  config.vm.provision "shell", path: "provision.sh"
  config.vm.network "forwarded_port", guest:80, host: 8080, id: "nginx" auto_correct:true
end
