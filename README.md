# Centos7 for Vagrant (virtualbox)

This repo contain definition files to build a
[Vagrant](http://www.vagrantup.com) box based latest CentOS 7 iso image.
This definition is made for fully-automated installation. 

**NOTICE!** When virtualbox window opens, and you'll see a countdown for starting installation,
DON'T DO ANYTHING! Installation will proceseed further automatically in few seconds!

##Dependencies

You need to install [Vagrant](http://www.vagrantup.com) and
[veewee](https://github.com/jedi4ever/veewee) with your favorite package
manager to build the image.

##Running

Checkout this repo. You'll need inside repo directory to build a box.

Just run the following command in the repository root:

    $ veewee vbox build CentOS-7.1
    $ veewee vbox export CentOS-7.1

##Troubleshoot

* If you can't authentificate to vagrant image please do this: `config.ssh.insert_key = false` in your Vagrantfile
