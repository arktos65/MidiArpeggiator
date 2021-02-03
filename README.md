# MidiArpeggiator

This project is based on https://github.com/raszhivin/arpeggio2 and has been refactored for
PlatformIO and run on an Arduino Uno microcontroller.

Hardware Requirements:

- Arduino Uno R3 microcontroller
- Parts list: https://www.mouser.com/ProjectManager/ProjectDetail.aspx?AccessID=e3a21f7d7d

Software Requirements:

- ProjectIO core v5.1.0

# Arduino Analog Pins

The following **analog pins** on the Arduino Uno R3 board are defined as follows:

- Pin 0 :: Root octave
- Pin 1 :: Octave shift
- Pin 2 :: N/A
- Pin 3 :: Pulse control
- Pin 4 :: Steps control
- Pin 5 :: Sequential octaves control
- Pin 6 :: Mode control
- Pin 7 :: Order control

Each pin is wired to a 10Kohms linear potentiometer allowing user to set the value of each control.

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
