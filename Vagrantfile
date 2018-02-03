Vagrant.configure(2) do |config|

  config.vm.box = "ubuntu/trusty32"
  config.vm.network "private_network", ip: "192.168.49.2"
  config.vm.hostname = "qa-server"

  config.vm.provision :shell, :path => "vm_provisioner/script.bs"

  config.push.define "ftp" do |push|
    push.host = "127.0.0.1:2202"
    push.username = "vagrant"
    push.password = "vagrant"
  end

end
