Vagrant.configure("2") do |config|
  config.vm.provision "ansible" do |ansible|
    ansible.compatibility_mode = "2.0"
    ansible.verbose = "y"
    ansible.playbook = "vagrant.yml"
    ansible.limit = "all"
    ansible.become = true
  end

  config.vm.define "ubuntu18" do |ubuntu18|
    ubuntu18.vm.box = "geerlingguy/ubuntu1804"
  end

  config.vm.define "centos7" do |centos7|
    centos7.vm.box = "geerlingguy/centos7"
  end

  config.vm.define "debian9" do |debian9|
    debian9.vm.box = "geerlingguy/debian9"
  end


end
