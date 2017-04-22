HW decoder for Ubuntu Xenial Xerus 16.04 LXDE OS Image (A64)
======================================================

This is a **deb package** for the **A64** OS image providing HW decoding on mplayer.

Tested and running on the following devices (1080P hdmi):

  - BananaPi M64
  - NanoPi A64
  - Pine64

To be tested on boards below soon when i get them:

  - SOPINE (gently sent by tllim) - stuck somewhere around the globe!?
  - OPI Win

Instructions
============

  - If you have attempted to install Cedrus/vdpau previoulsy, remove it completely!
  - Clone this repo: 

		git clone https://github.com/avafinger/cedrusH264_vdpau_A64

  - Install it:

		sudo dpkg -i cedrusH264_vdpau_1.0-1.deb 

  - Reboot or shutdown depending which board you have

	sudo rebbot
	or
	sudo shutdow -h
	

