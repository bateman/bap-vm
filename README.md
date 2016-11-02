# bap-vm
Virtual Machine for [Best-Answer Prediction seminar](https://github.com/bateman/bap-seminar)

## Download VirtualBox
Download the installer and extension pack for your OS from https://www.virtualbox.org/wiki/Downloads

On a Mac with `Homebrew` already installed, simply run the following from terminal (root password will be asked):
```
$ brew tap caskroom/cask
$ brew cask install virtualbox virtualbox-extension-pack
```
## Download the VM image
The Virtual Box image is based on Lubuntu 16.04 LTS Xenial Xerus, obtained from [osboxes.org](http://www.osboxes.org/virtualbox-images/). Download the (compressed) VDI image from here: [32bit](https://drive.google.com/open?id=0B89FZverAlQVTm52TzBvaFdCWDA) | [64bit](https://drive.google.com/file/d/0B89FZverAlQVZkdTV3FxdlFfTnc).

## Import VM into VirtualBox

Click `New` to create a new instance for the guest OS, then press the `Expert Mode` button.
![](./img/vb1.png)

The guest OS is a Linux (Lubuntu): pleae, select 64 or 32 bit, depending on your host machine architecture; also, make sure to assign at least 2 Gb of memory. Finally, brose the location on your hard-drive where you stored the VDI file.
![](./img/vb2.png)

## Further config

You might want to fine-tune the config for your guest OS according to the host machine. Click on `Settings`. At least, consider enabling bidirectional copy-and-paste between the two OS's, as shown in the picture below.
![](./img/vb3.png)

## Run

Simply click the green arrow `Start` to run the guest OS.


## Other info
Automatic login is set at startup. User credentials are the following:
```
Username: osboxes
Password: osboxes.org
```
These will be necessary for executing administrive (root) changes.

## Guest Additions (optional)

Should your screen size be quite small, it means that you need to install the Guest Additions. Mount the ISO as shown in the picture below. Then, open terminal and browse to the mount location, which will be something like `/media/osboxes/VBOXADDITIONS_5.1.6_110634/` (note that the version may vary).

![](./img/vb4.jpg)

Now, simply run `sudo ./VBoxLinuxAdditions.run` and reboot the guest OS.

