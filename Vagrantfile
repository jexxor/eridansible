Vagrant.configure("2") do |config|
  config.vm.box = "generic/debian12"
  config.vm.hostname = "eridansible"
  config.vm.network "private_network", ip: "192.168.10.100"

  config.vm.provider :libvirt do |libvirt|
    libvirt.memory = 2048
    libvirt.cpus = 2
  end
end