bone2cloud_local
================

Bone2Cloud (Local) will allow you to control the LEDs on your BeagleBone Black (BBB) from your browser using Socket.IO and BoneScript to control a BeagleBone Black from a remote device. You'll be able to turn on/off LED's from a mobile device (cell phone, tablet) and read analog voltages from the 7 ADCs. The code uses Node.js as the web server, Socket.IO for communication between the web page and the BeagleBone Black, and Mobile JQuery for the web page lay-out.

Getting Started

What you'll need:

Beaglebone back Rev C.
for Windows user, you need to have Putty

Installation

Make sure you have an Internet connection through a network cable or Wifi. Connect to the BeagleBone Black by SSH. Set the current time just to be sure:
/usr/bin/ntpdate -b -s -u pool.ntp.org
Install Socket.IO:

cd /var/lib/cloud9
npm install socket.io
Download files from GitHub to the BeagleBone Black:

cd ~
git clone git://github.com/sensors2cloud/bone2cloud_local
cp bone2cloud_local/*  /var/lib/cloud9/
cd /var/lib/cloud9/
node bone2cloud_local.js

In the console you'll see something like this:
----------------------------------
-   Bone2Cloud (Local) v 0.0.4   -
----------------------------------
Server running on: http://192.168.1.69:8000

Go to the url in a web browser on your PC or other device. 

More info

Visit Sensors2cloud  for more information at http://www.sensors2cloud.com/openhw

Written by Sensors2cloud Inc.,.

MIT License. All text above must be included in any redistribution.
