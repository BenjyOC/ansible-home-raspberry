Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/groovy64"

  config.vm.provider "virtualbox" do |vb|
    vb.memory = "1024"
  end

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
    ansible.ask_vault_pass = true
  end
end
