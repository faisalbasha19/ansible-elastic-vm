Vagrant.configure("2") do |config|
    config.vm.box = "bento/ubuntu-20.04"
 
    config.vm.define "ansible-master" do |master|
        master.vm.network "public_network"
        master.vm.provider "virtualbox" do |vb|
            vb.gui = false
            vb.name = "ansible-master"
            vb.memory = "2048"
        end
    end

    config.vm.define "elk-node1" do |elk1|
        elk1.vm.network "public_network"
        elk1.vm.provider "virtualbox" do |vb|
            vb.gui = false
            vb.name = "elk-node1"
            vb.memory = "2048"
        end
    end

    config.vm.define "elk-node2" do |elk2|
        elk2.vm.network "public_network"
        elk2.vm.provider "virtualbox" do |vb|
            vb.gui = false
            vb.name = "elk-node2"
            vb.memory = "2048"
        end
    end

    config.vm.box_check_update = false 
end
