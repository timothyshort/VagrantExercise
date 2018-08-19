Vagrant.configure(2) do |config|

  config.vm.box = "ubuntu/trusty32"
  config.vm.network "private_network", ip: "192.168.49.2"
  config.vm.hostname = "qa-server"
  
  #define synced folder
  config.vm.synced_folder "src/", "/home/vagrant"

  #run provisioning script
  config.vm.provision :shell, :path => "vm_provisioner/script.bs"

end
