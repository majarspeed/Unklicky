# Unklicky TAP (unTAP)

This is a unklicky sensor for TAP. Thanks to the Voron team for this design and Badnoob for spearheading the effort and lead developer role.

It's almost as precise as the optical sensor, it's main goal is to reduce the initial Voron hug (a lot of people start buying the same obscure part, leaving it out of stock). With that said i can see one using it as a primary sensor as it can achieve a range in probing better than 0.003125 with a standard deviation of 0.000841.

**A range of 0.005 is excellent and enough for our 3D printer needs.** don't chase unicorns.

It's pretty easy to install, it does require a somewhat tuned printer.

This version, due to size requirements (needs to fit between TAP and X cable chains), it needs to replace TAP upper parts.

This is functionally  a drop in replacement/spare for the optical PCB for TAP, it uses it's own TAP upper part, but only requires 2 cables, a mcu GND (or V-) and the probe (should use a endstop) signal pin, it does not need a 5v or 24v connection.



| ![Unklicky TAP](./Photos/Unklicky_Tap_slim.png) |
| :---------------------------------------------: |

# How does it work?

The principle behind this sensor, is using the MGN12 steel carriage to make contact with two m2x10 self tapping screws, thereby closing the circuit between the mcu GND (or V-) and the probe (should use a endstop) signal pin.
Two 6x3 magnets makes the pin attract the probe body.

On the image bellow, you can see Unklicky TAP sensor touching the X axis MGN12 carriage.

| ![Unklicky TAP](./Photos/UnklickySlim_inaction.jpg) |
| --------------------------------------------------- |

More instructions below:

# What do I need?

## Bom
| Name | Pieces |
| ------ | ------ |
| M3 Heatset insert | 4 |
| 6x3mm Magnet | 2 |
|M2x10 self tapping screw| 2 |
|18 to 22 AWG wire| as required |



## Printed parts

| Name | Pieces |
| ------ | ------ |
| UnTAP_Body_v2.stl | 1|
|UnTAP_pins_v2| all |

There are more pins that may suit your printer better, see if any helps you on your issue (the 9mm pin for instance allow a 9mm screw to reach the carriage, a 10mm screw would go 1mm deeper into the MGN12 carriage.

The V2 version compared to the v1 is longer, so the screws are in a better location (some Carriages have a slot in the middle that can disturb the probing).

I recommend to print all the pins, they are really fast to print and it's a lot easier to print them at once.

### Printing instructions

The parts should be printed with the definitions below, they are oriented ready to print:

* initial layer height:0,24
* layer height: 0.2mm
* bottom/top/perimeters: 4
* infill: more than 30%
* infill type: Cubic
* Thin walls: On

The TAP Body requires supports, but they are included in the model.

## Build

| Instruction | Image |
| ------ | ------ |
|1. Print the parts as they are oriented and remove the body support.| ![Instructions](./Photos/Unklicky_Tap_slim_SS.png) |
|2. Insert the pin magnet, it should be insert until the it can no longer move. A small part of the magnet will remain outside the slot.| ![pin magnet](./Photos/UnklickySlim_1.jpg "Pin magnet") |
| 3. Rotate the pin and place it on the sensor body, with the magnet opening facing the back.<br />The pin magnet opening is facing the back in the image<br />Attach the other magnet to the outside of the body, and make sure that you respect that orientation when it is inserted on the probe body, both magnets should attract. |![body magnet orientation](./Photos/UnklickySlim_2.jpg "body magnet orientation")|
|4. respecting the polarity, insert the magnet in the sensor body, it should go all the way in, with a bit of force, then stay there. (the groove that holds the magnet was actually designed by Badnoob)<br />Verify that the pin moves freely and jumps back to its resting position reliably. If the pin sticks or jams, try lightly sanding the top and bottom layers.|![body magnet](./Photos/UnklickySlim_3.jpg "body magnet")|
|5. Slot one of the wires trough the side holes, screw a m2x10 self tapping screw on the hole, making sure it is solidly installed.<br />Repeat this procedure for the other side of the pin.| ![wire installation](./Photos/UnklickySlim_4.jpg "wire installation")<br />![wire installation](./Photos/Unklicky_5.jpg "wire installation") |
|6. the sensor is now ready to attach to TAP as it's upper body instead of the Optical PCB sensor + TAP upper part, you can use zip ties to secure both ends of the connectors, just leave room for the pin to move up and down.| ![final look](./Photos/UnklickySlim_6.jpg "Final look") |

## Klipper configuration

Below are the klipper specific unklicky TAP probe configuration, for the rest, please follow the TAP optical probe manual and procedures, they are the same.

```jinja2
[probe]
pin: ^Pin [should enable pullups "^" and use a endstop pin for better effect]
speed: 5
sample_retract_dist: 1.0
samples_tolerance: 0.05
samples_tolerance_retries: 3
```

## Initial run

After initial assembly, don't forget to check your Z probe offset, it will have changed.
**You should also condition the probe with the Klipper command "probe_accuracy samples=5000"** somewhere on top of the bed, it helps getting better results faster.
Speaking of faster, the best results for UnklickyTAP is between 5 and 10mm/s probe speed.

if you decide to use it, give me feedback, either here, or on Voron discord, my discord user is JosAr#0517, feel free to ping me in this channel  [Usermod probes help](https://discord.com/channels/460117602945990666/969563854071799818)

Please feel free to reach out if you have any issues. 



