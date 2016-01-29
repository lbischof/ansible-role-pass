# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  config.vm.define "jessie" do |jessie|
    jessie.vm.box = "debian/jessie64"
  end

  config.vm.define "precise" do |precise|
    precise.vm.box = "ubuntu/precise64"
  end

  config.vm.define "trusty" do |trusty|
    trusty.vm.box = "ubuntu/trusty64"
  end

  config.vm.define "centos7" do |centos7|
    centos7.vm.box = "centos/7"
  end

  config.vm.define "fedora22" do |fedora22|
    fedora22.vm.box = "box-cutter/fedora22"
  end

  config.vm.provision "ansible" do |ansible|
      ansible.playbook = 'tests/test.yml'
  end
  config.vm.synced_folder ".", "/vagrant", disabled: true
end
