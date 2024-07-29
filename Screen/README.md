# This page will tell you the ways to install the display driver in different operating system  
### First you need to install the operating system you need into RaspberryPi, this is the [tutorial](https://www.raspberrypi.com/documentation/computers/getting-started.html), when you choose device, select Raspberry Pi Zero 2W.
# Raspberry Pi OS  

Add the following line in `/boot/config.txt` in your TF card  

```sh
dtoverlay=vc4-kms-dpi-hyperpixel4sq
``` 
And the `config.txt` file will look like this:  
![image](https://github.com/user-attachments/assets/33139e0d-2477-4732-8ff5-a3e2bce9d383)  
Now you can insert the TF card in to the slot and your HackberryPi will run Raspberry Pi OS on the screen.  
![RaspberryPiOSfoto](https://github.com/user-attachments/assets/faff7b6f-a20e-45b8-801a-6f6dfe51b122)

# Kali Linux    

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
