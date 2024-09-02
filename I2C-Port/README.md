 First, don't enable I2C interface in raspi-config. Because the default I2C pins are used by the display. If you enable the I2C interface, the screen will be black. You need to connect HackberryPi to another display with an HDMI cable to disable the I2C interface to make it back.

There is a [STEMMA QT](https://learn.adafruit.com/introducing-adafruit-stemma-qt/what-is-stemma-qt) port on board, which means you can connect a sensor board with STEMMA QT port with HackberryPi through the I2C interface.  
On HackberryPi 
