Vagrant.configure("2") do |config|
   config.vm.define "master" do |master|
     master.vm.box = "ubuntu/bionic64"
     master.vm.network "private_network", type: "dhcp",
        name: "vboxnet0" 
     master.vm.provider "virtualbox" do |vb|
        vb.memory = "8192"
        vb.cpus = "2"
     end
   end
   config.vm.define "slave1" do |slave1|
      slave1.vm.box = "ubuntu/bionic64"
      slave1.vm.network "private_network", type: "dhcp",
         name: "vboxnet0"
   end
end
