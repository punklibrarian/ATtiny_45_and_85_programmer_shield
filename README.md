ATtiny 45 and 85 Programmer Shield - For Arduino
================================================
Copyright 2011 Design Tech Industries (DTI)

DTI email: <jameskun89@rocketmail.com>

The **ATtiny 45 and 85 Programmer Shield** is the product of a bored Saturday afternoon and using what I learnt from 
reading High-Low Tech's tutorial on programming an ATtiny 45 & 85 using an Arduino (http://hlt.media.mit.edu/?p=1229).

Features:

 * Pin compatible with Uno Arduino variants
 * ATtiny Pin 0 LED (for Blink sketch test) 
 * A 10uF capacitor between RST and GND to stop Arduino auto-resetting. 
 * Open Source; OSHW compliant
 * Design files freely available

In this repository you will find the gerber files for BatchPCB (http://batchpcb.com), along with project (.pro), board (.brd) 
and schematic (.sch) files for this shield in the 'EAGLE and 'KiCad' folders. Inside the 'EAGLE' folder you will find a folder
called 'eagleUp' which contains a 3D model of the shield in SKP format **(It also has the eagleUp files themselves which includes 
a PNG that can be used for home etching of the shield).**

**I release this design WITHOUT ANY WARRANTY. I created this for fun. Please check the design before using as I am not 
responsible if it fries something on your Arduino board.**

INSTALLATION
------------
**EAGLE**
The design is saved as an EAGLE project. EAGLE PCB design software is available from www.cadsoftusa.com 
free for non-commercial use and can be installed on Windows and Mac, with Linux support through WINE. 
To use this project download it and place the directory containing these files into the "eagle" directory 
on your computer. Then open EAGLE and navigate to Projects -> eagle -> ATtiny_45_and_85_programmer_shield.

**KiCad**
KiCad EDA Suite is an Open Source alternative to EAGLE. It is available on Windows and Linux and can be installed 
on Mac. It is available from http://kicad.sourceforge.net and works in a similar way to EAGLE. You will find project 
files for KiCad in the aptly named folder in this repository. To use this project download it and place the directory 
containing these files into a folder of your choice. Then open KiCad and navigate to File -> Open -> 
'FOLDER_OF_YOUR_CHOICE' -> ATtiny_45_and_85_programmer_shield.pro

HOW TO USE
----------
To get this to work you need to add ATtiny hardware definitions to your Arduino IDE. I use Wiring 1.0 (http://wiring.org.co/download/)
on Mac OSX Lion. I downloaded the ATtiny 45 and 85 hardware definitions from the High-Low Tech website 
(http://hlt.media.mit.edu/wp-content/uploads/2011/06/attiny45_85.zip) which I unzipped and placed the resulting folder into my sketchbook's
hardware folder (/Documents/Wiring/hardware). **You may need to create the 'hardware' folder if it doesn't already exist.**

You will also need to open the ArduinoISP (WiringISP) sketch from the examples menu and upload it to the Arduino you will be using this 
shield with. After that's done your Arduino is ready for the shield!

As an example try uploading the Blink sketch to test the shield and if it all works:

 * Open the Blink sketch from the examples menu.
 * Change the pin numbers from 13 to 0.
 * Select “ATtiny45 (w/ Arduino as ISP)” or “ATtiny85 (w/ Arduino as ISP)” from the **Tools > Board** menu (leave the serial port set to that of your Arduino board).
 *  Upload the sketch.

The shield has a built in LED connected to the ATtiny's pin 0 for convenience.

BILL OF MATERIALS
-----------------

4 x 1k 1/6 watt resistor (http://littlebirdelectronics.com/products/resistor-1k-ohm-1-6-watt-pth)
1 x ATtiny 45/85 µC (http://littlebirdelectronics.com/products/avr-8-pin-20mhz-8k-4ad-attiny85)
1 x 8-pin DIP socket (http://littlebirdelectronics.com/products/dip-sockets-solder-tail-8pin)
1 x 10mm Blue LED (http://littlebirdelectronics.com/products/diffused-led-blue-10mm)
1 x 5mm Green LED (http://littlebirdelectronics.com/products/basic-led-5mm-green)
1 x 5mm Red LED (http://littlebirdelectronics.com/products/basic-led-5mm-red)
1 x 5mm Yellow LED (http://littlebirdelectronics.com/products/basic-led-5mm-yellow)
1 x 10uF Capacitor (http://littlebirdelectronics.com/products/10uf-25v-rb-electrolytic-capacitor-105oc)
1 x Break Away Headers - Straight (http://littlebirdelectronics.com/products/break-away-headers-straight)

DISTRIBUTION
------------
The specific terms of distribution of this project are governed by the license referenced below.

LICENSE
-------
> This work is licensed under the Creative Commons Attribution-ShareAlike License.  
> 
> To view a copy of this license, visit:
> 
>   http://creativecommons.org/licenses/by-sa/3.0/  
>   http://creativecommons.org/licenses/by-sa/3.0/legalcode
> 
> or send a letter to
> 
>   Creative Commons  
>   171 Second Street, Suite 300  
>   San Francisco  
>   California, 94105  
>   USA

The "license" folder within this repository also contains copies of the
license(s) referenced above.