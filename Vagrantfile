Vagrant.configure(2) do |config|
    config.vm.box = "ubuntu/trusty64"
    config.vm.hostname = "pim.be"
    config.vm.synced_folder "C:/Users/Pim/Devops_Vagrant/do_ex1", "/vagrant"
    config.vm.network "forwarded_port", guest: 40, host: 4040
    config.vm.provision  "shell", path: "provision_nginx.sh"
    config.vm.provision  "shell", path: "provision_php.sh"
end