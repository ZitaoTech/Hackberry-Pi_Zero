# This page will tell you the ways to install the display driver in different operating system and some using tips of the display  
### First you need to install the operating system you need into RaspberryPi, this is the [tutorial](https://www.raspberrypi.com/documentation/computers/getting-started.html#installing-the-operating-system), when you choose device, select Raspberry Pi Zero 2W.  
### There is a mini-HDMI port on the top side of HackberryPi. You can connect it with another screen. You can use the following commands to disable/enable the displaying.

```sh
vcgencmd display_power 0
vcgencmd display_power 1
```
### The default backlight brightness of the display after you turn HackberryPi on would be 50%. There is a physical button of the top side of HackberryPi. You can single press it to toggle the backlight of the display. You can also adjust the backlight brightness by long pressing the button: If you first long press the button the backlight brightness will slowly increase to 100%, if you now release the button and long press the button again, the backlight brightness of the display will slowly drop to 10%.  
# Raspberry Pi OS after 04/04/2022 or later  

Add the following line in `/boot/config.txt` in your TF card  

```sh
dtoverlay=vc4-kms-dpi-hyperpixel4sq
``` 
And the `config.txt` file will look like this:  
![image](https://github.com/user-attachments/assets/33139e0d-2477-4732-8ff5-a3e2bce9d383)  
Follow the steps:  
Insert the TF card in to the slot  
Turn on the HackberryPi, the screen will be black, wait until the white led on top stop blinking.  
Turn off the HackberryPi and reboot.  
And then your HackberryPi will run Raspberry Pi OS on the screen.  
![RaspberryPiOSfoto](https://github.com/user-attachments/assets/faff7b6f-a20e-45b8-801a-6f6dfe51b122)

# Kali Linux or Raspberry Pi OS before 04/04/2022   

### Step 1  
Add the following lines in `/boot/config.txt` in your TF card  

```sh
dtoverlay=hyperpixel4
overscan_left=0
overscan_right=0 
overscan_top=0
overscan_bottom=0
framebuffer_width=720
enable_dpi_lcd=1
display_default_lcd=1
dpi_group=2
dpi_mode=87
dpi_output_format=0x5f026
dpi_timings=720 0 20 20 40 720 0 15 15 15 0 0 0 60 0 36720000 4
```
And the `config.txt` file will look like this:  
![image](https://github.com/user-attachments/assets/eb698c68-0dce-4346-9013-562dcafa3381)

### Step 2  
Download the `hyperpixel4.dtbo`file in this github page   
Put the `hyperpixel4.dtbo`file into `/boot/overlays`folder  
Now you can insert the TF card in to the slot and your HackberryPi will run Kali Linux on the screen.  
![Kalilinux Foto](https://github.com/user-attachments/assets/59792d53-11be-4482-83eb-5bd8ca7a9110)
# RetroPi OS  
### Step 1  
Add the following lines in `/boot/config.txt` in your TF card  

```sh
dtoverlay=hyperpixel4
enable_dpi_lcd=1
dpi_group=2
dpi_mode=87
dpi_output_format=0x5f026
dpi_timings=720 0 20 20 40 720 0 15 15 15 0 0 0 60 0 36720000 4
```
And the `config.txt` file will look like this:  
![image](https://github.com/user-attachments/assets/40c5440e-34c2-45ca-aa42-7911d98e7115)

### Step 2  
Download the `hyperpixel4.dtbo`file in this github page   
Put the `hyperpixel4.dtbo`file into `/boot/overlays`folder  
Now you can insert the TF card in to the slot and your HackberryPi will run RetroPi OS on the screen.  
![RetroPiFoto](https://github.com/user-attachments/assets/8cc5cef6-7c7e-4d3f-ad7a-3357ff6c9ce3)

# DietPi  
DietPi is an extremely lightweight Debian OS, highly optimised for minimal CPU and RAM resource usage. The instruction is made by [Bjoern Franck](https://github.com/bjoernfranck)  
You can view the tutorial at this [page](https://github.com/bjoernfranck/HackberryPi/tree/main/DietPi)  
![image](https://github.com/user-attachments/assets/31e83c06-085c-4b7a-b38f-0236433038fb)
