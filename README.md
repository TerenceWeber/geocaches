# Project Overview
At a high level, the project goal is to create a Witcher-style medallion that vibrates with increasing intensity when approaching any from a set of geocaches.

## Components
- 3D-printed medallion shell
- [ESP32-C3 microcontroller](https://a.co/d/04HP3uRo)
- [M10-12 GPS module](https://a.co/d/061m5ueC)
- [DRV2605L haptic driver](https://a.co/d/061m5ueC)
- [ERM vibration motor](https://a.co/d/0gel93cU)
- [Power switch](https://a.co/d/06c0i7uY)
- Interaction button (TBD)
- [380 mAh LiPo battery](https://a.co/d/04OjKxDo)

## Base Medallion STL File
Here is a link to the [medallion page](https://www.printables.com/model/357016-witcher-3-wolf-medallion). The **Files** tab has two seemingly identical STL files, so I assume the first one is the one to use.

## Modifications
The medallion will need several modifications to accommodate the project's various constraints and requirements.
- **Size**
  - The medallion will have to be scaled up overall to fit the internal components. How much is still TBD.
- **Compartment**
  - Due to the unfriendly shape of the base medallion, the back side of the medallion will need an extruded compartment to house the majority of the electronic components. The shape is up for debate. It could be a simple straight extrusion making a compartment the same shape as the flush back side of the medallion. Or the entire medallion could be mirrored then sheared to create a compartment that could lend a smoother overall look.
- **Top cutout**
  - The ceramic antenna of the GPS module needs to be sky-facing, so there needs to be a cutout on the topside of the medallion to expose it. Preferably it is not obviously visible, but not a dealbreaker if it is.  The module itself is 10x16mm and one of the short (10mm) sides has wires coming out (see the Amazon link's pictures) so accounting for the wires in the cutout size would be smart.
- **Bottom cutouts**
  - The bottom also needs some cutouts. Each of these should be spaced apart to give proper room for securing the components and for interacting with them cleanly, but close enough together (say, 2-3mm apart) to be aesthetically pleasing and compact. There are three cutouts to account for on the bottom:
    - The ESP32-C3 has a USB-C port for charging the battery and uploading code. It's a standard size USB-C port and it may be recessed a bit inside the medallion.
    - A power switch which is 8.7x3.7mm
    - A press button for interaction (acknowledge a geocache, factory reset, etc.). The size and model of this still TBD.
