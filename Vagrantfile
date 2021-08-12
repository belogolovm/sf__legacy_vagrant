$script = <<SCRIPT
sudo yum install postgresql84 postgresql84-server postgresql84-contrib -y
sudo /etc/init.d/postgresql initdb
sudo /etc/init.d/postgresql start
SCRIPT
Vagrant.configure("2") do |config|
  config.vm.box = "bento/centos-5"
  config.vm.provision "shell", inline: $script
end