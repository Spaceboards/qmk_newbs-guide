![Pinout](https://cdn-learn.adafruit.com/assets/assets/000/046/240/original/microcomputers_Adafruit_Feather_32u4_Basic_Proto_v2.3-1.png)

Do not use pins 14-16, they are reserved for the Bluetooth controller

Make sure that the LiPo you buy has Negative  (black) on the right side (closest to the Micro USB Port)

Short En and Gnd to turn off the 3.3v regulator, this disables LiPo and USB power

config.h add this
```
#define AdafruitBleResetPin D4
#define AdafruitBleCSPin B4
#define AdafruitBleIRQPin E6
```
rules.mk addition
```
BLUETOOTH = AdafruitBLE
```
	
