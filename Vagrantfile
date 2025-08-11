Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/jammy64"
  config.vm.hostname = "server-auditor"
  config.vm.network "private_network", ip: "192.168.56.10"
  config.vm.synced_folder ".", "/vagrant"

  # VM resources first
  config.vm.provider "virtualbox" do |vb|
    vb.memory = "1024"
    vb.cpus = 2
  end

  # Provision after hardware setup
  config.vm.provision "shell", inline: <<-SHELL
    sudo apt update && sudo apt upgrade -y
    sudo apt install -y git curl nano make
  SHELL
end
