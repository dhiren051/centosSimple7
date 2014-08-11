# centosSimple7
####Codename: surly-snatch

This is my **first** Vagrant base box with a clean, manual install of the latest 64-bit CentOS server install. After I've gotten the formula down, I'll auto-build with Packer.

Very shortly I'll include some `BASH` shell automation (`bootstrap.sh`) to work out a quick draft of some requirements. Within a few months the BASH automation will be replaced with `Python` & `Puppet`automation.

You are free to use it but please keep in mind: This is for my personal experimentation; it's really just for *me*.

It's available now at [Vagrant Cloud](https://vagrantcloud.com/todd_dsm/centosSimple7) repo.

##Highlights
* CentOS 7.0-1406 x86_64 (Minimal ISO)
* TESTING ONLY (for now)
* Auto-Build: Packer (coming shortly)
* Auto-Conf:  BASH   (coming shortly)
* Auto-Conf:  Python (coming much later; stay tuned)
* I will make every attempt to *always* keep this the latest version of CentOS 7.

##To Use
```
cd    ~/projectDirectory/              (where you keep all of your other projects)
git clone https://github.com/todd-dsm/centosSimple7.git
mv centosSimple7/ newProjectName       (whatever you want to call it)
cd newProjectName/
vagrant up
vagrant ssh
```
After logging in as the user `vagrant` you can become `root` by entering: `sudo su -`

####That's it! 
You can now begin *your* experimentation.

##BASE Configuration
These services are enabled but not hardened:
* SSH
* NTP
* SELinux: enabled
* [Vagrant Keys](https://github.com/mitchellh/vagrant/tree/master/keys)
* VBoxGuestAdditions-4.3.14

##Provider Support
* VirtualBox (confirmed; built on vbox)
* VMware (unconfirmed)
* Some third option (unconfirmed)

##Cloud Support
* None - *yet*.

##Totally Unsupported
Non-constructive Feedback, including but not limited to BWRC:
 * Bitching
 * Whining, or
 * Recreational Complaining

All else is not only encourage but rewarded.

Cheers
