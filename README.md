# create 1 vm Vagrantfile, 2 core 2GB of ram
## Intro
This manual is dedicated to create create 1 vm Vagrantfile, 2 core 2GB of ram. 
Tested on Mac OS X.

## Requirements
- Oracle Virtualbox recent version installed
[VirtualBox installation manual](https://www.virtualbox.org/manual/ch01.html#intro-installing)

- Hashicorp vagrant recent version installed
[Vagrant installation manual](https://learn.hashicorp.com/tutorials/vagrant/getting-started-install)

- git installed
[Git installation manual](https://git-scm.com/download/mac)

## Preparation 
- Clone git repository. 

```bash
git clone https://github.com/antonakv/vagrant-ob-cpuram
```

Expected command output looks like this:

```bash
Cloning into 'vagrant-ob-cpuram'...
remote: Enumerating objects: 12, done.
remote: Counting objects: 100% (12/12), done.
remote: Compressing objects: 100% (12/12), done.
remote: Total 12 (delta 1), reused 3 (delta 0), pack-reused 0
Receiving objects: 100% (12/12), done.
Resolving deltas: 100% (1/1), done.
```

- Change folder to vagrant-ob-cpuram

```bash
cd vagrant-ob-cpuram
```

## Provisioning

- In the same folder you were before run 

```bash
vagrant up
```

Sample result

```bash
$ vagrant up
Bringing machine 'mysql' up with 'virtualbox' provider...
==> mysql: Importing base box 'aakulov/mysql64'...
==> mysql: Matching MAC address for NAT networking...
==> mysql: Checking if box 'aakulov/mysql64' version '21.03.11' is up to date...
==> mysql: Setting the name of the VM: vagrant-ob-cpuram_mysql_1615464256180_16190
==> mysql: Clearing any previously set network interfaces...
==> mysql: Preparing network interfaces based on configuration...
    mysql: Adapter 1: nat
    mysql: Adapter 2: hostonly
==> mysql: Forwarding ports...
    mysql: 22 (guest) => 2222 (host) (adapter 1)
==> mysql: Running 'pre-boot' VM customizations...
==> mysql: Booting VM...
==> mysql: Waiting for machine to boot. This may take a few minutes...
    mysql: SSH address: 127.0.0.1:2222
    mysql: SSH username: vagrant
    mysql: SSH auth method: private key
    mysql: 
    mysql: Vagrant insecure key detected. Vagrant will automatically replace
    mysql: this with a newly generated keypair for better security.
    mysql: 
    mysql: Inserting generated public key within guest...
    mysql: Removing insecure key from the guest if it's present...
    mysql: Key inserted! Disconnecting and reconnecting using new SSH key...
==> mysql: Machine booted and ready!
==> mysql: Checking for guest additions in VM...
==> mysql: Setting hostname...
==> mysql: Configuring and enabling network interfaces...
==> mysql: Mounting shared folders...
    mysql: /vagrant => /Users/aakulov/Documents/Development/Hashicorp/vagrant-ob-cpuram
```
