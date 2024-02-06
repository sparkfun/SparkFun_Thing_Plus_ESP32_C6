## USB CDC on Boot Settings

Take note of the option labeled "USB CDC on Boot" when selecting the Board from the Tools menu. This option sets the serial outputs and defines their label for use in code. The SparkFun variants default to Enable USB CDC on boot which sets both <code>Serial</code> and <code>Serial0</code> as available serial ports. In this configuration, <code>Serial</code> corresponds to the direct USB/Serial converter on the chip (and the USB-C interface) and <code>Serial0</code> corresponds to the UART0 bus (default pins are 16 and 17).

With either setting, <code>Serial1</code> is available and refers to the UART1 bus (default pins are 4 and 5).

## RGB LED Pin

The board definition for the Thing Plus - ESP32-C6 sets IO23 to use espressif's `RGB_BUILTIN` code support. This automatically includes the necessary code to control an RGB LED easily when calling `RGB_BUILTIN`. Unfortunately, this means the RGB PTH pin (IO23) can run into code conflicts when users attempt to use it for another purpose. If you *really* need IO23 for something other than the RGB LED, you may need to modify the board definition files in the ESP32 Arduino boards package. Modifying these files is beyond the scope of this tutorial and is not supported by SparkFun.

## General Troubleshooting

!!! warning "Need Help?"
    If you need technical assistance or more information on a product that is not working as you expected, we recommend heading on over to the [SparkFun Technical Assistance](https://www.sparkfun.com/technical_assistanc) page for some initial troubleshooting.

    <center>
    [SparkFun Technical Assistance Page](https://www.sparkfun.com/technical_assistance){ .md-button .md-button--primary }
    </center>
    
    If you can't find what you need there, the [SparkFun Forums](https://forum.sparkfun.com/index.php) is a great place to search product forums and ask questions.
    
    !!! info "Account Registration Required"
        If this is your first visit to our forum, you'll need to create a [Forum Account](https://forum.sparkfun.com/ucp.php?mode=register) to post questions.