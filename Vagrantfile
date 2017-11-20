# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure(2) do |config|
  # The most common configuration options are documented and commented below.
  # For a complete reference, please see the online documentation at
  # https://docs.vagrantup.com.

  # Every Vagrant development environment requires a box. You can search for
  # boxes at https://atlas.hashicorp.com/search.
  # Uses non official box for ubuntu xenial 64, as offical ubuntu package is
  # not compliant to vagrant standards...
  # Box supports virtual box, vmware and parallels provider
  config.vm.box = "bento/ubuntu-16.04"

  # Disable automatic box update checking. If you disable this, then
  # boxes will only be checked for updates when the user runs
  # `vagrant box outdated`. This is not recommended.
  # config.vm.box_check_update = false

  # Create a forwarded port mapping which allows access to a specific port
  # within the machine from a port on the host machine. In the example below,
  # accessing "localhost:8080" will access port 80 on the guest machine.
  # config.vm.network "forwarded_port", guest: 80, host: 8080
  # config.vm.network "forwarded_port", guest: 443, host: 8443

  # Create a private network, which allows host-only access to the machine
  # using a specific IP.
  config.vm.network "private_network", ip: "11.11.11.111"
  config.vm.hostname = "app.dev"

  # config.vm.synced_folder "htdocs", "/home/vagrant/htdocs", type: "rsync", rsync_exclude: ".git/"
  # config.vm.synced_folder "craft", "/home/vagrant/craft", type: "rsync", rsync_exclude: ".git/"
  # config.vm.synced_folder "log", "/home/vagrant/log", type: "rsync", rsync_exclude: ".git/"

  config.vm.synced_folder "htdocs", "/home/vagrant/htdocs", type: "nfs"
  config.vm.synced_folder "craft", "/home/vagrant/craft", type: "nfs"
  config.vm.synced_folder "log", "/home/vagrant/log", type: "nfs"

  config.vm.provider "virtualbox" do |vb|
    vb.memory = "2048"
    vb.cpus = 2
    vb.customize ["modifyvm", :id, "--ioapic", "on"]
    # vb.gui = true
  end

  config.vm.provider "vmware_fusion" do |vm|
    vm.vmx["memsize"] = "2048"
    vm.vmx["numvcpus"] = "2"
  end

  config.vm.provider "parallels" do |prl|
    prl.name = "vagrant"
    prl.memory = 2048
    prl.cpus = 2
    prl.linked_clone = true
    prl.check_guest_tools = true
    prl.update_guest_tools = true
  end

  # SSH Configuration Options
  config.ssh.forward_agent = true
  config.ssh.username = "vagrant"
  config.ssh.password = "vagrant"
  config.ssh.insert_key = true
  #config.ssh.host = "11.11.11.111"
  #config.ssh.port = "22"

  config.vm.provision "ansible_local" do |ansible|
    ansible.install_mode = :pip
    ansible.version = "latest"
    ansible.playbook = "environment/playbook.yml"
    # ansible.galaxy_role_file = "environment/requirements.yml"
    # ansible.verbose = true
  end

end
