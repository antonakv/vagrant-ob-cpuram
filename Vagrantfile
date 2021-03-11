Vagrant.configure("2") do |config|  
  config.vm.provider "virtualbox" do |v|
    v.memory = 2048
    v.cpus = 2
  end

  config.vm.define vm_name="mysql" do |mysql|
    mysql.vm.box = "aakulov/mysql64"
    mysql.vm.hostname = vm_name
    mysql.vm.network "private_network", ip: "192.168.102.101"
  end

end