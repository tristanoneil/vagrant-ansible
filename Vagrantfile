Vagrant.configure('2') do |config|
  config.vm.box = 'hashicorp/precise32'
  config.vm.network :private_network, ip: '172.0.1.50'

  config.vm.provision 'ansible' do |ansible|
    ansible.verbose = 'v'
    ansible.playbook = 'provisioning/playbook.yml'
    ansible.sudo = true
  end
end
