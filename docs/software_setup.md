---
icon: simple/arduino
---

!!! attention
	If this is your first time using Arduino, please read through our tutorial on [installing the Arduino IDE](https://learn.sparkfun.com/tutorials/installing-arduino-ide). If you have not installed an Arduino library before, we recommend you check out our [installation guide](https://learn.sparkfun.com/tutorials/installing-an-arduino-library).

With the ESP32-C6 Thing Plus connected to our computer, it's time to set up the boards package in Arduino.

## Installing espressif Arduino Boards

!!! important
    
    As of this writing, the Thing Plus ESP32-C6 is awaiting approval to be included in the alpha version of the ESP32 boards package (3.0.0-alpha2 currently) so it is *not* included in the alpha install but we're hoping it gets added very soon. We'll keep an eye out for the next update (whether it be to alpha or a full release of v3.0.0) and update this page once it is out.
    
To install the ESP32 boards package, open the Preferences menu by navigating to <b>File</b> > <b>Preferences</b>. Look at the bottom of the Preferences menu for "Additional boards manager URLS" and then copy this JSON link into that field:

<code>
    https://espressif.github.io/arduino-esp32/package_esp32_dev_index.json
</code>

Click "Ok" and then open the *Boards Manager* tool, search for "espressif ESP32" and install the latest alpha release (3.0.0-alpha2 or later). This install process may take some time so feel free to step away while it downloads and installs.

<figure markdown>
[![ESP32 Boards manager install.](./assets/img/espressif_arduino_boards.jpg){ width="600"}](./assets/img/espressif_arduino_boards.jpg "Click to enlarge")
</figure>

As mentioned above, the espressif ESP32 Arduino Boards package should soon include the Thing Plus - ESP32-C6. In the meantime, users can get most of the functionality from this board by selecting either the "SparkFun ESP32-C6 Qwiic Pocket" or the "ESP32C6 Dev Module". The Qwiic Pocket will have things like the Qwiic/I<sup>2</sup>C bus tied to the same pins as the Thing Plus.

## espressif IDF

Users who prefer to use espressif's development toolkit, espressif IDF, can get started by following their instructions [here](https://www.espressif.com/en/products/sdks/esp-idf) and  ESP32-C6 specific documentation [here](https://docs.espressif.com/projects/esp-idf/en/stable/esp32c6/index.html). 