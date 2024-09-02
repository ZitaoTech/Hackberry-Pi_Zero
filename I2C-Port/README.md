 First, don't enable I2C interface in raspi-config. Because the default I2C pins are used by the display. If you enable the I2C interface, the screen will be black. You need to connect HackberryPi to another display with an HDMI cable to disable the I2C interface to make it back.

The I2C pins on HackberryPi are: GPIO10 for I2C_SDA and GPIO11 for I2C_SCL  
There is a [STEMMA QT](https://learn.adafruit.com/introducing-adafruit-stemma-qt/what-is-stemma-qt) port on board, which means you can connect a sensor board with STEMMA QT port with HackberryPi through the I2C interface.  
On HackberryPi you need to open a terminal, and type:
``` sh
sudo ln -s /dev/i2c-11 /dev/i2c-1
```
to symlink i2c-11 to i2c-1 to fool any I2C devices into talking to the alternate one rather than the standard one.

Then you can just type this in a terminal:
``` sh
sudo i2cdetect -y 1
```
to check if the sensor is available.

![image](https://github.com/user-attachments/assets/f8abfa25-cc58-4e8e-89c7-4e42de650e48)
