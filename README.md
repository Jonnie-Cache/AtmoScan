## AtmoScan

Instructable can be found [HERE](https://www.instructables.com/id/AtmoScan/).  
See it in action in this [VIDEO](https://www.youtube.com/watch?v=iyFuKU8ZcuA).

**What's new** - Atmoscan is evolving:

* Some small hardware changes improved the original design, including the ability to **turn off itself from software**, remediating one of the biggest drawbacks of the design - how to handle low battery. 
* Command added to the setup **menu to turn off the device**
* White screen with low battery issue **mitigation**
* A PCB v2 design is now published together with a guide to easily **apply the change to boards V1.0.**
* Battery pack now based on 5 x 18650 Li-ion in "olympic circles" configuration. Way more performant and reliable than the chinese Li-Po pack
* Repositioning of the CO2 sensor, to completely separate the temperature sensor from any potential heat source
* CAD files for the **complete enclosure**, with improved design

Atmoscan might be (to my knowledge at least) the first ESP8266 application that **uses all GPIOs**, including those that allegedly cannot be used.

**ATMOSCAN** is a multisensor device that measures:

* Temperature
* Humidity
* Pressure
* CO2
* CO
* NO2
* VOC (Air Quality indicator)
* PM 01
* PM25
* PM10
* PM 01
* Radiation

It has an LCD color display, it is gesture controlled and it posts to ThingSpeak (or others) via MQTT, but can properly handle disconnected operations. With a rechargeable battery it lasts a full day when disconnected from power.

It uses a a multitasking cooperative framework and is very responsive to user input while sampling sensors, handling UI, posting to MQTT. I believe it squeezes quite a bit out of the tiny ESP8266...

It integrates a number of open source libraries and leverages internet web services. I started buiding the software with a proper OO application framework in mind and you can find artifacts of it... but never had the time to properly finish it the way i started, so i quickly completed it with way too many hacks. Therefore code could be way better (not properly commented, test code, residuals...).  If anyone is interested in contributing, it's very welcome.

I still have a few PCBs that i am happy to give away to those who want to build it and contribute to it.

### MAIN FEATURES
```
* Color screen
* Gesture control
* Location awareness
* ThingSpeak logging        
* Gracefully handles connected and disconnected operation
* 24h Rechargeable battery
* OTA updates
* Bonus features:
	* Weather Station
	* Plane Spotter

```


### CREDITS


**INCLUDES CODE & LIBRARIES FROM**

```
Adafruit
Arcao
Bblanchon
Bodmer
ClosedCube
Gmag11
Knolleary	
Lucadentella
Seeed
Squix78
Tzapu
Wizard97	
```

**INTEGRATES WEB SERVICES FROM**

```
Adsbexchange.com
GeoNames.org
Google.com
Mylnikov.org
Timezonedb.com
Wunderground.com
```

