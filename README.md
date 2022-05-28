# Ubo-HAT
This repo contains the schematic and layout design files as well as design overview for Ubo Top PCB / HAT. We will publish schematics and layout in Eagle CAD and plan to add KiCAD version as well. 

# System Design

In designing Ubo Top PCB (HAT), we tried to use popular components that have already gained adoption among the developer community and are developer friendly. In addition, we made sure that we can source these components for manufacturing. There are several development boards with one or several of these components that you can buy from either Sparkfun, Adafruit, Tindie, SeedStudio or other vendors. At the end of this repo, we have provided links to some of the development boards as reference.

The main objective in designing Ubo was centred around improving developer and end-user experience through offering a rich user interface. Since Raspberry Pi by itself is just a compute brain with no peripherals, it is often challenging to offer a compelling UX/UI to the end user without an interface.

In the following section, we discuss how each sub-system was chosen to enhance user and developer experience as well as technical details of implementation.  

## Sub-systems
In this section, we discuss each sub-system function, their purpose, and corresponing design decisions.

### Display
OLED versus TFT (OLED more cost effective but color depth)
Touch versus non-touch
Display size (0.54 inch in early prototypes) large rough to display essential information, QR code, etc
Cost
Decision

### keypad
7 buttons
5-way navigation switch, tedious experience and 
Menu system 

### LED ring
- Ring of 27 RGB LEDS arranged on the edge of the PCB

Communicate key informationa and notification silently from a distance 

### Infrared
- 4 IR Transmitters 
- 1 IR Receiver for code learning
### Temperature sensor
### Light sensor
### Audio
- Stereo Audio In/Out (2 microphones and 2 speakers)
### EEPROM 
- chip for automatic device tree population
### Security 
securely storing private keys
performing necessary crypo operations
license management for propritery software, secure wallets, etc
### Radio
- Optional Radio module
- Experimental features (Software defined radio)

# Breakout boards

Display
LEDs
Security IC:
Light Sensor
Temperature Sensor
GPIO Expander:
Audio:
Adafruit
SeeedStudio
WaveShare
IR

