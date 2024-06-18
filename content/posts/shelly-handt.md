+++
title = "Setting up Shelly H&T Plus with Home Assistant"
author = ["Jack"]
lastmod = 2024-06-18T20:28:19+01:00
tags = ["home-assistant"]
draft = false
+++

## Introduction {#introduction}

I bought two Shelly H&amp;T plus devices a couple of months ago.
The reason for choosing them at the time was because:

-   They had a legible screen.
-   The company seemed to have a reasonable reputation.
-   There was an option to use the devices without their own apps (as in, local use only).
-   WiFi as a protocol seemed cleaner at the time, less to go wrong.

-- (In the meantime, I don't know if this is so true anymore).


## Setup {#setup}

Just some notes for myself next time I have to set these up..

1.  Pressing the button on the back for 5 seconds puts it into a setup mode where the device is a WiFI Access Point.

This means that you can connect to it directly via WiFi (as in, it will show up in your list of WiFi networks to connect to).
When this happens, go to the IP address 192.168.33.1.
From here, you then have all sorts of options.
In our case, we want to turn on an option called 'Outbound websocket'.
You will give it an address like: ws://192.XXXXX:8123/api/shelly/ws with SSL connectivity set up and a \* for the cert.
(There's some pickiness here on the capitalization I think, looking at other folks complaints online so keep all lowercase, just in case it's an issue).
When you make changes on the webserver, you'll often have to reboot the temperature sensor, so just be aware of that.
Also, because the device goes into sleep mode often, you'll quite likely have to press the button on the device to get these changes to be worked on.
Once that's all done, going back to the server webpage, it should tell you that it's all good now.
Then you go to the Home Assistant webpage and it should add the entity automatically.
Again, a restart of Home Assistant seemed necessary here.
