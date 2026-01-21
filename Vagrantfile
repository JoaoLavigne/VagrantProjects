Vagrant.configure("2") do |config|
  config.vm.box = "hashicorp-education/ubuntu-24-04"
  config.vm.network  "public_network"

  config.vm.provider "virtualbox" do |vb|
    vb.name = "second_project_vagrant"
  end

  config.vm.provision "shell" do |s|
    s.inline = <<-SHELL
      apt-get update
      apt-get install -y vim nginx telnet htop nmap net-tools wget unzip curl
      useradd -m -s /bin/bash Joao
    SHELL
  end

  

end
