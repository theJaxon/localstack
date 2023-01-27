Vagrant.configure("2") do |config|
  config.vm.box = "almalinux/9"
  config.vm.box_version = "9.0.20221003"
  config.vm.hostname = "almalinux"
  config.vm.synced_folder ".", "/vagrant", type: "virtualbox"
  config.vm.box_check_update = false
  config.vm.network "private_network", ip: "192.168.80.120"
  config.vm.provider "virtualbox" do |vb|
    vb.name   = "almalinux"
    vb.cpus   = 2
    vb.memory = "4096"
  end

  config.vm.provision "ansible_local" do |ansible|
    ansible.playbook = "localstack.yml"
    ansible.become   = true
  end
end