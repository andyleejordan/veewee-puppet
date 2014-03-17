Ubuntu Server 12.04.4 LTS Vagrant VirtualBox with Puppet 3.4.3
========

Veewee definition and scripts to build a VirtualBox VM for vagrant,
based off Ubuntu Server 12.04.4 LTS (with amd64 architecture). It
includes the latest version of Puppet (3.4.3), "deep_merge" gem (for
Hiera), and VirtualBox Guest Additions.

It is setup to be dual core, with 1 GB RAM, and an 8 GB virtual
disk. It is trimmed so as to not have Chef or Ruby. It has the
packages aptitude, curl, git, gnupg2, mg, wget, and unzip
pre-installed.

This is a definition for building with
[veewee](https://github.com/jedi4ever/veewee). It fails the included
validation tests because of the (purposeful) lack of Ruby. I made it
because all the publically available Vagrant boxes lacked Puppet
3.4.3, which I need for testing my Puppet manifests.
