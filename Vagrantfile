# -*- mode: ruby -*-
# vi: set ft=ruby :

# run vagrant up (name) to test a particular box

Vagrant.configure(2) do |config|
  # Ubuntu 14.04 - Trusty Tahr
  config.vm.define "ubuntu1404" do |ubuntu1404|
    ubuntu1404.vm.hostname = "ubuntu1404test"
    ubuntu1404.vm.box = "ubuntu/trusty64"
    ubuntu1404.vm.provision "ansible" do |ansible|
      ansible.playbook = "playbook.yml"
    end
  end

  # Ubuntu 12.02 - Precise Pangolin
  config.vm.define "ubuntu1204" do |ubuntu1204|
    ubuntu1204.vm.hostname = "ubuntu1204test"
    ubuntu1204.vm.box = "ubuntu/precise64"
    ubuntu1204.vm.provision "ansible" do |ansible|
      ansible.playbook = "playbook.yml"
    end
  end

  # Debian 7.4
  config.vm.define "debian7" do |debian7|
    debian7.vm.hostname = "debian7test"
    debian7.vm.box = "chef/debian-7.4"
    debian7.vm.provision "ansible" do |ansible|
      ansible.playbook = "playbook.yml"
    end
  end

  # Debian 6.4
  config.vm.define "debian6" do |debian6|
    debian6.vm.hostname = "debian6test"
    debian6.vm.box = "debian/jessie64"
    debian6.vm.provision "ansible" do |ansible|
      ansible.playbook = "playbook.yml"
    end
  end

  # CentOS 7
  config.vm.define "centos7" do |centos7|
    centos7.vm.hostname = "centos7test"
    centos7.vm.box = "centos/7"
    centos7.vm.provision "ansible" do |ansible|
      ansible.playbook = "playbook.yml"
    end
  end

  # CentOS 6
  config.vm.define "centos6" do |centos6|
    centos6.vm.hostname = "centos6test"
    centos6.vm.box = "chef/centos-6.6"
    centos6.vm.provision "ansible" do |ansible|
      ansible.playbook = "playbook.yml"
    end
  end
end