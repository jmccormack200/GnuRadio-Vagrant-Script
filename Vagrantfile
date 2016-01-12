Vagrant.configure("2") do |config|
	config.vm.box = "ubuntu/trusty64"
	config.vm.provision :shell, path: "bootstrap.sh"
	config.vm.network :forwarded_port, guest: 88, host:4568

	config.vm.provider "virtualbox" do |v|
		v.memory = 2048
		v.gui = true
	end
end
