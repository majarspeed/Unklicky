# BFP Unklicky

This is a 6x3 unklicky probe. Thanks go to JosAR for all the hard work and testing. 
![bfp](https://github.com/majarspeed/Unklicky/raw/main/pictures/BFP.jpg "BFP")

# What do I need?

## Bom
| Name | Pieces |
| ------ | ------ |
| 6x3MM Magnet | 5|
|12 or 14 mm M3 screw| 1|
|18 to 22 AWG wire| <100 mm|

## Printed parts
| Name | Pieces |
| ------ | ------ |
| BFP_Unklicky_v6.stlt | 1|
|D_pin_v6.stl| 1|

## Build
| Instruction | Image |
| ------ | ------ |
| 1. Ensure that the pin can slide within the body freely; any excess friction can affect probe accuracy. Gently sand any spots that don't slide well. Make sure that the screw in the pin slot can slide up and down correctly.| |
| 2. Insert rear top magnet. | [<img src="https://github.com/majarspeed/Unklicky/raw/main/pictures/top_mag.jpg" width="250"/>](https://github.com/majarspeed/Unklicky/raw/main/pictures/top_mag.jpg) |
| **Note:** If using an existing dock, make sure the magnets are oriented to attract and not repel. For a new install, the pole needs to be the opposite of the front two that are installed later.| |
| 3. Strip the wire and wrap it around the pin with the starting point being on the D-Cut side. Use a single twist and then cut off any extra wire as any binding will cause problems later.| [<img src="https://github.com/majarspeed/Unklicky/raw/main/pictures/side%20wrap.jpg" width="250"/>](https://github.com/majarspeed/Unklicky/raw/main/pictures/side%20wrap.jpg)[<img src="https://github.com/majarspeed/Unklicky/raw/main/pictures/top_wrap.jpg" width="250"/>](https://github.com/majarspeed/Unklicky/raw/main/pictures/top_wrap.jpg)|
| **Note:** Multiple wraps can be used for thinner wires but take care to have it flat on the bottom of the pin so the magnet can seat correctly. See the above image.| |
|4. Place a magnet on top of the rear magnet installed in Step 1 and press the bottom of the pin against it to insert the magnet. You may need to slide the pin sideways to retain the magnet when removing. |[<img src="https://github.com/majarspeed/Unklicky/raw/main/pictures/mag_pin.jpg" width="250"/>](https://github.com/majarspeed/Unklicky/raw/main/pictures/mag_pin.jpg)|
| **Note:** This magnet will be pushed and not pulled, so it isn't critical for it to be super secure and you may find the fit fairly loose. This is by design to avoid having the pin bind up in the body. | |
|5. Thread the other end of the pin wire through the slot in the top of the body. Cut and strip the wire on top and insert the stripped end under either front magnet. | [<img src="https://github.com/majarspeed/Unklicky/raw/main/pictures/bottom_thread_hole.jpg" width="250"/>](https://github.com/majarspeed/Unklicky/raw/main/pictures/bottom_thread_hole.jpg)|
| **Note:** This will be easier to see and do in the newer revision of the body but it is very similar to threading a needle.| |
|6. Using a short piece of wire, strip one side and insert it into the hole before installing the screw. On top, strip the other side of the wire and insert it under the opposite front magnet from Step 5. |[<img src="https://github.com/majarspeed/Unklicky/raw/main/pictures/front_thread_hole.jpg" width="250"/>](https://github.com/majarspeed/Unklicky/raw/main/pictures/front_thread_hole.jpg)[<img src="https://github.com/majarspeed/Unklicky/raw/main/pictures/top_wired.jpg" width="250"/>](https://github.com/majarspeed/Unklicky/raw/main/pictures/top_wired.jpg)|
| **Note:** You can also wrap the wire around the screw before installing the screw.| |
|7. Once the screw from Step 6 is installed all the way, ensure the pin is pushed in and aligned correctly. It should slide with very little resistance. |[<img src="https://github.com/majarspeed/Unklicky/raw/main/pictures/front_screw.jpg" width="250"/>](https://github.com/majarspeed/Unklicky/raw/main/pictures/front_screw.jpg)|
|8. In Klipper, change both the z-height for the probe and the move height for QGL/Z-Tilt to 25mm. | |
|9. While this guide will not go into Auto-Z Calibration, switch_offset will need to be adjusted to ensure your appropriate probe behavior. The stock UnKlicky should have a switch_offset of about 6mm and the BFP about 3mm. This should set the probe to their maximums and you should adjust down as needed. The offset will vary based on the thickness of the wires used.  **PLEASE TEST!** I do not want to see pictures of damaged PEI sheets.||
|10. The rest of the build/install can proceed as with the normal [Klicky](https://github.com/jlas1/Klicky-Probe/blob/main/README.md). Glue can be used as needed but ensure that it doesn't interfere with electrical contact.| |
| **Note:** Images may not represent the current parts as they were taken with test parts.| |

## Contact

You can usually find me on the Voron Discord, so feel free to ping me using this link if you have any issues. 

[Help I broke my Unklicky](https://discord.com/channels/460117602945990666/969563854071799818). 

Discord name Dustinspeed#6423.