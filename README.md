# Eagle-8: Pentium Pro for affordable boards

This is a Socket 8 to Slot 1 adapter (so called "slotket") which allows you to install Pentium Pro CPUs in Slot 1 motherboards. This project was mainly started because of the Socket 8 boards scarcity and limitations (no AGP bus, limited to EDO memory, etc) and being tired of having to deal with them. 

![Eagle-8 rev 1A PCBs](images/front.png)

Features:
- AM3 bracket holes + 3D printed spacer (modern AM3 CPUs sit lower than the Pentium Pro, so it has to be adapted)
- spot for an optional NTC thermistor located right under the CPU package; it is connected to the J3 header at the top
- spot for an optional 3-pin fan header, fed from the +5V pin in the Slot 1 connector
- FSB jumper with the option to run the slotket at 100MHz bus speed

There is an interactive HTML BOM which you can find [here](kicad/bom/ibom.html)

Support is experimental at the moment. The slotket will run on most boards with a Pentium II Overdrive CPU, because it is based on the Deschutes core.

However, as of now only 440FX based Slot 1 boards will run this slotket out of the box with a Pentium Pro. This is because most newer boards either lack Pentium Pro microcodes and/or have bugged BIOSes which freeze upon CPU speed detection. A few select ASUS boards received experimental patched BIOSes, which were kindly provided by Deniz Özmen on his [website](https://oezmen.eu/bios/), though keep in mind your mileage may vary.
