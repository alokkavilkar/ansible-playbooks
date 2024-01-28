
Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/xenial64"
  config.vm.synced_folder '.', '/home/vagrant/foo'

  config.vm.define "controller" do |controller|
    controller.vm.network :private_network, ip:"192.168.61.10"
    controller.vm.box = "ubuntu/xenial64"
    
  end

  config.vm.define "db" do |db|
    db.vm.box = "ubuntu/xenial64"
    db.vm.network :private_network, ip:"192.168.61.11"
  end

end

