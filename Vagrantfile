Vagrant.configure("2") do |config|
  config.vm.define "server" do |server|
    server.vm.box = "debian/bullseye64"
    server.vm.hostname = "server"
    server.vm.network "private_network", ip: "192.168.50.10"
    server.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
      vb.cpus = 1
    end
  end

  config.vm.define "client" do |client|
    client.vm.box = "debian/bullseye64"
    client.vm.hostname = "client"
    client.vm.network "private_network", ip: "192.168.50.11"
    client.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
      vb.cpus = 1
    end
  end
end
