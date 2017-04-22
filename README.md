HW decoder for Ubuntu Xenial Xerus 16.04 LXDE OS Image (A64)
======================================================

This is a **deb package** for the **A64** OS image providing HW decoding on mplayer.

Tested and running on the following devices (1080P hdmi):

  - BananaPi M64
  - NanoPi A64
  - Pine64

To be tested on boards below as soon as i get them:

  - SOPINE (gently sent by tllim) - stuck somewhere around the globe!?
  - OPI Win

## HW decoding (1920x1080 H264) with cedrus
[![A64 Cedrus in action](https://github.com/avafinger/nanopi-a64-firmware/raw/master/img/1920x1080.jpg)](https://youtu.be/mXMOh9ShDDc)

Instructions
============

  - If you have attempted to install Cedrus/vdpau previously, remove it completely!
  - Clone this repo: 

		git clone https://github.com/avafinger/cedrusH264_vdpau_A64

  - Install it:

		sudo dpkg -i cedrusH264_vdpau_1.0-1.deb 

  - Reboot or shutdown depending which board you have

		sudo reboot
		or
		sudo shutdown -h
	
  - After rebooting or restarting your board you can test MP4 H264 (big buck bunny for example)
    with mplayer without sound to make sure cedrus is working!

		mplayer-mute big_buck_bunny_1080p_H264_AAC_25fps_7200K.MP4 

  - To play with sound (output to hdmi)

		mplayer-hdmi big_buck_bunny_1080p_H264_AAC_25fps_7200K.MP4 

  - If you are brave, you can setup audiocodec (JACK), when ready:

		mplayer-jack big_buck_bunny_1080p_H264_AAC_25fps_7200K.MP4 

Source
======

  - libcedrus
  - libvdpau-sunxi