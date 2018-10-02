# Vagrant

[Vagrant](https://www.vagrantup.com/) is an open-source software product for
building and maintaining portable virtual software development environments.

### Installation

Vagrant uses [VirtualBox](https://www.virtualbox.org/) to manage the virtual
dependencies. You can directly [download VirtualBox](https://www.virtualbox.org/wiki/Linux_Downloads)
and install it or install the VirtualBox package which is available in the
Ubuntu's repositories:

```bash
sudo apt install virtualbox
```

You can directly [download Vagrant](https://www.vagrantup.com/downloads.html)
and install it or install the Vagrant package which is available in the
Ubuntu's repositories:

```bash
sudo apt install vagrant
```

### Usage

To create and configure the virtual machine according to the Vagrantfile:

```bash
vagrant up
```

To ssh into the virtual machine:

```bash
vagrant ssh
```

To stop the virtual machine:

```bash
vagrant halt
```

To destroy all resources that were created during the creation of the machine:

```bash
vagrant destroy
```
