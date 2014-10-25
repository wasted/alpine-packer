Vagrant.require_version ">= 1.4.3"
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
	config.vm.define "alpine" do |node|
		node.vm.provider "virtualbox" do |v|
			v.name = "alpine"
			v.customize ["modifyvm", :id, "--memory", "512"]
		end

		# don't set either, it will fail
		#node.vm.hostname = "alpine"
		#node.vm.network :private_network, ip: "10.220.43.10"
		node.vm.box = "alpine64"
	end
end
