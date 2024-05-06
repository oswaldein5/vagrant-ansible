# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
	config.vm.box = "bento/ubuntu-22.04"
	
	config.vm.network "forwarded_port", guest: 80, host: 80

	config.vm.synced_folder "files", "/home/vagrant",
		owner: "vagrant",
		group: "vagrant"

	config.vm.provider "virtualbox" do |vb|
		vb.memory = "2048"
	end

	config.vm.provision "shell", inline: <<-SHELL
		sudo apt update
		sudo apt install ansible -y
	SHELL

	config.vm.provision "shell", path: "run_ansible.sh"
end
