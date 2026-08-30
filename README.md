# Waveshare GC9A01A display driver for ZephyrRTOS.
This driver borrows the code and template of drivers/display/display_ili9xxx.c and .h

This driver is intended to be used in other projects, it is not a standalone app.

Note: All the development in this driver has been to mimic the "out of tree driver" development where minor changes will be implemented to make it work as a part of the main zephyr repository.

Out of tree driver development follow the pattern of https://github.com/teslabs/zds-2022-drivers-app and https://github.com/zephyrproject-rtos/example-application.


## Folder - drivers
1. drivers/display contains the core driver code for the GC9A01A display.

## Folder - dts
1. dts/bindings/display contains the device tree stuff for the GC9A01A display.
2. It is important for the intitialization sequence of the display and also configuring it as an SPI device.

## Folder - include
1. include/zephyr/dt-bindings folder contains include file that is used in the overlay to select the pixel format. This can be omitted but keeping it for further development.


Finally any support to make the driver work better or optimize it would be appreciated. 
