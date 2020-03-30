Vagrant.configure("2") do |config|
config.vm.provision "shell", path: "install-apache.sh"
 config.vm.define "web_1" do |w1|
   w1.vm.box = "ubuntu/xenial64"
   w1.vm.synced_folder "www_1", "/var/www/html"
   w1.vm.network "forwarded_port", guest: 80, host: 8080
 end
 config.vm.define "web_2" do |w1|
   w1.vm.box = "ubuntu/bionic64"
   w1.vm.synced_folder "www_2", "/var/www/html"
   w1.vm.network "forwarded_port", guest: 80, host: 8008
   w1.vm.provision "shell", inline: "apt-get update && apt-get install -y htop"
 end
end
