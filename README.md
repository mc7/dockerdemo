dockerdemo
==========

Scripts to make it quicker to build a VM to demo Docker.

about
-----
These scripts assume you have a Linux desktop or server already installed inside your virtual machine. (To stop getting space warnings allocate 12GB+ hard disk.)

They were originally written for a training session at BDLSS (Bodleian Digitial Libary Services and Support) part of the Bodleian Libraries at the University of Oxford.

Visit their website at: http://www.bodleian.ox.ac.uk/bdlss

scripts
-------
The scripts all contain a number, this give a rough indication of when to run it.

* 101 - simple demo with pausing - starts 3 versions of postgresql, stops and deletes them
* 103 - demo of complex system in single image
* 105 - demo of splitting system into sub-system images and linking
* 501 - will stop all containers and delete all containers, with warning first.

Setup scripts

* 991 - run once - restart - will install docker and configure username *demo* (who must exist)
* 992 - run once - will pull a set of images (run again to pull the latest versions)

new computer
------------
To demo on a new computer do this:

sudo apt-get install git
git clone https://github.com/mc7/dockerdemo.git
cd dockerdemo/
ls
./bdlss998_support
./bdlss991_docker_install
reboot

Script 998 set up the bin folder as a link so commands work from anywhere. The following will add the images, git repos an some images for demos.
bdlss992_pull_images
bdlss993_gitpulls
bdlss994_dpulls

At this point demos 101, 103 and 105 should work.

