# bap-vm
Virtual Machines for bap-seminar repo

## Download VirtualBox
Download the installer and extension pack for your OS from https://www.virtualbox.org/wiki/Downloads

On a Mac, simply run the following from terminal (root password will be asked):
```
$ brew tap caskroom/cask
$ brew cask install virtualbox virtualbox-extension-pack
```
## Download the VM image
Get the VDI image from [here](./vdi/lubuntu-bap-vm.vdi)

## Import VM into VirtualBox

Click `New` to create a new instance for the guest OS, then press the `Expert Mode` button.
![First step](./img/vb1.png)

The guest OS is a Linux (Lubuntu) 64-bit; make sure to assign at least 2 Gb of memory. Finally, brose the location on your hard-drive where you stored the VDI.
![Second step](./img/vb2.png)



