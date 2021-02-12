# MidiArpeggiator

This project is based on https://github.com/raszhivin/arpeggio2 and has been refactored for
PlatformIO and run on an Arduino Nano microcontroller.

Hardware Requirements:

- Arduino Nano microcontroller
- Parts list: https://www.mouser.com/ProjectManager/ProjectDetail.aspx?AccessID=e3a21f7d7d

Software Requirements:

- ProjectIO core v5.1.0
- Visual Studio Code (recommended)

I strongly recommend using Visual Studio Code as your editor.  It's free from Microsoft and a full
functioned editor with a large library of plugins to meet your development needs.


    This firmware is designed to work with the REV 2 hardware design.  The breadboard layout and schematics are included
    in the wiki in this Github project for your reference.

# Arduino Analog Pins

The following **analog pins** on the Arduino Nano v3 board are defined as follows:

- Pin 0 :: Root octave
- Pin 1 :: Octave shift
- Pin 2 :: Pulse control
- Pin 3 :: Root note
- Pin 4 :: Arp steps
- Pin 5 :: Mode control
- Pin 6 :: Sequence octave control
- Pin 7 :: Order control

Each pin is wired to a 10Kohms linear potentiometer allowing user to set the value of each control.

    The pin numbers are defined in macros in `main.cpp`.  If you wish to rearrange the pins, simply update the corresponding macro value before compiling the code.

# LED Indicators

There are two LEDs in this design.  The Green LED (LED3) is a power indicator and lights up when power is applied to the device.  The Red LED (LED2) is a pushed button indicator and will light any time you push one of the buttons (except the power button).  Each are protected by a 220ohms resistor.

# MIDI Pinouts

 MIDI is a serial communication protocol for music devices.  The solder side of the connector pins are as follows:

 - Pin 1 :: Not used
 - Pin 2 :: Ground
 - Pin 3 :: Not used
 - Pin 4 :: 5V DC
 - Pin 5 :: Send (Serial TX)

# License & Authors

Copyright:: 2019 https://github.com/raszhivin

Copyright:: 2021 TGW Consulting, LLC.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
