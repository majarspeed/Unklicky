# Thank you Guys 
I love seeing the makes and all the questions and some awesome derivates are coming out of this project. 

Keep your eyes peeled there is a awesome revision on the horizon from Josar

And there is an amazing Euclind derivitive doen by Minisekt you can view [Unclid here](https://github.com/Minsekt/unclid).

There is new versions of the unklicky that is avaliable for the voron Stealth burner only currently. JosAr has integrated the the unklicky into the NG or next generations of Klicky. Check it out here https://github.com/jlas1/Klicky-Probe/tree/main/Probes

A great tutorial on Klicky/Unklicky was made by a member of the discord if you have any questions this should help for the setup. Thanks Logan BC 🇨🇦 VT.435 for creating such a great resouce. https://github.com/LoganFraser/VoronMods/tree/main/KlickySetup


# Unklicky

Drop in magnet based klicky probe In the orginal and now a 6x3 magnet variant called the BFP. 

![Top](https://github.com/majarspeed/Unklicky/raw/main/pictures/topview.png "Top")
![Botton](https://github.com/majarspeed/Unklicky/raw/main/pictures/Bottomview.png "Bottom")

Also keep in mind that klicky is based off the original work done over at Annex Engineering the excellent work that was done with the quickdraw probe. 
Thanks for calling this out. I did know the original was based on their work but it slipped my mind. They have an excellent group that does a lot of good things for the community. Support them in there work and thanks for keeping me honest here guys. 
https://github.com/Annex-Engineering/Quickdraw_Probe

Klicky is also based on [Euclid](https://www.euclidprobe.com/).

Thanks go to JosAR again for all the hard work and testing, please support his project and all the hard work he has done and is continuing to do. 
https://github.com/jlas1/Klicky-Probe

Testing with the auto z
While the switch offset can be changed by wire thickness on the wrap. 6mm seems to be a safe starting point for the the unklicky. And 3.2 seems to be a good starting point for the BFP. You can mesure from the body to the probe point to get the switch offset. And visit Protoloft and support him for all the work he has done on the auto z project. https://github.com/protoloft/klipper_z_calibration 


Parts kits thanks to DFH

[Buy full kit here](https://deepfriedhero.in/products/unklicky-full-kit-by-dustinspeed?_pos=1&_psq=unkl&_ss=e&_v=1.0&aff=8 "Full Unklicky Kit")

[Buy sidegrade kit here](https://deepfriedhero.in/products/unklicky-sidegrade-kit-by-dustinspeed?_pos=2&_sid=d0a66cc6e&_ss=r&aff=8 "Sidegrade Unklicky Kit")


## Versions and diffrences 
| Unklicky | useage |
| ------ | ------ |
| Unklicky |  The original. Made to retain the same shape and body as klicky. The only one to use 3x2 magnets in the pin. Uses wire wrapped pin method |
| Unklicky BFP | Larger body to allow the use of a 6 x 3 standard magnet. Uses the orginal wire wrapped pin method |
| Unklicky BFP-HS | Even Larger body to allow the use of a 6 x 3 standard magnet and a heatset in the pin to allow a shorter pin throw. And more clearance for wires. does not increase accuracy but does make the build easier. |
| Unklicky Z | First standard z endstop has multiple pin options. Uses the Heat set pin method and was intended to be modular and allow for customization of the pins |
| Unklicky Sexbolt | Sex bolt mod. Uses a single pin and 5mm OD chicago screw or sexbolt and 695/f695 bearing. |
| Unklicky Sexbolt-SBS (bearing sleeve) | Sex bolt mod. Uses a single pin and 5mm OD chicago screw or sexbolt. Allows the reuse of bearing sleeve from other sexbolt mods. |
| Unklicky Sexbolt Bearing free version | Sex bolt mod. Uses a single pin and 6mm OD and 5mm rod with  chicago screw or sexbolt.  |





# Unklicky Newest version 2
New version of the 3x2 probe is now available. This includes some QOL improvements. But does not really improve on any performance in any significant way. 
Added a screw mount on the rear so a magnet or screw can be used. May be useful if you have especially strong magnets.
Added a shaped pin that is easier to wire. And only inserts in one direction. 
New pin can be printed flat on the plate to make it easier to print and align the layer lines for smoother operation. 
V1 will be retained for now as well.


![V2 3x2](https://github.com/majarspeed/Unklicky/raw/main/pictures/3x2NP3.jpg "V2 3x2")

# BFP newest Version 6
added a alpha release under BFP
This is a 6x3 unklicky probe, it's a mod developed by me and JosAr.
![bfp](https://github.com/majarspeed/Unklicky/raw/main/pictures/BFP.jpg "BFP")

With the D-shaped shaft make sure there is no elephant foot to interfere with the motion. 
we have found for the wire to to the PIN/stalk it does seem to work better with a bare wire. 
Please feel free to reach out if you have any issues. 


# But how does it work!! 
There has been a lot of questions around this. So hopefully I can shed some light. 
The Probe uses an internal magnet on top of the pin/stalk. This magnet is not part of the circuit it is only used to provide a spring for the the probe. 

The real part of the probing is actually done by the screw. 
There is a contact point between the screw and the wire. This allows the unklicky to be normally closed. 
![Contact](https://github.com/majarspeed/Unklicky/raw/main/pictures/BFPContact.png "Contact")
![Left](https://github.com/majarspeed/Unklicky/raw/main/pictures/BFPIL.png "Left")

# But how well does it work!! 

Measurements were at 240 hotend, 95 bed, 55 chamber, on a Z belted [Tiny-M](https://github.com/gsl12/Tiny-M).
10k probe accuracy tests with 5 touches each. 
In the sense distance you can see the heatup at the start. And the consistency once up to temp.
![Deviation](https://github.com/majarspeed/Unklicky/raw/main/pictures/std%20deviation.png "Deviation")

Besides being one of the most precise switch's of the microswitch shootout (which will have soon a dedicated repository by JosAr), it withstood 50000 probes at 3mm/s

![sense distance](https://github.com/majarspeed/Unklicky/raw/main/pictures/Probe%20sense%20distance.png "sense distance")


































