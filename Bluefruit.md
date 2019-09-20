
Do not use pins 14-16, they are reserved for the Bluetooth controller
Make sure that the LiPo you buy has negitibe (black) on the right side (closest to the Micro USB Port)

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
	