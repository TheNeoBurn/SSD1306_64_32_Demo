# SSD1306_64_32_Demo
A working demo using the SSDD1306 64x32 0.49" OLED display via I²C

I tinkered and googled alot to find a working solution to use these displays with a Raspberry Pi. As I used a 128x64 0.96" display before, that was my starting point.

This solution is by no means perfect but I was unable to find another working one for Python yet.

## I²C bus speed

I advise to increese the baudrate on the I²C bus to improve refresh rates:

sudo nano /boot/config.txt

*uncomment and edit the line with for i2c:*

dtparam=i2c_arm=on,i2c_arm_baudrate=400000

