# Minority Stories

## VM Setup
[Download and install Vagrant](http://www.vagrantup.com/downloads.html)

In the project root, run the following command in the terminal:
> $ curl -L http://rove.io/install | bash

You will likely receive an error like `Failed to mount folders`. If so, run the
following comment in the terminal:
> $ vagrant plugin install vagrant-vbguest

After the plugin is installed, `ssh` into the virtual machine:
> $ vagrant ssh

In the virtual machine, run:
> $ sudo ln -s /opt/VBoxGuestAdditions-4.3.10/lib/VBoxGuestAdditions /usr/lib/VBoxGuestAdditions

Log out of the virtual machine and run:
> $ vagrant reload

You should be good to go, and the project will be in `/vagrant` on the virtual
machine. Edit files locally, and use the VM only as your server.
