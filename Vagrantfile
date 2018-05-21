Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
  end
  config.vm.network "forwarded_port", guest: 1760, host: 8080
end
