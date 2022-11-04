Vagrant.configure("2") do |config|
  config.hostmanager.enabled = true 
  config.hostmanager.manage_host = true
  
  ### Master ###
  config.vm.define "master" do |master|
    master.vm.box = "bento/ubuntu-20.04"
    master.vm.hostname = "master"
    master.vm.network "private_network", ip: "192.168.56.100"
	master.vm.provider "virtualbox" do |vb|
     vb.memory = "2048"
	 end
   end
     ### Jenkins ###
  config.vm.define "jenkins" do |jenkins|
    jenkins.vm.box = "bento/ubuntu-20.04"
    jenkins.vm.hostname = "jenkins"
    jenkins.vm.network "private_network", ip: "192.168.56.200"
	jenkins.vm.provider "virtualbox" do |vb|
#     vb.memory = "1024"
	 end
   end
   ############# Node1#######
  config.vm.define "node1" do |node1|
    node1.vm.box = "bento/ubuntu-20.04"
    node1.vm.hostname = "node1"
	node1.vm.network "private_network", ip: "192.168.56.101"
  end

end