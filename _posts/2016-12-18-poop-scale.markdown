---
layout: post
title:  Apache MiNiFi-CPP - USB Poop Scale
date:   2016-12-18 15:58:20 -0500
categories: Apache MiNiFi-CPP
---

One of my first observations being a father is the insane amount of time my wife and I spend discussing poopy diapers. It is a gross necessary detail of being a parent. My pediatrician (also a giant nerd like myself) recommended an IOS app where we could keep track of such primitive details and then share that data with him at visits. While my wife applauded his suggestion I couldn't help but think there had to be a better way to do this in 2016 than an app. Long story short their isn't. However this did get the wheels turning in my head. I have been spending a good bit of time lately working with Apache MiNiFi-CPP and thought this a great opportunity to show off the power of a CPP version of Apache MiNiFi.

![USB Poop Scale Architecture](https://raw.githubusercontent.com/jdye64/jdye64.github.io/master/assets/images/USB_Poop_Scale_Architecture.png)

![Apache NiFi Workflow](https://raw.githubusercontent.com/jdye64/jdye64.github.io/master/assets/images/Poop_Scale_USB_Screenshot.png "Apache NiFi Workflow")

<a href="http://www.youtube.com/watch?feature=player_embedded&v=NObOFfeHCJs
" target="_blank"><img src="http://img.youtube.com/vi/NObOFfeHCJs/0.jpg" 
alt="Apache MiNiFi-CPP Poopy Diaper Scale" width="240" height="180" border="10" /></a>

Unfortunately the code for LibUSB is LGPL licensed so it is incompatible with the ASVL2 license that Apache MiNiFi-CPP uses so I am not able to contribute it to Apache MiNiFi-CPP project at this time. However anyone interested can view the code and get ideas or slightly modify it for use on their own. [GetUSB.cpp source code](https://github.com/jdye64/nifi-minifi-cpp/blob/libusb/libminifi/src/GetUSB.cpp)