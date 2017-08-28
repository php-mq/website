VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.box = "DreiWolt/devops007"
  config.vm.network :private_network, ip: "192.168.3.21"
  config.vm.hostname = "Website"
  config.hostsupdater.aliases = ["dev.dev.php-mq.org.de", "pma.dev.php-mq.org.de", "readis.dev.php-mq.org.de"]
  config.vm.synced_folder ".", "/vagrant", type: "nfs"
  config.vm.provision "shell", path: "env/bootstrap.sh", run: "always"

end
