dockerdemo
==========

Scripts to make it quicker to build a VM to demo Docker.

about
-----
These scripts assume you have a Linux desktop or server already installed inside your virtual machine. (To stop getting space warnings allocate 10GB+ hard disk.)

They were originally written for a training session at BDLSS (Bodleian Digitial Libary Services and Support) part of the Bodleian Libraries at the University of Oxford.

Visit their website at: http://www.bodleian.ox.ac.uk/bdlss

scripts
-------
The scripts all contain a number, this give a rough indication of when to run it.

* 991 - run once - restart - will install docker and configure username *bdlss* (who must exist)
* 992 - run once - will pull a set of images (run again to pull the latest versions)
* 101 - simple demo with pausing - starts 3 versions of postgresql, stops and deletes them
