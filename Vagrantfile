# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "geerlingguy/centos7"

  config.vm.network :private_network, ip: "192.168.99.9"

  config.ssh.insert_key = false
  # We will use Ansible synchronize to copy files
  # config.vm.synced_folder ".", "/vagrant", disabled: true

  config.vm.provider :virtualbox do |vb|
    vb.customize ["modifyvm", :id, "--memory", 512]
    # vb.customize ["modifyvm", :id, "--vtxvpid", "off"]
    # vb.customize ["modifyvm", :id, "--cpus", "1"]
  end

  config.vm.provision :ansible do |ansible|
    ansible.playbook = "playbooks/main.yml"
  end
end
