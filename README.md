# usb-intruderer

This will be where we collect all efforts to get into the SMEG+ via one of its USB ports.

## The idea from a bird's view

While this will use some ideas from [psakey](https://github.com/Mwyann/psakey) and [smeg-plus\_key](https://github.com/bousqi/smeg-plus_key), the idea is more to use some more powerful hardware like a Beaglebone Black to pretend being all sorts of USB devices to the USB host (which in our case is the SMEG+). In particular we're hoping to play some switcheroo while pretending to be a mass storage device. But ~~yes, in all likelihood USB CDC isn't going to be supported by the SMEG+, so~~ we need to figure out what device classes we can pose as to the head unit. @bousqui has done some prior work regarding this. At this point it seems like conclusions drawn from strings?!

## Reading material

* [Pretty much a link dump about USB-related topics](https://www.devalias.net/devalias/2018/05/13/usb-reverse-engineering-down-the-rabbit-hole/)
* [sunxi Wiki namespace about USB Gadgets](http://sunxi.org/USB_Gadget)
* [USBQ Toolkit](https://usbq.org/), also [on GitHub](https://github.com/CarveSystems/usbq)
    * In part based on [USBiquitous](https://airbus-seclab.github.io/#2016) kernel module ([paper](https://airbus-seclab.github.io/usbq/SSTIC2016-Article-usb_toolkit-camredon.pdf), [kernel](https://github.com/airbus-seclab/usbq_core), [userland](https://github.com/airbus-seclab/usbq_userland))
* [Very old article about GadgetFS](http://www.linux-usb.org/gadget/) ... this may not be of too much value these days, but we found it an enlightening read
* Two-part article on how to use [GadgetFS](https://www.collabora.com/news-and-blog/blog/2019/02/18/modern-usb-gadget-on-linux-and-how-to-integrate-it-with-systemd-part-1/) and [FunctionFS](https://www.collabora.com/news-and-blog/blog/2019/03/27/modern-usb-gadget-on-linux-and-how-to-integrate-it-with-systemd-part-2/) in conjunction with systemd


> NB: No need to point out a supposed spelling mistake in the project name. It's an allusion to some of those stealth levels in [RTCW](https://en.wikipedia.org/wiki/Return_to_Castle_Wolfenstein), where the enemy soldiers are shouting "intruderer, intruderer" ... before well ... 😁
