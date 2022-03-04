Vagrant.configure("2") do |config|

	if Vagrant.has_plugin? "vagrant-vbguest"
		config.vbguest.no_install = true
		config.vbguest.auto_update = false
		config.vbguest.no_remote = true
	end
 
	 config.vm.define :servidorpxe do |servidorpxe|
		servidorpxe.vm.box = "centos/stream8"
		servidorpxe.vm.network :private_network, ip: "192.168.0.2"
		servidorpxe.vm.hostname = "servidorpxe"
	 end
end