Vagrant.configure(2) do |config|
  config.vm.box = "osx-10.11"

  config.vm.synced_folder '.', '/opt/kitchenplan', create: true, type: 'nfs'

  config.vm.provider "parallels" do |prl|
    prl.use_linked_clone = true
    prl.customize ['set', :id, '--startup-view', 'window']
  end
end
