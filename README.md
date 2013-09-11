Baofeng UV5R TRRS Adapter
=========================
http://github.com/johnboiles/BaofengUV5R-TRRS

Tiny board that allows you to connect the Baofeng UV5R radio to a smartphone or other device that uses a TRRS connector for audio. Useful for connecting the radio to a software TNC app such as [APRSDroid](http://aprsdroid.org/) or [PocketPacket](https://itunes.apple.com/us/app/pocketpacket/id336500866?mt=8). Solder on the components, solder on the cables, then provide some stress relief (I like zip ties and heat shrink), and you can use your UV5R with your smartphone for APRS on the cheap.

![Baofeng UV5R TRRS Adapter](http://johnboiles.s3.amazonaws.com/Screenshots/BaofengUV5R-TRRS.png)

Notes
-----
A small capacitor and 3 resistors to trick the iPhone into thinking a microphone was connected. This part of the schematic was inspired by [this article](http://www.creativedistraction.com/demos/sensor-data-to-iphone-through-the-headphone-jack-using-arduino/) on connecting Arduino to an iPhone.

A small capacitor on the speaker out of the radio removes any DC bias. (I'm not sure why this was necessary, but in my testing it made receipt of packets much more reliable.)

A diode tricks the radio into not activating PTT while still (sorta) connecting the grounds. (This is certainly a hack, and I'm very open to better ideas. Please submit an issue if you have ideas!)

On my UV5R+, volume is maxed, vox is set to 2 and, squelch is set to 1. On my iPhone volume is also maxed.

Schematic
---------
![Schematic](http://johnboiles.s3.amazonaws.com/Screenshots/BaoFeng%20to%20iPhone%20TRRS%20Cable%202.png)

Bill of Materials
-----------------
1x 3.5mm Stereo Cable

1x 2.5mm Stereo Cable

1x 3.5mm TRRS Cable

1x 10k Resistor 0603

2x 2.2k Resistor 0603

2x .1uF Capacitor 0603

1x Diode 1206