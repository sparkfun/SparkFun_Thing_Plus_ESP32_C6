---
icon: simple/arduino
---

!!! attention
	If this is your first time using Arduino, please read through our tutorial on [installing the Arduino IDE](https://learn.sparkfun.com/tutorials/installing-arduino-ide). If you have not installed an Arduino library before, we recommend you check out our [installation guide](https://learn.sparkfun.com/tutorials/installing-an-arduino-library).

With the ESP32-C6 Thing Plus connected to our computer, it's time to set up the boards package in Arduino.

## Installing espressif Arduino Boards

!!! important
    As of this board's release, espressif is currently working on an update to v3.0.0 for their Arduino boards package to include the Thing Plus - ESP32-C6 as a board variant (among other updates). Unfortunately, as of this writing, this version does <i>not</i> include the Thing Plus ESP32-C6 and is also in alpha phase at the moment so installing this package requires a few extra steps. Open the preferences menu by navigating to <b>File</b> > <b>Preferences</b>. Look at the bottom of the Prefences menu for "Additional boards manager URLS" and then copy this JSON link into that field:
    https://espressif.github.io/arduino-esp32/package_esp32_dev_index.json

    Click "Ok" and then open the Boards Manager tool, search for "espressif ESP32" and install the latest alpha release (3.0.0-alpha2 or later). This install process may take some time but when it completes, you can select "ESP32-C6 dev module" as the board to upload code to the Qwiic Pocket Development Board. We'll keep an eye out for the full release of v3.0.0 and update this page once it is out.

The espressif ESP32 Arduino Boards package should soon include the Thing Plus - ESP32-C6 though as of this writing it is not included. In the meantime, users can get most of the  Install it by opening the Boards Manager tab on the left side of the IDE, then search for "espressif ESP32" and install the latest version of the ESP32 boards package as the screenshot below shows. This assumes the use of Arduino 2.x. Legacy users (Arduino 1.8x and previous) can find the Boards Manager tool in File/Tools/Boards Manager.

<figure markdown>
[![ESP32 Boards manager install.](./assets/img/espressif_arduino_boards.jpg){ width="600"}](./assets/img/espressif_arduino_boards.jpg "Click to enlarge")
</figure>

## Addressable LED Library



## espressif IDF

Users who prefer to use espressif's development toolkit, espressif IDF, can get started by following their instructions [here](https://www.espressif.com/en/products/sdks/esp-idf) and  ESP32-C6 specific documentation [here](https://docs.espressif.com/projects/esp-idf/en/stable/esp32c6/index.html). 