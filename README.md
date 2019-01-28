This project is about:

     What is zero day? 
Is like an attack to an app or system by writting malicious code. 
It just because is known the vulnerability of the system.
This vulnerability in general is unknown by the user even for the vendor of the targeted system.
Until the vulnerability in mitigated, hackers can affects computer programs, data, other computers or even a network.

     What is a virtual machine?
Is an emulator os a computer system. Defined by Popek and Goldberg like a isolate duplicate of a real computer
There are different fuctions:
-System virtual machines or full virtualization VMS-->execute entire operating systems. (ex.Windows,Linux)
-Process virtual machines-->execute computer programs in a platform-independent environment.

     How to run Ubuntu on the Holberton computers?
p7-3:~ 27$ vagrant box list
modernIE/w10-edge (virtualbox, 0.0.3)
ubuntu/trusty64 (virtualbox, 20160108.0.0)

p7-3:~ 27$ export VAGRANT_HOME=/Users/Shared/.vagrant.d/

to inicite vagrant -->vagrant init

then open the file with an editor an replace "base" with the Ubuntu VM name in this case "ubuntu/trusty64"

to go into the VM run vagrant ssh command

the result: 
vagrant@vagrant-ubuntu-trusty-64:~$

     Using Vagrant on your personal computer Mac OSx
Donwnload virtual box from https://www.virtualbox.org/wiki/Downloads
install virtual box
Download Vagrant from https://www.vagrantup.com/downloads.html
install vagrant
Open the terminal application and the lines starts with "$"
Add the Ubuntu 14.04 (Trusty) image to your box list: $ vagrant box add ubuntu/trusty64 Warning: this step can take time
create a virtual machine
$ vagrant init ubuntu/trusty64-> it will generate a Vagrantfile with base = "ubuntu/trusty64" - you don’t have to execute this command line everyday, only once, to create a new virtual machine 
$ vagrant up -->itl will start your virtual machine
$ vagrant ssh -->Now you are inside your virtual machine
