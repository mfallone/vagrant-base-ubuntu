# This is a simple vagrant file which will pull and install 
# the version of ubuntu listed.
# Move to the directory of this file and run `vagrant up`
# The first run will take extra time due to having to download the vm image
Vagrant.configure(2) do |config|
    config.vm.box = "ubuntu/bionic64"
    #config.vm.network "public_network", type: "dhcp", bridge: "<interfacename>"
    config.vm.network "public_network", type: "dhcp"
    config.vm.provision :shell, path: "bootstrap.sh"
    config.vm.provider "virtualbox" do |v|
        v.name = "my_test_vm"
    end
end

